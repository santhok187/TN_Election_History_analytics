# TN_Election_History_analytics

Repository for Tennessee election analytics.

Structure:
- Databricks/ — Databricks notebooks and jobs
- PowerBI/ — Power BI reports and assets
- docs/ — Documentation (architecture, runbooks, data dictionary)
- README.md — this file

Quick push (from repo root):
```
cd d:\Learning\Github_rep\TN_Election_History_analytics
git init                # if needed
git add .
git commit -m "Add project skeleton"
git branch -M main
git remote add origin <REMOTE_URL>
git push -u origin main
```


ingesting data from source to ADLS GEN2 (to automate ADF)
Loading the data from landing folder (RAW\elections\) to bronze (Curated\elections)
Transformaing the data into single silver layer (analytics)
Visualize it using the PowerBI

Dataset courtesy- Kaggle (https://www.kaggle.com/datasets/srinrealyf/1971-2021-tamilnadu-legislative-election-dataset)
