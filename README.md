# Exoplanet Data Analysis & Interactive Dashboard  
**NASA Exoplanet Archive — Python · Power BI**

This project explores the properties, discovery methods, and temporal trends of confirmed exoplanets from the **NASA Exoplanet Archive**, combining Python-based data cleaning/analysis with an interactive Power BI dashboard designed for clear visual communication and exploratory analysis.

The goal is to demonstrate a complete, end-to-end data workflow:
- dataset acquisition
- cleaning & preprocessing (Python + pandas)
- exploratory data analysis (EDA)
- interactive visualization (Power BI)
- insight extraction and scientific interpretation

---

## Dashboard Preview

![Power BI Dashboard](exoplanet_dashboard.pdf)

## Data Sources

- **Raw data** (not included):  
  NASA Exoplanet Archive – Planetary Systems (PS) Table  
  https://exoplanetarchive.ipac.caltech.edu/cgi-bin/TblView/nph-tblView?app=ExoTbls&config=PS

- **Processed data** (included):  
  `data/exoplanets_clean.csv`  
  Obtained via ETL steps described in the notebook.

## Project Structure
The repository is organized into the following directories:

├── data/  
│   └── exoplanets_clean.csv          # Cleaned dataset used for analysis  
│  
├── exoplanet_analysis.ipynb      # Python EDA + preprocessing  
│  
├── exoplanets_dashboard.pbix     # Interactive dashboard (Power BI Desktop)  
│  
├── powerbi_dashboard.pdf        # Dashboard pdf image 
│  
└── README.md

## Analyses Included

### **1. Exoplanet Discoveries per Year**
A line chart illustrating how the number of exoplanets discovered each year has evolved.

### **2. Discovery Methods Breakdown**
A bar chart comparing the prevalence of different detection techniques such as Transit, Radial Velocity, Imaging, and others.

### **3. Average System Distance per Year**
A time-trend visualization showing how the mean distance of discovered exoplanetary systems changes across discovery years.

### **4. Orbital Period Distribution**
A line-type histogram comparing orbital period distributions across discovery methods, paired with a dedicated orbital-period slicer for adaptive range selection.

## Tools Used

### **Python**
- pandas  
- numpy  
- matplotlib  

Used for:
- dataset acquisition  
- data cleaning & processing  
- handling missing values  
- exploratory data analysis (EDA)  
- generating initial scientific plots  

### **Power BI**
Used to build the interactive dashboard through:
- KPI cards  
- line & bar charts  
- categorical and numeric slicers (year, method, period range)  
- custom binning for orbital periods  
- controlled visual interactions  
- cross-filtering and dynamic exploration

## How to Run the Project

### **1. Clone the repository**
```bash
git clone https://github.com/AlessioLapponi/exoplanet_data_analysis.git
```
### **2. Run the Python notebook**
```bash
exoplanet_analysis.ipynb
```

### **3. Open the Power BI dashboard**
```bash
exoplanet_dashboard.pbix
```

# **Insights & Observations**

- The number of confirmed exoplanets increases sharply after major space missions such as *Kepler*, launched in 2009 and retired in 2018, demonstrating the impact of dedicated observatories. After this mission, the number of observable exoplanets seems almost saturated, at least before another dedicated probe is launched.
- Average system distances can fluctuate year-to-year, reflecting changes in telescope sensitivity and survey strategies. However, overall a positive trend between distances and years can be observed. This indicates how the space exploration can go deep as the years pass. A further analysis of this trend, using machine learning methods, will follow to predict the future of space observation.
- The Transit method dominates modern exoplanet detection due to large-scale photometric surveys and high cadence monitoring.
- Orbital periods show a strong observational bias: short-period planets are far more frequently detected across all methods. The transit method shows a particular success in the observation of short-period planets while, for longer period planets, the Radial Velocity method is way more effective.
- Further quantitative analysis will follow very soon.


## Author

**Alessio Lapponi**  
Applied Physicist | Soon PhD in Cosmology, Space Science and Space Technology | Numerical Modelling | Data Analysis  
[LinkedIn](https://www.linkedin.com/in/alessio-lapponi-297b58247)



