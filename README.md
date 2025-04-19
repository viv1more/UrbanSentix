# 🚀 UrbanSentix – Sentiment Analysis on City Services

UrbanSentix is a Big Data-powered sentiment analysis project focused on understanding public opinion about **city services** using real-time and historical data. This project uses scalable, open-source tools and is designed to be **lightweight** and **compatible**.

---

## 🎯 Project Goals & Scope

- **Objective:**  
  Analyze citizen feedback to understand sentiment trends on urban services like water, roads, sanitation, and public safety.

- **Target Outcomes:**  
  - Identify positive and negative public sentiment  
  - Provide real-time insights to authorities  
  - Enable proactive decision-making for urban management  

---

## 📊 Data Sources

- 🗣 **Citizen Complaints** – Government portals, city websites  
- 🌐 **Social Media** – Twitter, Reddit, Facebook  
- 📰 **News Articles** – Local news platforms and city bulletins

---

## 🧰 Tech Stack (Windows & Hadoop-Free)

| Layer               | Tool/Tech                | Purpose                                |
|---------------------|--------------------------|----------------------------------------|
| 🔍 Data Collection   | `Scrapy`                 | Scraping complaints, posts & news      |
| ⚙ Data Processing    | `PySpark (Standalone)`   | Scalable data processing               |
| 🧠 NLP & Sentiment   | `spaCy`, `TextBlob`      | Text cleaning & sentiment scoring      |
| 🛢️ Data Storage       | `DuckDB`, `PostgreSQL`    | Lightweight + structured DB storage    |
| 📈 Visualization      | `Apache Superset`, `Power BI` | Dashboards and real-time insights  |
| 🔗 API Integration   | `FastAPI`                | Real-time access to sentiment data     |

---

## 📌 Key Features

- ✔️ Multi-source sentiment tracking  
- ✔️ Dashboard with filtering by date, location, and topic  
- ✔️ Lightweight, no external Hadoop setup required  
- ✔️ Real-time API for integration with external apps  

---

## 📁 Folder Structure

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
   
</head>
<body>
    <h2>Project Directory Structure</h2>
    <pre>
UrbanSentix/
├── data_sources/              # Raw, processed, and external datasets
│   ├── raw/                   # Unprocessed scraped files
│   ├── processed/             # Cleaned and structured data
│   └── external/              # Social media exports, news archives
├── data_scraping/             # Web scraping scripts using Scrapy
│   └── scrapy_spiders/
│       ├── complaints_spider.py
│       ├── news_spider.py
│       └── twitter_scraper.py
├── sentiment_analysis/        # NLP-based sentiment analysis
│   ├── text_cleaning.py
│   ├── sentiment_spacy.py
│   └── sentiment_textblob.py
├── spark_processing/          # PySpark scripts for Big Data processing
│   ├── spark_job.py
│   └── config/
│       └── spark_config.json
├── database/                  # SQL setup and DB utilities
│   ├── duckdb_init.sql
│   ├── postgresql_schema.sql
│   └── db_utils.py
├── dashboards/                # Visual dashboards
│   ├── powerbi/               # Power BI dashboards (.pbix or screenshots)
│   └── superset/              # Superset configs or exports
├── api/                       # FastAPI service
│   ├── main.py
│   ├── routes/
│   └── models/
├── notebooks/                 # Jupyter notebooks for EDA or prototyping
│   └── exploratory_analysis.ipynb
├── utils/                     # Helper functions and logging
│   ├── helpers.py
│   └── logger.py
├── requirements.txt           # Python dependencies
├── LICENSE                    # License file (MIT, Apache, etc.)
└── README.md                  # You're here! :)
    </pre>
</body>
</html>
