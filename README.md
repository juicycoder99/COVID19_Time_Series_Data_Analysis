# Programming Languages for Data Analysis (CS405) — Assignment 1

Coursework for **Programming Languages for Data Analysis (CS405)**, Department of Computer Science,
Bishop's University.

## COVID-19 data analysis with pandas

Loading and reshaping the Johns Hopkins CSSE global confirmed-cases time series
(`time_series_covid19_confirmed_global.csv`) and analysing China's provincial data with pandas.

The solution is in [`Covid19_Assignment_1.ipynb`](Covid19_Assignment_1.ipynb).

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
jupyter notebook Covid19_Assignment_1.ipynb
```

## Files

| File | Description |
|------|-------------|
| `Covid19_Assignment_1.ipynb` | Full solution |
| `Covid19_Assignement_1_Student_version_2.pdf` | Assignment description |
| `time_series_covid19_confirmed_global.csv` | Source dataset (JHU CSSE) |
