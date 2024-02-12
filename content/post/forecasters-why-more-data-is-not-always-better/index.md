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

```

* **ARIMA (Autoregressive Integrated Moving Average)** Analyze time series data, capturing trends, seasonality, and autocorrelation for nuanced forecasts. Sample Python code below:

```

```

**Incorporating External Signals** Move beyond internal sales figures. Integrate factors like:

\- Market Intelligence

\- Competitor activities

\- Social media sentiment analysis

**Rigorous Evaluation** Quantify forecast accuracy using measures like Mean Absolute Error (MAE) and Mean Squared Error (MSE). This facilitates the comparison of model alternatives.

```

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