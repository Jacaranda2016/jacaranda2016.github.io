I am new to Flask and the most well-known Python ORM SQLAlchemy. I will record my learning notes and some significant erorrs I met here.

## ERROR 1
```
ModuleNotFoundError: No module named 'MySQLdb'
```
### Debugging
1.check whether pymysql has been installed or not. if no, install it; if yes
2. check db URI 
dialect+driver://username:password@host:port/database
for mysql:
mysql+pymysql://username:password@host:port/database

## Issue 2 How to configure the engine when using flask_sqlalchemy
As we know, flask_sqlalchemy is a lightweight ORM module for flask 

```
#config the db address
app.config['SQLALCHEMY_DATABASE_URI'] = db_URI
app.config['SQLALCHEMY_COMMIT_ON_TEARDOWN'] = True
db = SQLAlchemy(app)
```

#### more configurations
```
app.config['SQLALCHEMY_ECHO']=True #logs
app.config['SQLALCHEMY_POOL_SIZE']=100 #default pool size is 5
app.config['SQLALCHEMY_POOL_RECYCLE']=290  #This number should < database server timeout time.
```
The configurable keywords 
https://flask-sqlalchemy.palletsprojects.com/en/2.x/config/?highlight=pool


## Issue 3 how to configure the engine to pool preping to avoid the long idle and timeout error

!! This can't be configured in the current version of flask_sqlalchemy

!! Even set the configuration using SQLALchemy shown below, it still does not work.
``` python
engine = create_engine(
    "mysql+pymysql://username:password@host:port/database",
    connect_args = {
        "port":3306
    },
    echo="debug",
    echo_pool="debug",
    pool_recycle=290,
    pool_pre_ping=True,
    pool_use_lifo=True,
)
```

### solution: using sqlalchmey session_factor and flask_scoped_session

```
from flask_sqlalchemy_session import flask_scoped_session
from sqlalchemy.orm import sessionmaker  

session_factory = sessionmaker(bind=engine)
session = flask_scoped_session(session_factory, app)
```
And in this way, don't have create a new session for each process because we are using session factory to handle the session creation, preping
and recyle. 


