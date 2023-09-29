Pandas
================================

## Get 1st and 3rd Fridays

```python
first = pd.date_range('2022-01-01', '2022-12-31', freq='WOM-1FRI')
third = pd.date_range('2022-01-01', '2022-12-31', freq='WOM-3FRI')
both = pd.Series(sorted(first.union(third)))
```
