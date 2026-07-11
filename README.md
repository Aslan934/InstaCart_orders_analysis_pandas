# Instacart Orders: Data Cleaning and Exploratory Data Analysis

## 📌 Project Overview

This project explores customer shopping behavior using an Instacart grocery orders dataset. The main goal is to apply **data preprocessing, cleaning, and exploratory data analysis (EDA)** techniques using **Python and pandas**.

The analysis focuses on understanding:

* When customers place grocery orders
* How frequently customers shop
* How many products customers typically purchase
* Which products are ordered most frequently
* Customer and product reorder behavior
* Which products are most commonly added to carts first

---

## 🛠️ Technologies Used

* Python
* pandas
* Matplotlib
* Jupyter Notebook / Google Colab

---

## 📂 Dataset

The project uses five related datasets.

### `instacart_orders.csv`

Each row represents an order placed through Instacart.

| Column                   | Description                                        |
| ------------------------ | -------------------------------------------------- |
| `order_id`               | Unique identifier for each order                   |
| `user_id`                | Unique identifier for each customer                |
| `order_number`           | Number of times the customer has placed an order   |
| `order_dow`              | Day of the week when the order was placed          |
| `order_hour_of_day`      | Hour of the day when the order was placed          |
| `days_since_prior_order` | Number of days since the customer's previous order |

### `products.csv`

Each row represents a unique product.

| Column          | Description                           |
| --------------- | ------------------------------------- |
| `product_id`    | Unique identifier for each product    |
| `product_name`  | Name of the product                   |
| `aisle_id`      | Identifier for the grocery aisle      |
| `department_id` | Identifier for the grocery department |

### `order_products.csv`

Each row represents a product included in an order.

| Column              | Description                                                      |
| ------------------- | ---------------------------------------------------------------- |
| `order_id`          | Unique identifier for each order                                 |
| `product_id`        | Unique identifier for each product                               |
| `add_to_cart_order` | Order in which the product was added to the cart                 |
| `reordered`         | `0` if the product had not been ordered before and `1` if it had |

### `aisles.csv`

| Column     | Description                      |
| ---------- | -------------------------------- |
| `aisle_id` | Unique identifier for each aisle |
| `aisle`    | Name of the aisle                |

### `departments.csv`

| Column          | Description                           |
| --------------- | ------------------------------------- |
| `department_id` | Unique identifier for each department |
| `department`    | Name of the department                |

---

## 🧹 Data Preprocessing

The preprocessing stage includes:

* Inspecting the structure and contents of all five datasets
* Correcting data types where necessary
* Identifying and handling missing values
* Detecting and removing duplicate records
* Validating important numerical ranges
* Preparing the datasets for exploratory analysis

Special attention is given to understanding the possible causes of missing and duplicate values and selecting appropriate methods for handling them.

---

## 📊 Exploratory Data Analysis

### A. Order Patterns

The analysis investigates:

* Whether `order_hour_of_day` contains valid values from `0` to `23`
* Whether `order_dow` contains valid values from `0` to `6`
* The number of orders placed during each hour of the day
* The distribution of orders across days of the week
* The number of days customers wait before placing their next order

---

### B. Customer and Product Analysis

The project also explores:

* Differences in shopping-hour distributions between Wednesdays and Saturdays
* The distribution of the number of orders placed by customers
* The 20 most frequently ordered products

---

### C. Advanced Analysis

Further analysis includes:

* The typical number of products purchased per order
* The distribution of order sizes
* The 20 most frequently reordered products
* The reorder proportion for each product
* The proportion of reordered products for each customer
* The 20 products most frequently added to the cart first

---

## 🔍 Key Questions

This project aims to answer questions such as:

1. What time of day do customers most frequently shop?
2. Which days of the week are the busiest?
3. How long do customers typically wait before placing another order?
4. Do shopping patterns differ between Wednesdays and Saturdays?
5. How many orders do customers typically place?
6. Which products are the most popular?
7. How many products are typically purchased in one order?
8. Which products are reordered most frequently?
9. What proportion of purchases are reorders?
10. Which products are most frequently added to the cart first?

---

## 📈 Skills Demonstrated

* Data cleaning and preprocessing
* Missing-value analysis
* Duplicate detection and removal
* Data type conversion
* Data validation
* pandas filtering and indexing
* `groupby()` and aggregation
* DataFrame merging
* Exploratory data analysis
* Data visualization with Matplotlib
* Interpretation of customer purchasing behavior

---

## 📁 Repository Structure

```text
instacart-orders-analysis/
│
├── instacart_orders_analysis.ipynb
├── README.md
└── datasets/
    ├── instacart_orders.csv
    ├── products.csv
    ├── order_products.csv
    ├── aisles.csv
    └── departments.csv
```

> **Note:** Large dataset files may be excluded from the repository depending on GitHub file-size limitations.

---

## 🚀 How to Run the Project

1. Clone this repository.
2. Open the Jupyter Notebook locally or in Google Colab.
3. Make sure the required dataset files are available in the expected directory.
4. Install the required Python libraries if necessary.
5. Run the notebook cells in order.

Required libraries:

```python
import pandas as pd
import matplotlib.pyplot as plt
```

---

