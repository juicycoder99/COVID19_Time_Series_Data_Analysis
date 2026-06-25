# COVID-19 Time-Series Data Analysis with pandas

Loading and reshaping the Johns Hopkins CSSE global confirmed-cases time series
(`time_series_covid19_confirmed_global.csv`) and analysing China's provincial data with pandas.

The implementation is in [`covid19_pandas_analysis.ipynb`](covid19_pandas_analysis.ipynb).

## Steps

1. Load the global confirmed-cases data from the CSV.
2. Count the total number of NaN values.
3. Replace the NaN values with the text `not available`.
4. Filter to China's data only.
5. Reset the index to start from 0.
6. Drop the `Country/Region`, `Lat` and `Long` columns.
7. Transpose the table so provinces are columns and daily cases are rows.
8. Analyse: total cases per province over the period, and a `describe()` summary.

## Running it

```bash
pip install pandas
jupyter notebook covid19_pandas_analysis.ipynb
```

## Files

| File | Description |
|------|-------------|
| `covid19_pandas_analysis.ipynb` | Full implementation and analysis |
| `PROJECT_BRIEF.pdf` | Project brief (goals, objectives, outcomes) |
| `time_series_covid19_confirmed_global.csv` | Source dataset (JHU CSSE) |
