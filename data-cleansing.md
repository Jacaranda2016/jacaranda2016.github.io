## What is "DATA CLEANSING"?
> Data Cleansing or Data Cleaning is the process of detecting and correcting(or removing) corrupt or inaccrurate records from a record set, table ,or database and refers to identifying incomplte, incorrect, inaccurate or irrelevant parts of the data and then replacing,modifying, or deleting the dirty or coarse data.
> from Wikipedia
#### Main Aspects:
- incomplete, such as missing/null
- inaccurate
- incorrect
-irrelevant


## How to explore data? (1)
#### Main Modules:
- import pandas as pd
- import numpy as np
- import matplotlib.pyplot as plt

#### Main Functions:
- .head()             #defalut value==5; display the first 5 lines
- .tail()             #default value==5; disply the last 5 lines
- .shape 
- .columns            #display the list of column names in the format of list
- .info()             #display RangeIndex, number of data columns, memory usage, data types
- .describe()         #display count, mean, std, min, 25%，50%，75% and max value of each column
- .value_counts()     #df[column_name].value_counts displaying the counts of unique values in this column


## How to explore data? (2)
Besides the methods above, we also can use diagrams to help us to understand the data. 
#### Main Modules:
- import matplotlib.pyplot as plt
### Main Diagrams
- bar chart
- scatter 
- hist
- line chart
- box 
- ...

#### Static or interactive?

### libraries for better visualization
- seaborn
- altair
- ...

## How to clean data?
### Remove columns/rows
1. remove from reading stage
``` pd.read_csv()```
```
pd.read_csv(
    ['filepath_or_buffer', "sep=','", 'delimiter=None', "header='infer'", 'names=None', 'index_col=None', 'usecols=None', 'squeeze=False', 'prefix=None', 'mangle_dupe_cols=True', 'dtype=None', 'engine=None', 'converters=None', 'true_values=None', 'false_values=None', 'skipinitialspace=False', 'skiprows=None', 'nrows=None', 'na_values=None', 'keep_default_na=True', 'na_filter=True', 'verbose=False', 'skip_blank_lines=True', 'parse_dates=False', 'infer_datetime_format=False', 'keep_date_col=False', 'date_parser=None', 'dayfirst=False', 'iterator=False', 'chunksize=None', "compression='infer'", 'thousands=None', "decimal=b'.'", 'lineterminator=None', 'quotechar=\'"\'', 'quoting=0', 'escapechar=None', 'comment=None', 'encoding=None', 'dialect=None', 'tupleize_cols=None', 'error_bad_lines=True', 'warn_bad_lines=True', 'skipfooter=0', 'doublequote=True', 'delim_whitespace=False', 'low_memory=True', 'memory_map=False', 'float_precision=None'],
)
```
- header=0 by default. If you want to escape row 0, you can set "header=1"
- nrows-- how many rows you want
- usecols-- which columns you want to import,using[0,1,3] or column names to choose the specific columns
         -- you can use df.columns to check all the columns and then choose the subset of columns you need


## Open data
1. [open data from Newyork City](https://opendata.cityofnewyork.us/)

