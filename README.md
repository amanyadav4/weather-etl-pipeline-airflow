# 🌤 Weather ETL Pipeline with Airflow & Docker

This project demonstrates a simple end-to-end ETL pipeline using Python, Airflow, and Docker. It extracts weather data from OpenWeatherMap API, transforms it using Pandas, and loads it into a PostgreSQL database.

## 🚀 Features
- Python-based modular ETL
- Airflow DAG for scheduling
- Dockerized environment
- PostgreSQL for data storage

## 🛠 Setup Instructions

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/weather-etl-pipeline-airflow.git
cd weather-etl-pipeline-airflow
```

2. **Configure Environment**
```bash
cp .env.example .env
```
Fill in your `WEATHER_API_KEY` and `DB_URI`.

3. **Start Airflow with Docker Compose**
```bash
docker-compose up --build
```

4. **Access Airflow UI**
- URL: [http://localhost:8080](http://localhost:8080)
- Username: `admin`
- Password: `admin`

## 📁 Folder Structure
- `weather_etl/`: Python ETL modules
- `dags/`: Airflow DAG definition
- `.env`: Environment configuration
- `docker-compose.yml`: Docker config for Airflow and PostgreSQL

## 📊 Output
Data is stored in the `weather_data` table of your PostgreSQL database.

## 📌 Future Improvements
- Add historical weather data support
- Load data to cloud (S3, BigQuery)
- Add Streamlit dashboard
