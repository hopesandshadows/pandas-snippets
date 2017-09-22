# pandas-snippets

# Columns 

## Get column list and values

`number = len(df.columns)`
`names = list(df.columns.values)`

`print(names, number)`

## count values from columns

`VARIABLE = df["COLUMNNAME"].value_counts()`

# Dataframe
## information about dataframe
`df.info()`

# Statistics
## descriptive stats of df
`df.describe()`

# Matplotlib
## display matplotlib inline
`%matplotlib inline`

# Histograms
## choose bin values
`df.hist(data, bins=[0, 10, 20, 30, 40, 50, 100])`

# Filter

## Create variables and then join

# Create variable with TRUE Player is Active 
`var1 = df['COLUMNNAME'] == 'Yes'`

# Create variable with False if club is Liverpool
`var2 = df['COLUMNNAME'] != 'Man U'`

# Create variable with False if name is John
`var3 = df['COLUMNNAME'] != 'John'`

# Filter all
`filtered = df[var1 & var2 & var3]`
