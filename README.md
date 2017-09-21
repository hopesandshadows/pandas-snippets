# pandas-snippets

# get column list

`number = len(df.columns)`
`names = list(df.columns.values)`

`print(names, number)`

# df info
`df.info()`

# descriptive stats
`df.describe()`

# count values from columns

`VARIABLE = df["COLUMNNAME"].value_counts()`

# display matplotlib inline
`%matplotlib inline`

## Histograms
# choose bins
`df.hist(data, bins=[0, 10, 20, 30, 40, 50, 100])`
# If you just want them equally distributed, you can simply use range:

`plt.hist(data, bins=range(min(data), max(data) + binwidth, binwidth))`
