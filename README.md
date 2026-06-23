# 🌦️ India Weather Analysis & Rainfall Prediction









> A large-scale weather analytics and rainfall prediction project built using nearly one million weather observations collected across India. The project focuses on understanding weather patterns, seasonal behavior, geographical climate differences, and rainfall prediction using Machine Learning.

---

# 📌 Business Problem

Weather forecasting plays a critical role in agriculture, transportation, disaster management, and resource planning.

Rainfall prediction is particularly challenging because it depends on multiple interacting environmental factors such as:

* Temperature
* Air Pressure
* Wind Speed
* Geographic Location
* Seasonal Variations
* Elevation

The objective of this project is to analyze historical weather observations and develop machine learning models capable of predicting rainfall patterns across different regions of India.

---

# 📂 Dataset Information

### Dataset Overview

| Attribute       | Details                     |
| --------------- | --------------------------- |
| Records         | 970,339                     |
| Features        | 15                          |
| Data Type       | Structured Weather Data     |
| Domain          | Climate & Weather Analytics |
| Problem Type    | Regression                  |
| Target Variable | Rainfall                    |

---

### Dataset Features

| Feature        | Description                 |
| -------------- | --------------------------- |
| date_of_record | Date of weather observation |
| month          | Month name                  |
| season         | Season category             |
| station_name   | Weather station name        |
| state          | Indian state                |
| district       | District name               |
| avg_temp       | Average temperature         |
| min_temp       | Minimum temperature         |
| max_temp       | Maximum temperature         |
| wind_speed     | Wind speed                  |
| air_pressure   | Atmospheric pressure        |
| elevation      | Elevation above sea level   |
| latitude       | Geographic latitude         |
| longitude      | Geographic longitude        |
| rainfall       | Rainfall amount             |

---

# 🔍 Data Quality Assessment

The dataset contained significant missing values in several weather variables.

| Feature      | Missing Values |
| ------------ | -------------- |
| min_temp     | 43,898         |
| max_temp     | 110,598        |
| wind_speed   | 274,444        |
| air_pressure | 304,664        |
| rainfall     | 257,554        |

### Handling Missing Values

Median Imputation was used because:

* Weather data contains outliers.
* Median is more robust than mean.
* Prevents skewing of temperature and rainfall distributions.

---

# 🔍 Exploratory Data Analysis (EDA)

Several exploratory analyses were performed to understand weather behavior across India.

### Key Analyses

✔ Rainfall Distribution Analysis

✔ Seasonal Rainfall Trends

✔ State-wise Weather Patterns

✔ District-wise Rainfall Variations

✔ Temperature Distribution

✔ Correlation Heatmap

✔ Geographical Climate Analysis

✔ Elevation vs Rainfall Relationship

---

# 📊 Key Findings

### 1. Rainfall is Highly Variable

Rainfall values showed significant variation across regions, indicating that location plays a major role in precipitation patterns.

### 2. Seasonal Impact is Significant

Monsoon seasons recorded substantially higher rainfall levels compared to other seasons.

### 3. Geographic Factors Matter

Latitude, longitude, and elevation demonstrated noticeable influence on weather characteristics.

### 4. Weather Variables are Interconnected

Temperature, air pressure, and wind speed collectively influence rainfall patterns rather than acting independently.

### 5. Prediction is Challenging

Rainfall exhibits strong non-linear behavior, making it difficult for simple regression models to generalize effectively.

---

# ⚙️ Data Preparation

### Feature Engineering

* Date conversion
* Month extraction
* Seasonal categorization
* Numerical feature preparation
* Categorical feature encoding

### Data Cleaning

* Missing value treatment
* Duplicate verification
* Data type correction

### Train-Test Split

* 80% Training Data
* 20% Testing Data
* Random State = 42

---

# 🤖 Machine Learning Models

Several regression approaches were explored for rainfall prediction.

### Evaluation Metrics

* MAE (Mean Absolute Error)
* MSE (Mean Squared Error)
* RMSE (Root Mean Squared Error)
* R² Score

---

# 📈 Model Performance

| Metric   | Score  |
| -------- | ------ |
| MAE      | 4.51   |
| MSE      | 195.32 |
| RMSE     | 13.98  |
| R² Score | -0.219 |

### Observations

* Training R² reached 0.986.
* Test R² dropped to -0.219.
* The model suffered from severe overfitting.
* Weather prediction remains challenging due to highly diverse climatic conditions across India.

---


# 🗂 Repository Structure

```text
india-weather-analysis-970k/
│
├── Weather_Analysis.ipynb
├── images/
│   ├── rainfall_distribution.png
│   ├── heatmap.png
│   ├── seasonal_analysis.png
│   └── statewise_rainfall.png
|   └── kerala rainfall.png
├── requirements.txt
└── README.md
```

---
## Dataset

Due to GitHub file size limitations, the dataset is not included in this repository.

Dataset Size: 970,339 Records

To run this project:

1. Download the dataset from the provided source.
2. Place the CSV file in the project root directory.
3. Run the notebook.
   

# 🚀 Getting Started

### Clone Repository

```bash
git clone https://github.com/nivedh-j/india-weather-analysis-970k.git
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Launch Notebook

```bash
jupyter notebook Weather_Analysis.ipynb
```

---

# 📦 Requirements

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
```

---

# 🔮 Future Improvements

* [ ] XGBoost Regressor
* [ ] CatBoost Regressor
* [ ] LightGBM Regressor
* [ ] Hyperparameter Tuning
* [ ] Feature Importance Analysis
* [ ] Cross Validation
* [ ] Streamlit Dashboard
* [ ] Real-Time Weather API Integration

---

# 👤 Author

**Nivedh J**

Data Analyst | Data Scientist

GitHub: https://github.com/nivedh-j

LinkedIn: https://www.linkedin.com/in/nivedhj/

---

# 📄 License

This project is licensed under the MIT License.
