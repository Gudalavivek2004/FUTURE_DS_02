# FUTURE_DS_02
Customer Retention &amp; Churn Analysis Dashboard
# Customer Retention & Churn Analysis Dashboard

This repository houses the end-to-end analytical deliverables for the **Telco Customer Retention & Churn Analysis** project. The pipeline ingests raw subscriber lifecycle ledgers, runs multi-dimensional aggregations, and surfaces critical business risk indicators via an interactive executive tracking dashboard.

## 📁 Repository Structure

The workspace is organized into the following baseline components:

*   **`Telco_Customer_Churn_Data.csv`**: The primary transactional master data sheet containing anonymized subscriber entries, demographic flags, and account metrics.
*   **`Customer_Churn_Analysis_Dashboard.pdf`**: A polished, publication-ready analytics briefing report providing deep-dives into churn drivers and lifecycle metrics.
*   **`Dashboard_Preview.png`**: A high-fidelity visual export of the monitoring panel interface for quick repository referencing.

## 📊 Core Performance Metrics

Based on the verified subscriber dataset log, our global customer portfolio breaks down into the following operational variables:

| Metric Indicator | Performance Value | Contextual Business Meaning |
| :--- | :--- | :--- |
| **Total Customers** | 7,043 | Total active and historical account rows parsed within the system register. |
| **Active Customers** | 5,174 | Volume of retained accounts with open contracts and no cancellation records. |
| **Churn Customers** | 1,869 | Sub-segment of consumers who terminated their relationship during the tracking frame. |
| **Churn Rate** | 26.54% | Percentage of gross consumer volume lost, indicating baseline market erosion risk. |
| **Avg Tenure** | 32.37 Months | The collective arithmetic mean lifespan of single accounts under contract loops. |
| **Avg Monthly Charges** | \$64.76 | Global historical average contract line-item revenue generation per customer. |

## 📊 Data Dictionary

The data schema maps transactional and behavioral flags across the following distinct keys:

*   **customerID**: System-assigned primary alphanumeric identifier tracking individual accounts uniquely.
*   **gender & SeniorCitizen**: Binary demographic categories for targeted customer subset indexing.
*   **Partner & Dependents**: Structural household context attributes evaluating account stabilization.
*   **tenure**: Integer variable detailing total continuous months a customer has maintained an active line.
*   **InternetService**: Product delivery tiers tracking network interface choices (DSL, Fiber optic, or None).
*   **Contract Loop**: Operational timeline obligations dictating service lifespans (Month-to-month, One year, Two year).
*   **PaymentMethod**: Core collection gateways preferred by end-consumers (Electronic check, Mailed check, Bank transfer, Credit card).
*   **MonthlyCharges & TotalCharges**: Float data arrays profiling monthly row revenues and cumulative lifecycle values.
*   **Churn**: Target classification flag indicating whether an account left during the calculation window.

## 🛠️ Technology Stack

The engineering and visual orchestration stack used to generate these project components includes:

*   **Data Manipulation Engine**: Python 3.10+ (utilizing vectorized Pandas loops) & Microsoft Excel.
*   **Report Compilation Framework**: HTML5 structure coupled with CSS3 Print-Media stylesheet sheets compiled down via WeasyPrint.
*   **Visualization Suite**: High-impact dashboards built utilizing custom dashboard charts, Matplotlib, and Seaborn parameters.

## ⚙️ How to Run & Requirements

### 1. Prerequisites
Ensure that a stable instance of Python 3.10 or a higher variant is running inside your development path tree.

### 2. Environment Installation
Configure your workspace libraries by executing the pip dependency installation string:
```bash
pip install pandas openpyxl weasyprint toolz matplotlib seaborn
```

### 3. Execution Execution Loop
To re-process raw profile fields, calculate active revenue run-rates, and re-export the layout files, use:
```bash
python generate_churn_dashboard.py
```
