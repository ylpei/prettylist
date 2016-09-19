# prettylist

A simple Python library for easily displaying tabular data in a visually appealing ASCII list format

```python
p = PrettyList([
    Column(header='City name'),
    Column(header='Area', fmt=F_RIGHT),
    Column(header='Population'),
    Column(header='Annual Rainfall')
], noheader=False, sort='City name', sep=' | ')

p.add_row(['Adelaide', 1295, 1158259, 600.5])
p.add_row(['Brisbane', 5905, 1857594, 1146.4])
p.add_row(['Darwin', 112, 120900, 1714.7])
p.add_row(['Hobart', 1357, 205556, 619.5])
p.add_row(['Sydney', 2058, 4336374, 1214.8])
p.add_row(['Melbourne', 1566, 3806092, 646.9])
p.add_row(['Perth', 5386, 1554769, 869.4])

print(p)
```

```
City name | Area | Population | Annual Rainfall
Adelaide  | 1295 |    1158259 | 600.5
Brisbane  | 5905 |    1857594 | 1146.4
Darwin    |  112 |     120900 | 1714.7
Hobart    | 1357 |     205556 | 619.5
Melbourne | 1566 |    3806092 | 646.9
Perth     | 5386 |    1554769 | 869.4
Sydney    | 2058 |    4336374 | 1214.8
```
