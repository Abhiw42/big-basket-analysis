# 🛒 Big Basket Analysis Project

## 📌 Overview

This project analyzes product data from Big Basket to derive insights such as pricing trends, top-selling items, brand distributions, and discount strategies. The analysis is performed using Python libraries like `pandas`, `numpy`, `matplotlib`, and `seaborn`.

---

## 📂 Dataset

* **File Name**: `BigBasket Products.csv`
* **Rows**: \~27,555 products
* **Columns**:

  * `index`, `product`, `category`, `sub_category`, `brand`
  * `sale_price`, `market_price`, `type`, `rating`, `description`

---

## 🧾 Project Steps

### 1. **Data Loading**

* Imported CSV using `pandas`.

### 2. **Initial Inspection**

* Displayed the first 12 rows using `data.head(12)`.

### 3. **Statistical Summary**

* Used `data.describe()` to get key metrics like mean, min, max, etc.

### 4. **Data Info**

* Used `data.info()` to inspect datatypes and missing values.

### 5. **Top & Least Sold Products**

* Assumed products with highest and lowest `sale_price` as proxies for best and worst-selling products.

### 6. **Discount Calculation**

* Calculated discount = `market_price - sale_price`.

### 7. **Missing Values**

* Identified missing values in key columns like `rating`, `sale_price`, `description`, etc.

### 8. **Outlier Detection & Treatment**

* Used boxplots to detect outliers in `sale_price`, `market_price`, and `rating`.
* Replaced outliers with the column mean using IQR method.

### 9. **Visualizations**

* **Correlation Heatmap** for numerical columns.
* **Histograms** and **Boxplots** for price distribution.
* **Barplot** for top 10 brands by product count.

---

## 🧰 Libraries Used

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

---

## 📈 Key Insights

* Products like "Beard Kit" and "Brass Cookware" have extremely high sale prices.
* Many products offer no discount, while some offer significant markdowns.
* Ratings are mostly centered between 3.5 and 4.5.
* A few brands dominate the product count on Big Basket.

---

## 📎 To Run the Project

1. Ensure you have Python 3.x installed.

2. Install required libraries (if not already):

   ```bash
   pip install pandas numpy matplotlib seaborn
   ```

3. Load the `.ipynb` notebook in Google Colab or Jupyter.

4. Upload `BigBasket Products.csv` and execute all cells.

---

## 📌 Future Enhancements

* Predictive analysis for dynamic pricing.
* Clustering similar products.
* Text analysis of product descriptions.
