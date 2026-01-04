---
title: Movie Data ETL Pipeline - Data Engineering Foundation Project
summary: This project showcases my ability to design and implement a complete local ETL pipeline, transforming raw movie CSV data into a clean, structured SQLite database ready for SQL analysis.
date: 2026-01-03
authors:
  - me
tags:
  - Data Engineering
  - Career Journey
  - Search Evaluation
cover:
  image: "cover.jpg"
image:
  filename: featured.jpg
  caption: 'Image credit: Photo by [**Igor Dias**](https://unsplash.com/@igordias1982) on [**Unsplash**](https://unsplash.com)'
---

## Overview
This project showcases my ability to design and implement a complete local ETL pipeline, transforming raw movie CSV data into a clean, structured SQLite database ready for SQL analysis.

> [!NOTE]+ NOTE  
> This project intentionally focuses on correctness and reproducibility, not scale or performance optimization.

---

## Business Problem
Raw datasets are rarely analysis-ready. In this project, movie data suffered from:

- Inconsistent formats and missing values  
- Multi-valued fields that break relational queries  
- No enforced schema or data type guarantees  

> [!WARNING]+ IMPORTANT  
> Without proper normalization and schema enforcement, SQL queries may return misleading or incorrect results, even if they run successfully.

The objective was to convert this raw data into a trustworthy, queryable dataset using sound data engineering practices.

---

## Solution
I built a Python-driven ETL pipeline that:

- Cleans and standardizes raw CSV data  
- Normalizes multi-valued attributes for relational storage  
- Enforces data types before loading  
- Stores the final result in a structured SQLite database  

This ensures the data can be reliably queried and extended in future pipelines.

---

## End-to-End Pipeline
```text
Raw CSV → Python (pandas) → Processed CSV → SQLite → SQL Queries
```
---

## Key Contributions
- Designed a **rerunnable ETL script** (not a one-off notebook)  
- Implemented **data normalization** for accurate SQL aggregation  
- Defined and enforced a **relational schema** in SQLite  
- Validated outputs using **SQL analytical queries**  
- Maintained a **clean, well-documented GitHub repository**  

---

## Tools & Technologies
- **Python (pandas)** for data transformation  
- **SQLite & SQL** for structured storage and querying  
- **Git & GitHub** for version control and documentation  
- **Command-line environment** for local execution 

> [!TIP]+ TIP  
> SQLite is a great choice for learning because it lets you focus on schema design and SQL fundamentals without dealing with database setup or infrastructure.

---

## Results
- Raw movie data converted into a **query-ready relational table**  
- Multi-valued genres transformed into **atomic, SQL-friendly records**  
- Reliable analytical queries enabled **without schema or type errors**  

---

## Why This Project Matters
This project demonstrates:

- Practical understanding of **ETL fundamentals**  
- Awareness of how **schema decisions affect downstream analysis**  
- Ability to move from **raw data to structured systems**, not just analysis  
- Engineering habits focused on **reproducibility and maintainability**  

---

## Links
- **GitHub Repository:**  
  https://github.com/faqihalamin95/movie-genre-analysis  

- **Technical Reflection:**  
  [*Closing Phase 1 – Building My Data Engineering Foundation*](https://datadonut.netlify.app/blog/closing-phase-1/)

---

## Next Steps
This foundation project is followed by **Phase 2**, which will focus on:

- Data modeling and normalization  
- Working with more structured local databases  
- Building repeatable and slightly more automated ETL workflows  