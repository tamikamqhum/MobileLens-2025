# MobileLens-2025: Smartphone Pricing & Specification Insight

![Phone Image](inputs/phone_image.png)

## Overview
MobileLens 2025 is a data-driven exploration of smartphone pricing and hardware specifications for devices released in 2025. This project analyses trends across major brands, compare specifications such as RAM, storage, battery, camera quality and evaluates how these variables influence smartphone prices. 
The final deliverable include exploratory data analysis (EDA), price-prediction in sights and an interactive Streamlit dashboard. 

## Motivation 
The smartphone market evolves rapidly, with frequent releases and large variations in specifications and pricing. Consumers, analysts and reviwers often struggle to understand the relationship between hardware features and price. 

This project aims to: 
- Identify the key drivers of smartphones in 2025
- Compare brand strategies and specifications
- Provide insights for consumers and analysts
- Buils a reproducible analytical workflow and dashboard 

## Dataset Description 
Dataset File: `mobile_prices_2025.csv`

The datset includes smartphone models released in 2025 and contains:

| Column | Description |
|--------|-------------|
| brand | Smartphone manufacturer |
| model | Model name |
| price_usd | Price of the device in USD |
| ram_gb | Device RAM in GB |
| storage_gb | Internal storage in GB |
| camera_mp | Camera resolution in megapixels |
| battery_mah | Battery capacity |
| display_size_inch | Display size in inches |
| charging_watt | Charging speed |
| 5g_support | Whether the phone supports 5G |
| os | Operating system |
| processor | Processor / chipset |
| rating | User/expert rating |
| release_month | Month of release |
| year | Release year (2025) |

## Tools & Technologies Used
- **Python**  
- **Pandas**, **NumPy**  
- **Matplotlib**, **Plotly**, **Seaborn**  
- **Scikit-Learn**   
- **Jupyter Notebook**  
- **Streamlit**  
- **Git / GitHub**

## Methodology 
1. **Data Preparation**
- Load Dataset
- Handle missing values 
- Clean and standardise variables 

2. **Exploratory Data Analysis**
- Price trends by brand
- Spec distributions
- Correlations between specs and price 
- Comparisons of OS, processors and release months

3. **Feature Engineering**
- Price-to-performance metrics 
- Smartphone tier classification 

4. **Modeling**
- Regression models to predict price 
- Feature importance evaluation

5. **Dashboard Development**
- Streamlit for dynamic exploration 
- Interactive filters and comparasons

## Hypothesis & Validation
### **Hypothesis 1: Devices with higher RAM and storage cost significantly more.**  
**Validation:**  
- Correlation analysis (`ram_gb`, `storage_gb` vs `price_usd`)  
- Price vs RAM/Storage regression plots  
- Regression model coefficients  

### **Hypothesis 2: Premium brands (Apple, Samsung, Google) charge more for similar specifications than others.**  
**Validation:**  
- Compute price-per-performance metric  
- Compare price distributions by brand  
- Visualise equal-spec comparisons  

---

### **Hypothesis 3: Higher camera resolution and battery capacity correlate with higher ratings.**  
**Validation:**  
- Correlation between `camera_mp`, `battery_mah`, and `rating`  
- Scatter plots with trend lines  
- Group analysis by device tier  

---

### **Hypothesis 4: Mid-range phones tend to offer higher charging wattage than budget or flagship models.**  
**Validation:**  
- Categorizs devices by price (budget/mid-range/flagship)  
- Compare average charging wattage  
- Boxplots of `charging_watt` by price tier  

---

### **Hypothesis 5: Display size has a moderate but positive effect on pricing.**  
**Validation:**  
- Regression of price vs display size  
- Examine R² and p-values  
- Compare display size across price tiers  


## Key Findings 
Examples of expected findings:
- Most influential specs on price  
- Brand-specific pricing trends  
- Best value-for-money models  
- Feature correlations (camera, RAM, battery, etc.)
