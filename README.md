# NYC Crime Complaints and Arrests Analysis

## Datasets

- [NYPD Complaint Data Historic](https://data.cityofnewyork.us/Public-Safety/NYPD-Complaint-Data-Historic/qgea-i56i)
- [NYPD Arrests Data Historic](https://data.cityofnewyork.us/Public-Safety/NYPD-Arrests-Data-Historic-/8h9b-rp9u)

## Download the 2025 data

Open a terminal in the project folder and run:

```bash
curl --progress-bar --get "https://data.cityofnewyork.us/resource/qgea-i56i.csv" --data-urlencode '$limit=1000000' --data-urlencode '$where=date_extract_y(rpt_dt)=2025' --output complaints_2025.csv
```

```bash
curl --progress-bar --get "https://data.cityofnewyork.us/resource/8h9b-rp9u.csv" --data-urlencode '$limit=1000000' --data-urlencode '$where=date_extract_y(arrest_date)=2025' --output arrests_2025.csv
```

Install the libraries

```bash
pip install pandas seaborn matplotlib geopandas
```
