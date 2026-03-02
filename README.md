# 📌 Sprint 12 — Open Data BCN (CKAN API)

## Description

This repository contains the practical exercises developed for **Sprint 12 – Open Data APIs**, focused on consuming public REST APIs to retrieve, explore and store real open data from the Barcelona City Council.

The project covers the complete data extraction workflow:
* Connection to the **Open Data BCN CKAN API**
* Dataset discovery and search using API endpoints
* Data extraction and transformation with **Pandas**
* Export of results to CSV for further analysis

The dataset used corresponds to **air transit data (Flightradar)** published by the Barcelona City Council.

---

## 📌 General Objectives

* Understand how REST APIs work and how to consume them with Python.
* Navigate a public data portal programmatically using API endpoints.
* Extract, filter and structure data returned in JSON format.
* Build a basic data pipeline from API call to CSV file.

---

## Specific Objectives

* Use `package_list` to retrieve the full catalogue of available datasets.
* Apply `package_search` to filter datasets by keyword.
* Use `package_show` to inspect dataset resources and identify valid formats.
* Query tabular data with `datastore_search`.
* Convert JSON responses into a Pandas DataFrame.
* Export the resulting dataset to a `.csv` file.

---

---

## Skills Practiced

* Connect to a public REST API using `requests`
* Browse and search datasets with `package_list`, `package_search` and `package_show`
* Query tabular data with `datastore_search`
* Convert API responses into a Pandas DataFrame
* Export results to CSV

---

## Project Structure

```
📁 Sprint_12_APIs
- PYTHON CODE: Sprint_12_APIs.ipynb
- opendata_bcn.csv
- Mapa conceptual APIs.JPG
- README.md
```

---

## Exercises Overview

### Level 1 — Dataset Discovery
Retrieve the full list of available datasets from the Open Data BCN portal using `package_list`.
* Explore dataset names and titles
* Identify datasets of interest using keyword filtering

### Level 2 — Keyword Search
Use `package_search` to filter datasets by topic.
* Search with keywords such as `"transit aeri"`
* Display dataset names, titles and number of available resources

### Level 3 — Data Extraction and Export
Select a dataset with CSV or JSON resources and extract data via the API.
* Use `package_show` to inspect dataset resources
* Select a valid `resource_id` from a CSV or JSON resource
* Retrieve at least 100 records with `datastore_search`
* Convert results into a Pandas DataFrame
* Save the DataFrame to a `.csv` file

---

## Technologies Used

* Python 3
* Pandas
* Requests
* Jupyter Notebook
* Open Data BCN — CKAN API

---

## Key Skills Demonstrated

* REST API consumption
* JSON parsing and data extraction
* Dataset search and filtering
* Data wrangling with Pandas
* Exploratory data analysis (EDA)
* CSV export

---

## API Reference

Base URL: `https://opendata-ajuntament.barcelona.cat/data/api/3/action/`

| Endpoint | Description |
|---|---|
| `package_list` | Full list of dataset names |
| `package_search?q=keyword` | Search datasets by keyword |
| `package_show?id=name` | Details and resources of a dataset |
| `datastore_search` | Query tabular data by resource ID |

More info: https://opendata-ajuntament.barcelona.cat/ca/desenvolupadors#APIS

---

## Learning Context

This project was developed as part of the **Data Analytics training program at IT Academy — Barcelona Activa**.  
Level: Beginner → Intermediate Data Analysis

---

## Author

**vbujaldon**
