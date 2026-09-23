# 🚀 Astrolytics

**A data-driven exploration of the Space Race — from Sputnik in 1957 to the present day.**

Astrolytics is a Python-based data analysis project that digs into more than six decades of space mission history. Using a dataset of **4,300+ launches** scraped from [nextspaceflight.com](https://nextspaceflight.com/launches/past/?page=1), this project explores launch trends, mission costs, success/failure rates, and the historic USA vs. USSR rivalry that kicked off the era of spaceflight.

---

## 📊 What This Project Does

Astrolytics answers questions like:

- Which organisations have launched the most rockets — and who dominates today?
- How many rockets are still active vs. retired?
- How expensive is a launch, and how has that cost changed over time?
- Which countries lead in total launches and mission failures? *(visualized on choropleth maps)*
- How did the Cold War-era Space Race between the USA and USSR play out year by year?
- Which months are the most popular for launches?
- Who led the "launch race" globally, year by year, from 1957 to 2020?

The analysis is presented as a fully worked Jupyter notebook, combining data cleaning, descriptive statistics, and rich interactive visualizations.

---

## 🛠️ Tech Stack

- **Python 3**
- **pandas** & **numpy** — data cleaning, wrangling, and analysis
- **matplotlib** & **seaborn** — statistical plotting
- **plotly** (`plotly.express`) — interactive charts, choropleth maps, sunburst charts
- **iso3166** — mapping country names to ISO codes for geographic visualizations
- **Jupyter Notebook**

---

## 📁 Project Structure

```
astrolytics/
├── mission_launches.csv                       # Raw dataset (4,324 launch records)
├── Space_Missions_Analysis__start_.ipynb       # Starter notebook (unsolved / template)
├── Space_Missions_Analysis__solved_.ipynb      # Full analysis with visualizations
└── README.md
```

---

## 📦 Dataset

The dataset (`mission_launches.csv`) contains launch records with the following fields:

| Column          | Description                                      |
|-----------------|---------------------------------------------------|
| `Organisation`  | Agency or company that conducted the launch       |
| `Location`      | Launch site                                        |
| `Date`          | Date and time of launch (UTC)                      |
| `Detail`        | Rocket and payload/mission details                 |
| `Rocket_Status`  | Whether the rocket is currently active or retired  |
| `Price`         | Estimated cost of the launch (USD, millions)       |
| `Mission_Status` | Outcome of the mission (Success / Failure, etc.)   |

---

## 🔍 Key Sections in the Analysis

1. **Preliminary Data Exploration** — cleaning missing values, duplicates, and descriptive stats
2. **Launches per Company** — who's launching the most rockets?
3. **Active vs. Retired Rockets**
4. **Mission Status Distribution**
5. **Launch Cost Analysis** — how expensive is spaceflight, and by whom?
6. **Choropleth Maps** — launches and failures by country
7. **Sunburst Chart** — countries → organisations → mission outcomes
8. **Spending Analysis** — total and per-launch spend by organisation
9. **Launch Trends Over Time** — yearly and month-on-month patterns
10. **Cold War Space Race** — USA vs. USSR launches, failures, and failure rates over time
11. **Year-by-Year Leaders** — which country/organisation led the launch count each year

---

## ▶️ Getting Started

### Prerequisites
Make sure you have Python 3 and Jupyter installed, then install the required packages:

```
pip install numpy pandas matplotlib seaborn plotly iso3166
```

### Running the Notebook

```
git clone https://github.com/rhitamcoder/astrolytics.git
```
```
cd astrolytics
```
```
jupyter notebook Space_Missions_Analysis__solved_.ipynb
```

If you'd like to work through the analysis yourself, start with `Space_Missions_Analysis__start_.ipynb` instead — it contains the setup and questions without the completed solutions.

---

## 📈 Sample Insights

- The Space Race saw dramatic shifts in dominance — from the USSR's early lead through the Cold War era, to the rise of organisations like **CASC** and **SpaceX** in more recent decades.
- Launch costs vary enormously between organisations, reflecting differences in rocket technology and reusability.
- Certain months show consistently higher launch activity, hinting at scheduling and weather-related patterns.

---

## 📝 License

The code in this repository (notebooks and analysis) is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

> **Note:** The MIT License applies to the code only. The dataset (`mission_launches.csv`) was scraped from a third-party source and is included here for educational/analysis purposes — it is not covered by this repository's license. Please check [nextspaceflight.com](https://nextspaceflight.com/launches/past/?page=1) for their own terms if you intend to reuse the data itself.

## 🙌 Acknowledgements

Dataset sourced from [nextspaceflight.com](https://nextspaceflight.com/launches/past/?page=1).
