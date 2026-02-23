# 🚗 Automobile Sales During Recession Periods
## Data Visualization with Matplotlib, Seaborn & Folium

An end-to-end data visualization project analyzing how XYZ Automotives' sales were impacted across six historical recession periods (1980–2020). The project produces 10 polished visualizations to communicate trends in sales, GDP, advertising, seasonality, consumer confidence, and unemployment.

---

## 📋 Project Overview

This project was built as a capstone lab for the IBM Data Visualization course. It answers 10 analytical questions using a curated set of chart types, progressing from simple line charts to interactive choropleth maps.

---

## 📁 Project Structure

```
automobile-sales-visualization/
│
├── automobile_sales_visualization.ipynb   # Full notebook with all 10 tasks
├── requirements.txt                        # Python dependencies
├── .gitignore                              # Files excluded from version control
└── README.md                              # This file
```

Output images are saved alongside the notebook when cells are run:
```
task1_1_yearly_sales.png
task1_2_ad_vs_sales.png
task1_3_vehicle_type_sales.png
task1_4_gdp_subplots.png
task1_5_seasonality_bubble.png
task1_6_scatter_confidence_price.png
task1_7_ad_pie.png
task1_8_vehicle_ad_pie.png
task1_9_unemployment_sales.png
task1_10_recession_map.html          ← Interactive Folium map
```

---

## 📊 Dataset

**Source:** IBM Skills Network  
**URL:** [automobile-sales.csv](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/d511MGfp_t00003eLym-dw/automobile-sales.csv)

| Column | Description |
|--------|-------------|
| `Date` | Month-end date of observation |
| `Recession` | 1 = recession period, 0 = normal |
| `Automobile_Sales` | Number of vehicles sold |
| `GDP` | Per capita GDP (USD) |
| `Unemployment_Rate` | Monthly unemployment rate |
| `Consumer_Confidence` | Synthetic consumer confidence index |
| `Seasonality_Weight` | Seasonal adjustment factor |
| `Price` | Average vehicle price |
| `Advertising_Expenditure` | Company ad spend |
| `Vehicle_Type` | Superminicar / Smallfamilycar / Mediumfamilycar / Executivecar / Sports |
| `Competition` | Market competition measure |
| `Month` / `Year` | Extracted from Date |

**Recession Periods Covered:**

| # | Period |
|---|--------|
| 1 | 1980 |
| 2 | 1981–1982 |
| 3 | 1991 |
| 4 | 2000–2001 |
| 5 | 2007–2009 (Financial Crisis) |
| 6 | 2020 Feb–April (COVID-19) |

---

## 📈 Visualizations & Tasks

| Task | Chart Type | Question Answered |
|------|-----------|-------------------|
| 1.1 | Line Chart (Pandas) | How do average sales fluctuate year-over-year? |
| 1.2 | Dual-axis Bar+Line | How does ad spend correlate with sales in non-recession years? |
| 1.3 | Grouped Bar (Seaborn) | How do vehicle type sales compare across recession/non-recession? |
| 1.4 | Subplots Line Charts | How did GDP vary during vs outside recessions? |
| 1.5 | Bubble Chart | How does seasonality impact monthly sales? |
| 1.6 | Scatter Plots (×2) | How do consumer confidence and price affect recession sales? |
| 1.7 | Pie Chart | What share of ad spend occurs during recessions? |
| 1.8 | Pie Chart | Which vehicle types received ad spend during recessions? |
| 1.9 | Line Plot | How does unemployment affect vehicle type sales? |
| 1.10 | Folium Choropleth | Which regions had the highest recession-period sales? |

---

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- pip

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/automobile-sales-visualization.git
cd automobile-sales-visualization

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch Jupyter
jupyter notebook automobile_sales_visualization.ipynb
```

> The notebook fetches the dataset automatically from IBM's cloud storage — no manual download needed.

---

## 📦 Dependencies

See `requirements.txt` for pinned versions. Core libraries:

- **pandas** — data manipulation and groupby aggregations
- **numpy** — numerical operations and trendline fitting
- **matplotlib** — base charting (line, scatter, pie, bubble, subplots)
- **seaborn** — statistical visualizations with theme support
- **folium** — interactive Leaflet.js maps in Python
- **requests** — HTTP data fetching

---

## 🔑 Key Insights

- Automobile sales drop sharply during all recession periods, most severely in 2008–2009
- Executive cars and sports vehicles suffer the steepest declines; superminis are most resilient
- Advertising spend falls during recessions, with remaining budget redirected toward affordable vehicle segments
- Consumer confidence has a strong positive relationship with sales — even during economic stress
- Seasonal patterns (year-end, festive periods) significantly drive monthly sales peaks

---

## 🛠 Technologies Used

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=flat)
![Seaborn](https://img.shields.io/badge/Seaborn-4c72b0?style=flat)
![Folium](https://img.shields.io/badge/Folium-77b829?style=flat)

---

## 📝 License

This project is open source and available under the [MIT License](LICENSE).
