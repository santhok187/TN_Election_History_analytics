# Documentation

________________________________________

Tamil Nadu Election Analytics Project

End-to-End Data Engineering and Visualization Pipeline
________________________________________
1. Project Objective
The objective of this project was to design and implement an end-to-end Azure data pipeline that ingests, transforms, and visualizes Tamil Nadu election data. The solution demonstrates the ability to handle large-scale, India-specific datasets and deliver friendly dashboards that highlight historical trends, party performance, and voter behavior.
________________________________________
2. Data Acquisition
•	Source: Public election datasets containing constituency, candidate, party, votes, margins, and turnout percentages across multiple years.
•	Challenges: Data was fragmented across general elections and by-elections, with inconsistent formats.
•	Solution: Unified datasets into a standardized schema with key fields: 
    -year, district, ac_no, ac_name, candidate, party, totvotes, margin, poll_percentage.
________________________________________
3. Data Ingestion
•	Tools Used:
    -  	Azure Data Lake Storage Gen2 (ADLS) for raw data landing.
    -	ADF for automated ingestion of CSV files.
    -	Databricks (Standard Edition) for mounting ADLS containers and streamlined access.
•	Workflow:
    -	Raw files ingested into ADLS.
    -	Automated scripts ensured repeatable ingestion for new datasets.
________________________________________
4. Data Transformation
•	Schema Design: Unified general and by-election tables into a single silver layer.
•	Transformation Logic:
    -	Cleaned candidate and party names.
    -	Derived metrics such as winning_percentage.
    -	Joined tables to create dashboard-ready structures.
•	Output Format: Stored in Parquet/Delta for efficient querying and integration with Power BI.
________________________________________
5. Analytics & Visualization
•	Tool: Power BI connected directly to ADLS silver layer.
•	Dashboard Pages:
    1.	Overview: turnout trends, electors vs votes, district map.
    2.	Party Performance: Seats won per party per year, vote share distribution, top candidates.
    3.	Constituency Drilldown: Interactive filters by year/district, margin trends, constituency winners.
    4.	Historical Summary: Aggregated stats, party dominance timeline, competitiveness index.
________________________________________
6. Publishing & Portfolio Strategy
•	Local Sharing: .pbix file, PDF exports, and screenshots.
•	Portfolio Packaging: 
    -	GitHub repository with dataset, pipeline scripts, and dashboard visuals.
    -	README explaining project scope and technical stack.
    -	Optional demo video showcasing dashboard interactivity.
________________________________________
7. Key Learnings & Impact
•	Technical Depth: Automated ingestion, schema unification, DAX measures, and Power BI storytelling.
•	Business Value: Dashboard provides a compelling narrative of Tamil Nadu’s electoral history.
•	Recruiter Appeal: Demonstrates ability to build scalable pipelines, optimize cost, and deliver actionable insights.
________________________________________
8. Conclusion
This project highlights the integration of Azure, Databricks, ADLS Gen2, and Power BI to deliver a complete data engineering and analytics solution. It showcases both technical expertise and the ability to create business-impactful dashboards that resonate with recruiters and analysts.
________________________________________
-Dataset Courtesy: Kaggle (Public Election Data Repository)
