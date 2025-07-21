# 📦 Customer Churn Dataset (Big Basket Simulation)

This dataset simulates customer, subscription, transaction, and churn behavior for a subscription-based e-commerce platform, inspired by Big Basket. It can be used for churn prediction, customer segmentation, cohort analysis, and end-to-end analytics pipelines.

---

## 🧾 Files Included

| File Name        | Description                                                                 |
|------------------|-----------------------------------------------------------------------------|
| `Customers.csv`   | Contains customer profile info like customer ID, name, location, age, etc. |
| `Subscriptions.csv`| Tracks subscription details including plan type, start/end dates, and renewal status. |
| `Transactions.csv` | Contains purchase records: order dates, categories, amount spent, and quantity. |
| `Churn.csv`       | Labels customers as churned or active, with reasons and churn dates where available. |

---

## 📊 Schema Overview

### 🧍‍♂️ Customers.csv
| Column Name      | Description              | Example             |
|------------------|--------------------------|---------------------|
| `CustomerID`     | Unique identifier         | 101                 |
| `Name`           | Customer name             | Arjun Verma         |
| `Age`            | Age of the customer       | 35                  |
| `Location`       | City/Region               | Bengaluru           |
| `SignupDate`     | Date of account creation  | 2019-06-12          |

---

### 📄 Subscriptions.csv
| Column Name         | Description                          | Example       |
|---------------------|--------------------------------------|---------------|
| `CustomerID`        | Foreign key to Customers.csv         | 101           |
| `PlanType`          | Plan name/type                       | Premium       |
| `StartDate`         | Subscription start date              | 2022-01-01    |
| `EndDate`           | Subscription end date (if any)       | 2023-01-01    |
| `IsRenewed`         | Boolean: 1 for renewed, 0 otherwise   | 0             |

---

### 💸 Transactions.csv
| Column Name        | Description                          | Example       |
|--------------------|--------------------------------------|---------------|
| `TransactionID`    | Unique ID per transaction            | T1001         |
| `CustomerID`       | Foreign key to Customers.csv         | 101           |
| `OrderDate`        | Date of transaction                  | 2022-10-15    |
| `Category`         | Product category                     | Groceries     |
| `AmountSpent`      | Total spend in INR                   | 1548.75       |
| `Quantity`         | Items purchased                      | 5             |

---

### 📉 Churn.csv
| Column Name      | Description                            | Example       |
|------------------|----------------------------------------|---------------|
| `CustomerID`     | Foreign key to Customers.csv           | 101           |
| `Churned`        | 1 if churned, 0 otherwise              | 1             |
| `ChurnReason`    | Reason for churn (if available)        | Poor Service  |
| `ChurnDate`      | Date customer churned (if applicable)  | 2023-03-20    |

---

## 🔍 Use Cases

This dataset is suitable for:
- Churn prediction using classification models.
- Customer segmentation via clustering or cohort analysis.
- Retention and renewal analysis.
- Subscription plan performance tracking.
- Dashboard development using Power BI / Tableau.

---


