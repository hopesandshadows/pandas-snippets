# pandas-snippets

## Importing Data
### From a CSV file
`pd.read_csv(filename)`

### From a delimited text file (like TSV)
`pd.read_table(filename)`

### From an Excel file
`pd.read_excel(filename)`

### Reads from a SQL table/database
`pd.read_sql(query, connection_object)`

### Reads from a JSON formatted string, URL or file.
`pd.read_json(json_string)`

### Parses an html URL, string or file and extracts tables to a list of dataframes
`pd.read_html(url)`

### Takes the contents of your clipboard and passes it to read_table()
`pd.read_clipboard()`

### From a dict, keys for columns names, values for data as lists
`pd.DataFrame(dict)`


## Columns 

### Get column list and values

`number = len(df.columns)`
`names = list(df.columns.values)`

`print(names, number)`

### count values from columns

`VARIABLE = df["COLUMNNAME"].value_counts()`

## Dataframe
### information about dataframe
`df.info()`

## Statistics
### descriptive stats of df
`df.describe()`

## Matplotlib
### display matplotlib inline
`%matplotlib inline`

## Histograms
### choose bin values
`df.hist(data, bins=[0, 10, 20, 30, 40, 50, 100])`

## Filter

### Create variables and then join

`var1 = df['COLUMNNAME'] == 'Yes'`

`var2 = df['COLUMNNAME'] != 0`

`var3 = df['COLUMNNAME'] != 'Something' `

### Filter all
`filtered = df[var1 & var2 & var3]`
