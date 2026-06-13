# 🚀 SpaceX Falcon 9 First Stage Landing — Exploratory Data Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-lightgrey?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-teal)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

## 📌 Project Overview

SpaceX advertises Falcon 9 rocket launches at **$62 million**, significantly less than competitors who charge upward of **$165 million**. The key to this cost saving is SpaceX's ability to **reuse the Falcon 9 first stage**.

This project performs an **Exploratory Data Analysis (EDA)** on SpaceX launch data to uncover patterns and factors that influence whether the Falcon 9 first stage lands successfully — a critical step toward understanding and predicting launch reusability.

**Workflow:**
1. **Data Collection (`API.ipynb`)** — Gathered Falcon 9 launch records via the SpaceX REST API
2. **Data Wrangling (`data wrangling.ipynb`)** — Cleaned, transformed, and labeled the data for analysis
3. **Exploratory Data Analysis (`EDA.ipynb`)** — Visualised patterns and relationships to identify factors affecting landing success

---

## 🎯 Objective

- Explore and understand the SpaceX Falcon 9 launch dataset
- Identify relationships between launch parameters and landing success
- Visualise key patterns across launch sites, orbits, payloads, and flight history
- Lay the analytical groundwork for a predictive classification model

---

## 📊 Dataset

- **Source:** IBM Data Science Capstone / SpaceX REST API & Wikipedia
- **Records:** SpaceX Falcon 9 historical launch data
- **Key Features:**
  - `FlightNumber` — sequential launch number
  - `LaunchSite` — location from which the rocket was launched
  - `PayloadMass` — mass of the payload in kg
  - `Orbit` — target orbit type (LEO, GTO, ISS, etc.)
  - `Outcome` — whether the first stage landed successfully

---

## 🛠️ Tools & Libraries

| Tool | Purpose |
|------|---------|
| Python | Core programming language |
| Pandas | Data loading, cleaning, and manipulation |
| NumPy | Numerical operations |
| Matplotlib | Base visualisations and charts |
| Seaborn | Statistical visualisations and heatmaps |
| Jupyter Notebook | Interactive analysis environment |

---

## 🔍 Key Analysis & Findings

### 1. 📍 Flight Number vs. Launch Site
- Explored how launch frequency is distributed across different SpaceX launch sites
- Found that **CCAFS SLC-40** handled the highest number of early launches, while **KSC LC-39A** gained prominence in later flights
- Later flight numbers (higher launch counts) show a stronger trend toward successful landings, indicating improvement over time

### 2. 📦 Payload Mass vs. Launch Site
- Analysed how payload mass varies by launch site
- Identified that certain launch sites are used for **heavier payloads**, and payload mass has a visible influence on landing outcome
- Lighter payloads generally showed higher landing success rates

### 3. 🌍 Success Rate by Orbit Type
- Compared landing success across orbit types including LEO, ISS, GTO, SSO, and others
- **LEO and ISS orbits** showed higher success rates compared to more demanding orbits like GTO
- Higher-energy orbits (e.g., GTO) are associated with lower first-stage recovery rates due to fuel constraints

---

## 📁 Project Structure

```
space-falcon-eda/
│
├── API.ipynb                       # Lab 1: Collecting launch data via SpaceX REST API
├── data wrangling.ipynb            # Lab 1-2: Cleaning and preparing the dataset
├── EDA.ipynb                       # Lab 2: Exploratory Data Analysis & visualisations
├── capstone-story-template 1.pdf   # Final capstone summary/report
└── README.md                       # Project documentation (this file)
```

---

## ▶️ How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/Pragati2411/space-falcon-eda.git
   cd space-falcon-eda
   ```

2. **Install dependencies**
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

3. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook EDA.ipynb
   ```

---

## 💡 Insights Summary

> Falcon 9 landing success has improved significantly over time. Launch site selection, payload mass, and target orbit are key factors influencing first stage recovery. These findings form the foundation for building a machine learning model to predict future landing outcomes.

---

## 🔗 Related Projects in This Series

| Project | Description |
|--------|-------------|
| EDA with SQL | Querying launch data using SQL for structured insights |
| EDA with Data Visualization | Advanced interactive visualisations of launch trends |
| ML — Loan Prediction | Classification model using Scikit-learn |

---

## 👩‍💻 Author

**Pragati** — Data Analyst | MSc Mathematics | IBM Data Science Professional Certificate  
📍 Surat, India | Open to Remote & Relocating to Mumbai / Hyderabad / Bangalore  
🔗 [GitHub Profile](https://github.com/Pragati2411)
