---
title: "Forecasters: Why More Data is Not Always Better"
date: 2024-02-12T17:04:40.119Z
draft: false
featured: false
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---
<!--StartFragment-->

Many #demand #forecasters, especially in the #retail sector, subscribe to the notion that the availability of more historical data always serves as the foundation for accurate predictions. While data plays a critical role, my experience in #datascience, #forecasting, and #supply #chain #management research building pricing and demand models over the years reveals the limitations of this **more data is better** mindset. Let's unpack how it can cloud judgment and negatively impact effective decision-making.

### The "More Data is Always Better" Trap

Let's look at an example. Say you're a footwear retailer forecasting demand for a trendy sneaker:

* **Sample Data:** 3 years of sales history

If you feed all 3 years of data into your model, it will give weight to those stockout periods and underestimate the impact of recent marketing, stockouts, and competition. You'll likely under-order, miss sales opportunities, and potentially create dissatisfied customers. Recent factors such as targeted marketing campaigns or supply chain disruptions can have significant impacts on demand patterns. Blindly incorporating all historical data into your model would distort predictions, leading to potential stockouts or excess inventory. 📉

**Issues with just using Sample Data:**

* Recent **marketing campaigns** have dramatically increased interest
* Supply chain disruptions caused **stockouts** for extended periods
* A **competitor** launched a similar product

### Strategies for Enhanced Forecasting

Let's explore a data-driven approach that incorporates a nuanced understanding of context:

**Data Segmentation & Cleaning:** Dissect sales history into distinct periods reflecting major variations in demand drivers. Eliminate anomalies or periods heavily impacted by non-recurring events.

**Time-Aware Modeling:** Consider techniques that adjust to demand trends and seasonality:

* **Weighted Regression Models:** Assign greater importance to recent "normal" demand cycles for more relevant predictions. Sample Python code below:

```
import pandas as pd
from sklearn.linear_model import LinearRegression

# Fictitious 'Trendy Kicks' Sneaker Data (monthly)
df = pd.DataFrame({
   'date': pd.date_range('2021-01-01', periods=36, freq='M'),
   'sales': [120, 115, 130, 125, ..., 750, 820, 840] 
})

# Weight recent 12 months more heavily 
weights = np.concatenate([np.ones(12), np.linspace(0.8, 1, 24)]) 

model = LinearRegression()
model.fit(df[['date']], df['sales'], sample_weight=weights)

# Forecast for the next few months...
```

* **ARIMA (Autoregressive Integrated Moving Average)** Analyze time series data, capturing trends, seasonality, and autocorrelation for nuanced forecasts. Sample Python code below:

```
from statsmodels.tsa.arima.model import ARIMA

# Prepare data, ensuring time series format
df['date'] = pd.to_datetime(df['date'])
df.set_index('date', inplace=True)

model = ARIMA(df['sales'], order=(2, 1, 1))  # Example order
model_fit = model.fit()

# Forecast and calculate accuracy
forecast = model_fit.forecast(steps=6) 
print(forecast)
```

**Incorporating External Signals** Move beyond internal sales figures. Integrate factors like:

\- Market Intelligence

\- Competitor activities

\- Social media sentiment analysis

**Rigorous Evaluation** Quantify forecast accuracy using measures like Mean Absolute Error (MAE) and Mean Squared Error (MSE). This facilitates the comparison of model alternatives.

```
from sklearn.metrics import mean_absolute_error, mean_squared_error

#  Assume 'y_true' (actual sales) and 'y_pred' (predictions) exist

mae = mean_absolute_error(y_true, y_pred)
mse = mean_squared_error(y_true, y_pred)

print("Mean Absolute Error (MAE):", mae)
print("Mean Squared Error (MSE):", mse)
```

### Key Takeaways for Forecasters

* **Context Matters:** Historical data exists within a dynamic landscape of marketing efforts, consumer behavior, and supply chain constraints.
* **Collaboration is Essential:** Partner with marketing and supply chain colleagues to gain a holistic understanding of demand and supply patterns.
* **Continuous Improvement:** Good forecasting is an iterative and evolving process. Remember, demand is dynamic and will change over time; your demand forecasting approach needs to be dynamic, too. Test diverse modeling approaches and evaluate performance to guide continued refinement.

### Conclusion

In the fast-paced retail environment, demand forecasting is both an art and a science. By moving beyond simple reliance on historical data and embracing a combination of data insights, model refinement, and contextual awareness, forecasters can equip their organizations with the foresight to make profitable, customer-centric supply chain decisions.

### How to reach out?

Always happy to discuss your forecasting accuracy needs. Reach out to me via LinkedIn.

**\#demandforecasting #datascience #supplychainmanagement #retailanalytics**

<!--EndFragment-->