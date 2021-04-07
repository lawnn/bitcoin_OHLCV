## OHLCV Data
使用例     
csv読み込み
```bash
import pandas as pd

def get_price_from_file(p):
    return pd.read_csv(p, index_col='time', parse_dates=True)


path = 'ohlc-30min.csv'
df = get_price_from_file(path)
```
範囲指定&期間指定     
```bash
df1 = df["2021-01-01 00:00:00": "2021-04-01"]
df2 = = df[60: 120]
```