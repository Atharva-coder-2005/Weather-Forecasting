#  Global Weather Trend Forecasting
### PM Accelerator Tech Assessment

---

##  About PM Accelerator
PM Accelerator is a product management training program that helps aspiring and experienced PMs accelerate their careers through real-world projects, mentorship, and community. Their mission is to **"support the PM community by providing access to resources, guidance, and opportunities to help them become their best selves."**

---

##  Project Overview
This project analyzes the **Global Weather Repository dataset** (137,413 rows, 41 features) to forecast future weather trends using data science and machine learning techniques.

---

##  Dataset
- **Source:** [Kaggle - Global Weather Repository](https://www.kaggle.com/datasets/nelgiriyewithana/global-weather-repository/code)
- **Size:** 137,413 rows × 41 columns
- **Coverage:** 211 countries, 257 cities
- **Date Range:** May 2024 – April 2026

---

##  Project Structure
weather-forecasting/

├── data/                  
├── outputs/               
├── notebook.ipynb         
├── requirements.txt       
└── README.md             

---

##  What's Covered

### 1. Data Cleaning & Preprocessing
- Removed redundant columns (duplicate unit columns)
- Engineered new features: hour, month, season, day_of_week
- Zero missing values in dataset

### 2. Exploratory Data Analysis (EDA)
- Temperature distribution by season
- Feature correlation heatmap
- Global temperature & AQI world map

### 3. Anomaly Detection
- Isolation Forest algorithm (5% contamination)
- Detected unusual weather events across the dataset

### 4. Environmental Impact Analysis
- PM2.5 vs Temperature scatter analysis
- Effect of humidity and wind on air quality

### 5. Feature Importance
- Random Forest based feature importance
- Top features: temperature, humidity, wind_kph

### 6. Climate Analysis
- Monthly temperature trends across top 10 countries
- Seasonal pattern identification

### 7. Forecasting Models
| Model | RMSE | MAE | R² |
|-------|------|-----|----|
| Prophet | 9.79 | 5.26 | -7.55 |
| XGBoost | 3.57 | 2.91 | -0.14 |
| Ensemble | 4.70 | 3.33 | -0.97 |

**Best Model: XGBoost (RMSE: 3.57°C)**

---

##  How to Run

### 1. Clone the repository
```bash
git clone https://github.com/Sanskriti-1011/Weather-forecasting.git
cd Weather-forecasting
```

### 2. Create virtual environment
```bash
python -m venv venv
venv\Scripts\activate  
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Download Dataset
Download from [Kaggle](https://www.kaggle.com/datasets/nelgiriyewithana/global-weather-repository/code) and place in `data/` folder.

### 5. Run Notebook
Open `notebook.ipynb` in VS Code or Jupyter and run all cells.

---

##  Requirements
pandas
numpy
matplotlib
seaborn
plotly
scikit-learn
prophet
xgboost
ipython
nbformat

---

##  Author
**Atharva**
PM Accelerator Tech Assessment Submission
