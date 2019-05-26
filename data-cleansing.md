## What is "DATA CLEANSING"?
> Data Cleansing or Data Cleaning is the process of detecting and correcting(or removing) corrupt or inaccrurate records from a record set, table ,or database and refers to identifying incomplte, incorrect, inaccurate or irrelevant parts of the data and then replacing,modifying, or deleting the dirty or coarse data.
> from Wikipedia
#### main aspects:
- incomplete, such as missing/null
- inaccurate
- incorrect
-irrelevant


## How to explore data? 
#### main modules:
- import pandas as pd
- import numpy as np
- import matplotlib.pyplot as plt

#### main functions:
- .head()  #defalut value==5; display the first 5 lines
- .tail()  #default value==5; disply the last 5 lines
- .shape 
- .columns #display the list of column names in the format of list
- .info()  #display RangeIndex, number of data columns, memory usage, data types
- .describe() #display count, mean, std, min, 25%，50%，75% and max value of each column
- .value_counts() #df[column_name].value_counts displaying the counts of unique values in this column


