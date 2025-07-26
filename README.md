# METAR Data Forecasting Using Facebook Prophet

Forecasting airport visibility using univariate and multivariate time-series modeling with Facebook Prophet, ARIMA, and ARIMAX.

Paper - “[Visibility Forecasting in Meteorological Aerodrome Report using Facebook Prophet](https://ijsrem.com/download/visibility-forecasting-in-meteorological-aerodrome-report-using-facebook-prophet/)”
International Journal of Scientific Research in Engineering and Management, Volume: 07, Issue: 06 | June 2023

📌 ### **Problem Statement**  

Meteorological Aerodrome Reports (METARs) are crucial weather updates used in aviation. Among the parameters they report, visibility is particularly critical for safe takeoffs and landings.
Traditional meteorological forecasting is often complex and time-consuming. This project proposes a data-driven and efficient approach to visibility prediction using time-series models, specifically:
- **Facebook Prophet** (univariate and multivariate)
- **ARIMA**
- **ARIMAX**

🧪 **Dataset Details**
- **Source:** [Kaggle METAR Dataset - KNYC](https://www.kaggle.com/datasets/cabaki/knycmetars2016)
- **Location:** New York Central Park (KNYC)
- **Records:** ~8,787 hourly observations (2015–2017)
- **Target:** Visibility (in miles)
- **Features:** Temperature, Windchill, Heat Index, Humidity, Pressure, Dew Point, Wind Speed, etc.

📈 **Forecasting Methodology**  

✅ **Data Preprocessing**
- Imputation of missing values using mean
- Conversion of timestamp to datetime format
- Stationarity tested via **Augmented Dickey-Fuller Test** (ADF)

🔍 **Exploratory Data Analysis**
- Time series decomposition to detect trends and seasonality
- Correlation matrix to select multivariate features

🧾**Project Highlights**
| Forecasting Type       | Models Used             | Features Included        | Best RMSE      |
| ---------------------- | ------------------------| -------------------------| ---------------|
| **Univariate Forecast**| Facebook Prophet, ARIMA | Visibility (target only) | 3.26 (FB Prop) |
| **Multivariate Forecast** | Facebook Prophet, ARIMAX | Visibility + Temp, Windchill, Pressure, etc. | **2.48 (FB Prophet)** |

**References**
- [Facebook Prophet Docs](https://facebook.github.io/prophet/)
- ARIMA and ARIMAX theory from [StatsModels](https://www.statsmodels.org/stable/index.html)
  
