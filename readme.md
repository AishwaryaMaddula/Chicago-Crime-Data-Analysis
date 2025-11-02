# 🏙️ Chicago Crime Analysis (2014–2023)

### **Project Overview**
This project explores crime trends in Chicago from 2014 to 2023 using a combination of **Python (for data cleaning and preprocessing)** and **Tableau (for visualization and dashboarding)**.  
The goal was to analyze the temporal, spatial, and categorical patterns of crime to identify insights that can assist **law enforcement, policymakers, and community organizations** in improving public safety and decision-making.

---

### **Objectives**
- Examine yearly, seasonal, and daily crime patterns in Chicago  
- Analyze the most common crime types and their locations  
- Explore **arrest vs non-arrest** trends and domestic crime distribution  
- Conduct **homicide-specific analysis** to understand community-level hotspots  
- Build an interactive **Tableau dashboard** for visual storytelling and insight discovery  

---

### **Data Source**
The dataset was obtained from the official **[Chicago Data Portal](https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-Present/ijzp-q8t2)**, which provides open-access public safety data.

- **Original dataset size:** 8.21 million records (2001–2024)  
- **Final filtered dataset:** 2.48 million rows (2014–2023) across 10 columns  
- **File size after cleaning:** ~266 MB  
- **Attributes retained:** Date, Primary Type, Description, Location Description, Arrest, Domestic, Community Area, Latitude, Longitude, Year  

---

### 🧰 **Technologies Used**

<p align="left">
  <img src="https://cdn.worldvectorlogo.com/logos/tableau-software.svg" width="40" height="40" alt="Tableau"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" width="40" height="40" alt="Python"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pandas/pandas-original.svg" width="40" height="40" alt="Pandas"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/numpy/numpy-original.svg" width="40" height="40" alt="NumPy"/>
  <img src="https://raw.githubusercontent.com/scipy/scipy/main/doc/source/_static/logo.svg" width="40" height="40" alt="SciPy"/>
  <img src="https://upload.wikimedia.org/wikipedia/commons/8/84/Matplotlib_icon.svg" width="40" height="40" alt="Matplotlib"/>
  <img src="https://seaborn.pydata.org/_images/logo-tall-lightbg.svg" width="40" height="40" alt="Seaborn"/>
  
</p>

- **Tableau** – Interactive dashboard and spatial visualization
- **Python** – Data preprocessing, cleaning, and export  
- **Pandas / NumPy** – Data manipulation and filtering  
- **SciPy** – Statistical summarization and data validation  
- **Matplotlib / Seaborn** – Exploratory data visualizations

---

### **Data Preparation in Python**
Steps performed in Jupyter Notebook before Tableau import:

1. Loaded the raw CSV (8.2M rows, 22 columns)
2. Dropped unused columns: `ID`, `IUCR`, `Beat`, `District`, `Ward`, `Block`, etc.  
3. Filtered dataset to **2014–2023** for contemporary analysis  
4. Removed nulls from critical columns like `Latitude`, `Longitude`, `Location Description`  
5. Exported cleaned dataset (`crimes_2014to2023.csv`, ~2.48M records) for Tableau visualization  

---

### **Tableau Dashboard**
<p align="center">
  <img src="Tableau-Analysis/TableauDashboard.png" width="800" alt="Chicago Crime Dashboard Screenshot"/>
</p>

#### **Dashboard Sections**
- **Dataset Overview:** Summary of crime totals, arrests, property vs violent crimes  
- **Crime Type Analysis:** Top 10 crime categories and domestic crime proportions  
- **Temporal Trends:** Yearly, seasonal, and time-of-day analyses  
- **Spatial Patterns:** Crimes by location type (street, residence, apartment, etc.)  
- **Homicide Analysis:** Geographic heatmap of homicides by community area and arrest rate trends  

---

### **Key Insights**

#### 🔍 **Overall Crime Patterns**
- **Theft** remains the most frequent crime (over 550K cases) followed by **Battery** and **Criminal Damage**  
- Overall crimes dropped notably during **COVID-19 (2020–2021)** but have rebounded since  
- **Arrests occur in only ~19% of cases**, indicating most crimes go unresolved  

#### 🕓 **Temporal and Spatial Trends**
- Most crimes occur **at night (46%)** and during **summer and fall months**  
- **Weekends** show a slight uptick in criminal activity  
- The **Street** is the most common crime location (32%), followed by **Residences** and **Apartments**

#### 🔫 **Homicide Analysis**
- **6,473 homicides** were recorded between 2014–2023  
- The **Austin community area** accounted for nearly **10%** of all homicides  
- **Most homicides occur in residences or apartments**, not public spaces  
- Arrest rates for homicide cases remain lower than ideal, showing investigative challenges

---

### **References**
- [Chicago Data Portal – Crimes 2001 to Present](https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-Present/ijzp-q8t2)  
- [Tableau Custom Shapes & Word Cloud Guides](https://www.tableau.com/drive/custom-shapes)  
- [Tableau Community Discussions](https://community.tableau.com/)

---
### 📄 Project Report
The detailed analysis, including all visuals and statistical summaries, can be viewed below:  
📘 [Open Full Report (Analysis.pdf)](https://github.com/AishwaryaMaddula/Chicago-Crime-Data-Analysis/blob/6844dc86e5634c53f63a6ddc2bb84b643793b0fa/Tableau-Analysis/Analysis.pdf)
