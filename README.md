# flipkart_data-SQL-analytics
# 🛒 E-Commerce Data Analysis (SQL + Python)

## 📌 Overview
This project analyzes an e-commerce dataset to uncover insights related to:
- Sales performance
- Discounts and demand
- Product ratings and reviews
- Logistics and delivery impact
- Return policies
- Brand and category performance

The analysis is performed using **SQL (via Jupyter Notebook)** and **Python (pandas)**.

---

## 🗂️ Database Schema

The project uses the following tables:

- **products** → product details (name, category, brand, etc.)
- **orders** → sales data (units sold, price, discount, stock, listing date)
- **reviews** → ratings and review counts
- **logistics** → delivery-related data
- **returns** → return policies
- **sellers** → seller info
- **payments** → payment methods

---

## 🔍 Key Business Questions & Insights

### 📈 Sales & Revenue
- Monthly revenue trends
- Top-performing brands by revenue and units sold
- Impact of discounts on sales

---

### 💸 Discounts Analysis
- Do higher discounts lead to higher sales?
- Identifying products with high discounts but low sales
- Discount vs demand relationship

---

### ⭐ Ratings & Reviews
- Relationship between rating and units sold
- Do products with more reviews sell more?
- High rating but low sales → potential visibility issue
- Low rating but high sales → risky products

---

### 🚚 Logistics & Delivery
- Does delivery time affect sales?
- Fast vs slow delivery performance
- City-wise delivery performance

---

### 🔁 Returns Analysis
- Do returnable products sell more?
- Relationship between return policy and sales
- Category-wise return policies

---

### 🏷️ Brand Performance
- Top brands by revenue
- Brands with highest ratings
- Underperforming brands despite high ratings

---

### ⏳ Product Lifecycle
- Performance of new vs old products
- Product listing trends over time
- Do older products get more sales and reviews?

---

## 🧠 Key Learnings

- **Correlation ≠ Causation**  
  (e.g., discounts may not directly cause higher sales)

- Aggregation must be done carefully  
  (product-level vs order-level analysis)

- Business insights require **relative comparison**, not fixed thresholds

- Data modeling decisions (like `listing_date` in orders) affect analysis accuracy

---

## 🛠️ Tech Stack

- **SQL** (MySQL / SQLite via SQLAlchemy)
- **Python (Jupyter Notebook)**
- **pandas**

---

## 📊 Example Insight

> Returnable products showed only a minimal increase in sales, indicating that return policy alone is not a strong driver of demand.

---

## 🚀 Future Improvements

- Build a **dashboard (Power BI / Tableau / Plotly)**
- Add **regression models** for demand prediction
- Create a **product health score**
- Perform **cohort and lifecycle analysis**

---

## 📁 How to Run

1. Open Jupyter Notebook
2. Connect to your database using SQLAlchemy
3. Run SQL queries using:
   ```python
   pd.read_sql(query, con=engine)
