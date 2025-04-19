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

UrbanSentix/
├── README.md                      # Project overview
├── LICENSE                        # License file (e.g., MIT)
├── requirements.txt              # Python dependencies

├── data_sources/                 
│   ├── raw/                      # Unprocessed scraped data
│   ├── processed/                # Cleaned/structured data
│   └── external/                # CSVs/news articles/social media exports

├── data_scraping/
│   └── scrapy_spiders/          # Scrapy spiders for complaints, news, social
│       ├── complaints_spider.py
│       ├── news_spider.py
│       └── twitter_scraper.py

├── sentiment_analysis/
│   ├── text_cleaning.py         # Preprocessing scripts
│   ├── sentiment_spacy.py       # spaCy sentiment pipeline
│   └── sentiment_textblob.py    # TextBlob-based fallback

├── spark_processing/
│   ├── spark_job.py             # PySpark transformation scripts
│   └── config/                  # Spark session config and schema defs

├── database/
│   ├── duckdb_init.sql          # DuckDB table setup
│   ├── postgresql_schema.sql    # PostgreSQL schema setup
│   └── db_utils.py              # DB insert/query helpers

├── dashboards/
│   ├── powerbi/                 # PBIX files or export images
│   └── superset/                # Superset dashboard JSONs and configs

├── api/
│   └── app/                     
│       ├── main.py              # FastAPI entry point
│       ├── routes/             # API endpoints
│       └── models/             # Pydantic models and DB models

├── notebooks/                   # Jupyter notebooks for EDA & prototyping
│   └── exploratory_analysis.ipynb

└── utils/
    ├── helpers.py               # Shared utility functions
    └── logger.py                # Logging setup
