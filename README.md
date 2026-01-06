# **Unlocking Insights to Improve E-commerce Efficiency and Customer Satisfaction**

## Project Overview

This project simulates a real-world e-commerce analytics scenario where transactional, behavioral, and geolocation data are analyzed to generate actionable insights that support strategic decision-making across:

* Customer experience optimization
* Delivery & logistics performance
* Revenue and product strategy
* Sales funnel efficiency and lead conversion

The project combines **exploratory data analysis, statistical analysis, predictive modeling, geospatial analysis, and dashboarding** to deliver business-ready insights.

---

## Business Objectives

1. **Delivery & Logistics**

   * Measure delivery efficiency by comparing estimated vs actual delivery dates
   * Identify cities and states with frequent delivery delays

2. **Customer Satisfaction**

   * Analyze review score distributions by product category and seller
   * Quantify the impact of delivery delays on customer reviews

3. **Revenue & Product Performance**

   * Identify top-performing product categories and sellers
   * Analyze payment methods and revenue contribution

4. **Sales Funnel & Lead Conversion**

   * Predict the likelihood of MQLs converting into closed deals
   * Identify high-converting lead sources and behaviors

5. **Experimentation & Optimization**

   * Suggest A/B test opportunities at the funnel and product level

6. **Business Monitoring**

   * Build an interactive KPI dashboard using Python Dash

---

## Key Questions Answered

* What drives late deliveries, and where do they occur most?
* How strongly do delivery delays impact customer satisfaction?
* Which products and regions generate the most revenue?
* What factors increase lead conversion probability?
* Where should the business run A/B tests to improve outcomes?

---

## Dataset Description

The project uses cleaned versions of the following datasets:

| Dataset                  | Description                             |
| ------------------------ | --------------------------------------- |
| `orders_clean`           | Order lifecycle and delivery timestamps |
| `order_items_clean`      | Products and sellers per order          |
| `order_reviews_clean`    | Customer review scores                  |
| `customers_clean`        | Customer location data                  |
| `sellers_clean`          | Seller geographic information           |
| `products_clean`         | Product attributes                      |
| `product_cat_name_clean` | Product category translation            |
| `order_payments_clean`   | Payment methods and values              |
| `qualified_leads_clean`  | Marketing qualified leads               |
| `closed_leads_clean`     | Closed / won deals                      |
| `geolocation_clean`      | Latitude and longitude by ZIP prefix    |

---

## ⚙️ Tech Stack

* **Python** (Pandas, NumPy, Scikit-learn, SciPy)
* **Visualization**: Matplotlib, Seaborn, Plotly
* **Geospatial**: GeoPandas, Geopy
* **Dashboarding**: Dash, JupyterDash
* **Machine Learning**: Random Forest, Logistic Regression
* **Statistics**: Pearson Correlation, Chi-Square Test

---

## 📁 Project Structure

```text
.
├── data/
│   └── cleaned_datasets/
├── notebooks/
│   ├── 10alytics_knpwledge.ipynb
├── dashboard/
│   └── dash_app.py
├── images/
│   └── project_overview.png
├── requirements.txt
├── README.md
└── LICENSE
```

---

## 🛠️ Installation Instructions

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/GogoHarry/ecommerce-analytics.git
cd ecommerce-analytics
```

### 2️⃣ Create Virtual Environment (Optional)

```bash
python -m venv venv
source venv/bin/activate   # macOS/Linux
venv\Scripts\activate      # Windows
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Usage

### Run Analysis Notebooks

Open Jupyter Notebook and run notebooks sequentially:

```bash
jupyter notebook
```

### Launch Dashboard

```bash
python dashboard/dash_app.py
```

Or in Jupyter:

```python
app.run_server(mode="inline")
```

---

## 📊 Dashboard KPIs Tracked

* Total Revenue
* On-time Delivery Rate
* Average Review Score
* Lead Conversion Rate
* Revenue by Product Category
* Average Delivery Delay by State
* Review Score vs Delivery Delay
* Conversion Rate by Lead Origin

---

## Methodology Summary

### Delivery Analysis

* Delivery delay calculated as:

```python
actual_delivery_date - estimated_delivery_date
```

* Categorized as Early, On-time, or Late

### Customer Satisfaction

* Correlation analysis between delay and review score
* Chi-square test confirms dependency between delivery timeliness and sentiment

### Predictive Modeling

* **Delivery Delay Prediction** → Regression models
* **Review Score Prediction** → Regression models
* **Lead Conversion Prediction** → Classification models

### Geospatial Analysis

* Seller-to-customer distance calculation using geodesic distance
* Identification of delay-prone regions

---

## A/B Testing Opportunities

* Shipping speed messaging vs standard delivery
* Product page content for high-delay categories
* Lead source prioritization
* Seller logistics optimization experiments

---

## 📈 Key Findings

* Delivery delays have a **moderate negative correlation** with review scores
* Late deliveries significantly increase negative reviews
* Certain states consistently experience higher delays
* A small number of categories drive a large share of revenue
* Lead conversion strongly depends on origin and behavioral profile

---

## Business Recommendations

* Prioritize logistics improvements in high-delay regions
* Incentivize sellers with better delivery performance
* Improve delivery expectation communication
* Focus marketing spend on high-converting lead sources
* Run controlled A/B tests before large-scale changes

---

## 🧑‍🤝‍🧑 Contribution Guidelines

Contributions are welcome!

1. Fork the repository
2. Create a feature branch
3. Commit changes with clear messages
4. Submit a pull request

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 🙋‍♂️ Contact

**Author:** Gogo Harrison
**Role:** Data Analyst / Data Scientist
**Email / LinkedIn:** *(https://www.linkedin.com/in/gogo-harrison/)*

---

## ⭐ Acknowledgments

* 10alytics Knowledge Quest
* Open e-commerce datasets
* Open-source Python community

---
