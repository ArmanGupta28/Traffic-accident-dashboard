# 🚦 Big Data Traffic Accident Analysis

### Analyzing Traffic Accident Patterns Using Apache Spark, Hadoop Concepts, and Streamlit

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Apache Spark](https://img.shields.io/badge/Apache%20Spark-Data%20Processing-E25A1C?logo=apachespark&logoColor=white)](https://spark.apache.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-Dashboard-FF4B4B?logo=streamlit&logoColor=white)](https://streamlit.io/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Plotly](https://img.shields.io/badge/Plotly-Interactive%20Charts-3F4F75?logo=plotly&logoColor=white)](https://plotly.com/)

## 📌 Project Overview

**Big Data Traffic Accident Analysis** is a data analytics project designed to explore traffic accident records, identify accident patterns, and present meaningful insights through an interactive web dashboard.

The project uses publicly available New York City motor vehicle collision data. Python and Pandas are used for data preparation and analysis, while Apache Spark demonstrates distributed-style data processing and aggregation. Hadoop and MapReduce concepts provide the broader Big Data processing context.

An interactive Streamlit dashboard allows users to explore accident statistics, compare patterns, and visualize findings using charts and filters.

## 🎯 Objectives

- Analyze traffic accident records to identify significant patterns.
- Clean and preprocess real-world accident data.
- Apply Big Data processing concepts using Apache Spark.
- Demonstrate MapReduce-style aggregation for summarizing records.
- Visualize accident trends through interactive charts and a web dashboard.
- Make data-driven insights easier to understand and explore.

## ✨ Key Features

- **Real-world dataset:** Uses publicly available NYC motor vehicle collision records.
- **Data preprocessing:** Handles missing values, date conversion, and data cleaning.
- **Accident analysis:** Summarizes collision records and explores accident characteristics.
- **Spark processing:** Uses PySpark for data transformation and aggregation.
- **MapReduce concepts:** Demonstrates aggregation through mapping and reduction-style operations.
- **Interactive dashboard:** Provides a browser-based interface built with Streamlit.
- **Data visualization:** Uses Plotly to display interactive charts.
- **Time-based filtering:** Allows users to explore records over selected date windows, depending on available data.
- **Web-based access:** Enables users to view the dashboard without manually running analysis notebooks.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Pandas | Data cleaning and analysis |
| Apache Spark (PySpark) | Data processing and aggregation |
| Hadoop and MapReduce concepts | Big Data processing concepts |
| Streamlit | Interactive web dashboard |
| Plotly | Interactive data visualizations |
| Requests | Retrieving data from the public API |
| Jupyter Notebook / Google Colab | Development and experimentation |

> **Implementation note:** The project demonstrates Spark processing and MapReduce-style operations. A fully configured, multi-node Hadoop cluster is not required for the Streamlit dashboard to run.

## 📂 Dataset

The project uses the **NYC Open Data – Motor Vehicle Collisions (Crashes)** dataset.

- **Source:** NYC Open Data
- **Dataset:** Motor Vehicle Collisions – Crashes
- **API endpoint:** https://data.cityofnewyork.us/resource/h9gi-nx95.json
- **Data type:** Public traffic collision records

The dataset contains accident-related information such as crash dates, locations, and reported collision details. The fields available for analysis depend on the records returned by the API.

## 🏗️ Project Workflow

1. **Data collection:** Retrieve collision records from the NYC Open Data API.
2. **Data preprocessing:** Convert the retrieved records into a structured DataFrame, clean relevant fields, and process dates.
3. **Data transformation:** Prepare the data for aggregation and analysis.
4. **Big Data processing:** Demonstrate aggregation using Spark and MapReduce-style operations.
5. **Insight generation:** Summarize collision patterns and relevant statistics.
6. **Visualization:** Create charts and visual summaries using Plotly.
7. **Dashboard deployment:** Present the analysis through a Streamlit web application.

## 🧰 Project Structure

```text
traffic-accident-dashboard/
│
├── app.py
│   └── Streamlit dashboard application
│
├── Big_Data_Traffic_Accident_Analysis_Colab.ipynb
│   └── Data preprocessing and Big Data analysis notebook
│
├── requirements.txt
│   └── Python dependencies
│
├── README.md
│   └── Project documentation
│
└── .gitignore
    └── Files excluded from version control
```

*The structure above is illustrative. Keep only the filenames and folders that actually exist in your repository.*

## 🚀 Run the Project Locally

### 1. Clone the repository

```bash
git clone https://github.com/ArmanGupta28/traffic-accident-dashboard.git
```

### 2. Open the project folder

```bash
cd traffic-accident-dashboard
```

### 3. Create a virtual environment (recommended)

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

If the repository does not yet contain a `requirements.txt`, install the packages used by the dashboard:

```bash
pip install streamlit pandas plotly requests
```

If running the analysis notebook, install PySpark as well:

```bash
pip install pyspark
```

### 5. Launch the dashboard

```bash
streamlit run app.py
```

Streamlit will display a local URL, usually:

```text
http://localhost:8501
```

Open the URL in your browser to explore the dashboard.

**Note:** The dashboard requires an internet connection to retrieve records from the public NYC Open Data API.

## 📊 Expected Outcomes

The project is intended to help users:

- Explore traffic collision records interactively.
- Understand patterns in the available accident data.
- Examine summarized statistics and visual trends.
- Experience a practical application of Python-based analytics and Big Data processing concepts.
- Interact with a web dashboard instead of relying only on notebook outputs.

Actual findings depend on the records returned by the dataset API and the analyses implemented in the project.

## 🌐 Live Demo

**Streamlit Dashboard:**  
https://traffic-dashboard-2026.streamlit.app/

**GitHub Repository:**  
https://github.com/ArmanGupta28/traffic-accident-dashboard

> If the repository was not renamed successfully, update the GitHub URL to match the exact repository name shown in your browser.

## 🔮 Future Scope

- Integrate additional traffic accident datasets from different cities.
- Add geographical maps and location-based accident visualizations.
- Explore accident severity patterns and contributing factors where the data supports them.
- Introduce predictive models for estimating accident risk.
- Optimize processing for larger datasets.
- Integrate a properly configured Hadoop cluster for distributed storage and processing.
- Add automated data refresh and more advanced dashboard filters.

## 👥 Contributors

**Project Team:** Add the names and roles of all group members here.

- **Member 1:** Project development and data analysis
- **Member 2:** Dashboard development and visualization

*Update the roles to reflect the actual contributions of your team.*

## 🎓 Academic Project

This project was developed as an academic project to demonstrate practical applications of Big Data analytics, data processing, and interactive visualization.

## 📜 Data Source and Acknowledgment

Data is sourced from [NYC Open Data](https://opendata.cityofnewyork.us/). Please review the dataset's terms and applicable data-use requirements before redistribution.

---

⭐ If you find this project useful, consider giving the repository a star!
