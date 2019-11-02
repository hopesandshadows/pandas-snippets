# pandas-snippets

## Filter

### Create variables and then join

`var1 = df['COLUMNNAME'] == 'Yes'`

`var2 = df['COLUMNNAME'] != 0`

`var3 = df['COLUMNNAME'] != 'Something' `

### Filter all
`filtered = df[var1 & var2 & var3]`

## Method chaining

Most pandas methods return a DataFrame so that another pandas method can be applied to the result.

```python
df = (pd.melt(df)
      .rename(columns={
            'variable' : 'var',           
             'value' :})
      .query('val >= 200')
      )
```
