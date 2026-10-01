# 🛒 Grocery Orders Analysis & Predictive Modeling

An end-to-end data analytics and machine learning project conducted as part of the AI & Machine Learning Training Program at Creativa Innovation Hub. This project explores transactional grocery data to uncover deep consumer behavior insights and implements a predictive AI model to forecast customer return intervals.

**Presented by:** Maha Mohamed Abdel-moniem

---

## 📌 Project Background & Objectives
In the rapidly growing e-grocery sector, delivery platforms generate massive amounts of customer data. Analyzing this transactional data helps businesses make smart, data-driven decisions to optimize inventory, improve customer retention, and drive sales growth.

### ❓ Core Business Questions Answered:
1. What are the best-selling and lowest-selling product departments?
2. How many days do customers typically wait before placing a new order?
3. Does the average shopping cart size evolve between historical orders and the last purchase?
4. Which popular products are prioritized and added first to the shopping cart?
5. What are the peak shopping hours and trends in customer loyalty throughout the day?

---

## 🛠️ Tech Stack & Libraries Used
* **Language:** Python
* **Data Wrangling:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn (Random Forest Regressor, Train-Test Split)

---

## 📊 Key Insights & Business Value

### 1. Department Sales Share (The Revenue Drivers)
* **Insight:** `Produce` and `Dairy Eggs` are the absolute giants, contributing to **over 50% of total customer orders** (Produce: 29.09%, Dairy Eggs: 16.76%).
* **Business Value:** Warehouse management must prioritize fresh restocking daily to prevent stockouts, and place high-profit margin items strategically nearby.

### 2. Time Gap Between Orders (Shopping Cycles)
* **Insight:** The distribution shows massive spikes exactly at **7 days and 30 days**, proving that customers shop on rigid weekly or monthly routines.
* **Business Value:** Marketing teams can automate smart coupon targeting to fire precisely when a customer is reaching their 7-day or 30-day cycle limit.

### 3. Add-to-Cart Priorities (Urgency Sensation)
* **Insight:** Essential items like `Banana` and `Bag of Organic Bananas` consistently maintain the lowest average position in the cart, meaning they are the very first items users add.
* **Business Value:** High-priority daily essentials should be featured directly on the app's homepage to create a frictionless checkout flow.

### 4. Peak Purchase Hours (Hourly Traffic Peak)
* **Insight:** Traffic follows a strict bell curve, heavily peaking between **10:00 AM and 4:00 PM** where customer shopping routine and reorder loyalty are at their highest.
* **Business Value:** Focus the daily advertising budget and promotional notifications during these peak daytime hours to maximize click-through rates.

---

## 🤖 Future Work: Predictive AI Model
To take this analysis a step further, a predictive machine learning model was developed:
* **Algorithm Used:** `RandomForestRegressor`
* **Features Trained on:** `order_hour_of_day`, `order_dow`
* **Target Metric:** `days_since_prior_order` (Predicting when the customer will return)
* **Model Result:** Successfully trained with a **Mean Absolute Error (MAE) of 6.92 days**. 

* **Business Impact:** This baseline model allows the grocery platform to anticipate ordering trends, optimize supply chain delivery loads, and automate personalized user re-engagement strategies.

---

## ⚙️ Installation & Usage
To view and run this project locally, make sure you have Jupyter Notebook installed and run:

```bash
# Clone the repository
git clone https://github.com

# Navigate to the project folder
cd grocery-orders-analysis

# Run the notebook
jupyter notebook analysis.ipynb
```
