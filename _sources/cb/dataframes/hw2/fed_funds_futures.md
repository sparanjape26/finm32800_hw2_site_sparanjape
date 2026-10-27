# Dataframe: `hw2:fed_funds_futures` - 30-Day Fed Funds Futures (ZQ) Daily Bars

Daily OHLCV bars (schema ohlcv-1d) for every listed ZQ contract on CME Globex (dataset GLBX.MDP3, parent symbol ZQ.FUT), covering roughly the trailing six months. Prices are index points equal to 100 minus the implied average fed funds rate. The data includes calendar-spread symbols such as ZQU6-ZQZ6, which are filtered out downstream with fedwatch.filter_outright_contracts. Far-dated contracts trade thinly and may have no bar on some days, so use each contract's last available close. Historical data lags real time by about a day. The pull is free under the course subscription and is guarded by a $0.00 cost check.


## DataFrame Glimpse

```
Rows: 11751
Columns: 7
$ date   <datetime[ns]> 2026-10-25 00:00:00
$ symbol          <str> 'ZQG7-ZQJ7'
$ open            <f64> 15.5
$ high            <f64> 16.0
$ low             <f64> 15.5
$ close           <f64> 16.0
$ volume          <u64> 333


```

## Dataframe Manifest

| Dataframe Name                 | 30-Day Fed Funds Futures (ZQ) Daily Bars                                                          |
|--------------------------------|--------------------------------------------------------------------------------------|
| Dataframe ID                   | [fed_funds_futures](../dataframes/hw2/fed_funds_futures.md)                                       |
| Sources                        | CME Group                                          |
| Providers                      | Databento                                        |
| Provider Links                 | https://databento.com/                                   |
| Tags                           | Futures, Monetary Policy, Fed Funds                                             |
| Access Types                   |                                       |
| How is data pulled?            | Databento Historical API via Python                                                   |
| Data available up to (min)     | 2026-10-25 00:00:00                                                             |
| Data available up to (max)     | 2026-10-25 00:00:00                                                             |
| Dataframe Path                 | C:\Users\Lenovo\.vscode-shared\hw2-sparanjape26\_data\fed_funds_futures.parquet                                             |


**Linked Charts:**


- [hw2:fedwatch_latest_forecast](../../charts/hw2.fedwatch_latest_forecast.md)



## Pipeline Manifest

| Pipeline Name                   | HW 2: The Yield Curve and the Policy Path                       |
|---------------------------------|--------------------------------------------------------|
| Pipeline ID                     | [hw2](../../../index.md)              |
| Maintainer                      | Jeremiah Bejarano               |
| Contributors                    | Jeremiah Bejarano |
| Repository                     | https://github.com/hw-finm-32800/hw2                  |
| Pipeline Web Page               | <a href="file://C:/Users/Lenovo/.vscode-shared/hw2-sparanjape26/docs/index.html">Pipeline Web Page      |
| Date of Last Code Update        | 2026-10-26 23:07:45           |
| OS Compatibility                | Windows, Linux, macOS |
| Linked Dataframes               |  [hw2:crsp_treasury_consolidated](../../dataframes/hw2/crsp_treasury_consolidated.md)<br>  [hw2:fed_yield_curve](../../dataframes/hw2/fed_yield_curve.md)<br>  [hw2:fed_funds_futures](../../dataframes/hw2/fed_funds_futures.md)<br>  |


**Build Commands:**
```
doit

```

