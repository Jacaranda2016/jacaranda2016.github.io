# How to Use Flask and SQLAlchemy to Build Restful API?

CRUD(create,read, update, delete)

## About Database
### Models

###Marshmallow to do the serialization to ouput json

### RESTfull Route


###How to understand API
Application Program Interface provided by a server/host. 

###How to understand RESTful API?
1. 每一种URI代表一种资源
2. 数据格式
3. HTTP请求：GET,POST(new),PUT(update),DELETE

###理解装饰器
我们使用route（）装饰器来告诉Flask什么样的URL能够触发我们的函数，这个函数的名字也在生成URL时被特定的函数采用，这个函数返回我们想要显示在用户浏览器中的信息。

###app运行
if __name__ =="__main__" 确保应用只会在该脚本被Python解释器直接执行的时候才运行，作为模块导入的时候不会运行。？？？But why??


##Differences between Json and Python dictionary
我们会发现，从形式来讲，这两者的确很像，都为 key : value 的形式，那么它们两者的异同是什么呢？ 简单来说，python 字典的数据格式就json的数据格式。 
但本质上来讲，字典是一种数据结构，json是一种格式；字典有很多内置函数，有多种调用方法，而json是数据打包的一种格式，并不像字典具备操作性，
并且是格式就会有一些形式上的限制，比如json的格式要求必须且只能使用双引号作为key或者值的边界符号，不能使用单引号，而且“key”必须使用边界符（双引号），
但字典就无所谓了。

作者：凡人求索
链接：https://www.jianshu.com/p/33160c224732
来源：简书
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。

Hannah补充：
Boolean values in json： true， false
Boolean values in Python dict： True， False
