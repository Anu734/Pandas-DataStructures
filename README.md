# Pandas-DataStructures
What is a Series? A Pandas Series is like a column in a table.  It is a one-dimensional array holding data of any type.
provides two main data structures:
Series – 1D labeled array
DataFrame – 2D labeled table (like Excel)
### What is a Series?
A Pandas Series is like a column in a table.
It is a one-dimensional array holding data of any type.
  # FEW EXAMPLES OF PANDAS SERIES  
# EXAMPLE -1
import pandas as pd
  a = [1, 7, 2]
  myvar = pd.Series(a)
print(myvar)

# EXAMPLE - 2
import pandas as pd
data = [10, 20, 30]
s = pd.Series(data)
print(s)

## 2. DATAFRAME 
 ### WNHAT  IS DATAFRAME ?
Data sets in Pandas are usually multi-dimensional tables, called DataFrames.
Series is like a column, a DataFrame is the whole table.
## CREATING DATAFRAME;
import pandas as pd
df = pd.DataFrame()
print(df)
## VARIOUS TASK  TO 
 ### Task	Code
Check null values:    	df.isnull().sum()
Replace values :       	df['col'].replace(old, new)
Drop rows/columns:	      df.drop(index=0) or df.drop(columns='col')
Reset index	:            df.reset_index(drop=True)
Set index :            	df.set_index('column')
##  Grouping Data
df.groupby('City')['Age'].mean()
## Example - 1
# Create a simple Pandas DataFrame:

import pandas as pd

data = {
  "calories": [420, 380, 390],
  "duration": [50, 40, 45]
}
## Example - 2
#load data into a DataFrame object:
df = pd.DataFrame(data)

print(df) 
Pandas use the loc attribute to return one or more specified row(s)

Example
Return row 0:

#refer to the row index:
print(df.loc[0])
