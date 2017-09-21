# pandas-snippets

#get column list

number = len(df.columns)
names = list(df.columns.values)

print(names, number)

#df info
df.info()

#descriptive stats
df.describe()

#count values from columns

VARIABLE = df["COLUMNNAME"].value_counts()

#display matplotlib inline
%matplotlib inline 
