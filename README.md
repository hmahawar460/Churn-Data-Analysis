# Customer Churn & Subscription Analytics Dashboard

A data analytics project that explores customer churn, subscription patterns, customer lifetime value (CLTV), customer satisfaction, and cancellation reasons using Python and a Power BI-style dashboard.

## GitHub Repository Description

**Customer churn analysis dashboard exploring churn rates, subscription plans, customer value, cancellation reasons, and customer segments using Python, data analysis, and Power BI.**

## Project Overview

Customer churn occurs when customers stop using or renewing a service. Understanding churn helps businesses identify customer groups that may need better support, improved onboarding, or more suitable subscription plans.

This project analyzes an exported customer dataset and presents key metrics through a dashboard with filters and visualizations. The goal is to turn customer data into understandable findings that can support retention planning.

## Dashboard Preview

Add the dashboard screenshot to your repository, preferably inside an `images` folder, using this filename:

`Churn_Data_PowerBI_Dashboard.png`

Then uncomment the image link below:

<!-- ![Customer Churn Power BI Dashboard](images/Churn_Data_PowerBI_Dashboard.png) -->

## Key Dashboard Metrics

- Total customers
- Churned customers
- Churn rate
- Average customer lifetime value (CLTV)
- Average customer satisfaction score (CSAT)

## Analysis Questions

This project explores questions such as:

1. What percentage of customers have churned?
2. Which subscription plan has the highest observed churn rate?
3. How does churn vary by subscription type?
4. What are the most frequently recorded cancellation reasons?
5. Which states have the highest observed churn rates?
6. Does the observed churn rate differ across gender groups?
7. What are the average CLTV and monthly charges?
8. How complete are the customer satisfaction and complaint records?
9. Which data-quality or dashboard issues should be checked before making business decisions?

## Dataset

The analysis uses the provided exported customer CSV. The dataset includes customer and subscription information, plan and contract types, churn status, cancellation reasons, monthly charges, CLTV, churn score, location, gender, and selected complaint and CSAT fields.

The supplied export contains **21 customer records**. In this extract, **6 customers are marked as churned**, giving an observed churn rate of **28.6%**.

> **Important:** This is a small sample. Segment-level percentages can change substantially with only one or two additional records. Findings should be treated as exploratory, not as proof that a particular customer attribute causes churn.

## Tools & Technologies

- **Python** — data analysis
- **pandas** — data cleaning and aggregation
- **NumPy** — numerical operations
- **Matplotlib / Seaborn** — data visualization
- **Jupyter Notebook** — analysis workflow
- **Power BI dashboard** — interactive KPI and segment exploration, as represented by the project dashboard

## Repository Structure

A suggested structure for the GitHub repository:

```text
Customer-Churn-Analytics/
├── README.md
├── churn_analysis.ipynb
├── exported_churn_data.csv
└── images/
    └── Churn_Data_PowerBI_Dashboard.png
```

Adjust the filenames or folders if your repository uses a different structure. Avoid uploading customer-identifying or confidential data to a public repository.

## How to Explore the Project

1. Clone or download this repository.
2. Open `churn_analysis.ipynb` in Jupyter Notebook or Google Colab.
3. Make sure the CSV path in the notebook matches the location of `exported_churn_data.csv`.
4. Run the notebook cells in order to review the data analysis.
5. Open the dashboard image in the `images` folder to view the dashboard layout.

### Install Python Libraries

If the notebook requires these packages, install them with:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

## Preliminary Findings

Based on the supplied dataset:

- **Overall churn:** 6 of 21 customers, or **28.6%**.
- **Basic plan:** the highest observed churn rate among plan types in this sample.
- **Referral-labelled subscription group:** a high observed churn rate in this small sample.
- **Cancellation reasons:** “Switched to competitor” is the most frequently recorded reason among the available cancellation-reason entries.
- **Data completeness:** some CSAT, complaint, and cancellation fields are missing and should be considered when interpreting results.

These findings describe the provided extract only. Check group sizes and data quality before using them to make business decisions.

## Recommendations

- Investigate why the Basic plan has a higher observed churn rate.
- Review referral-source customers' onboarding and service experience.
- Capture cancellation reasons consistently.
- Improve the completeness of CSAT and complaint information.
- Validate dashboard labels, calculations, filters, and date aggregation.
- Re-evaluate the findings with a larger dataset covering multiple periods.

## Limitations

- The exported dataset contains only 21 rows.
- Some fields contain missing values.
- Currency units for CLTV and monthly charges are not specified in the export.
- The data is observational, so the analysis does not establish causation.
- Dashboard values may depend on filters or transformations that are not fully represented in the CSV.

## Future Improvements

- Analyze churn across a larger customer population and longer time period.
- Add monthly and cohort-based churn tracking.
- Improve data validation and missing-value handling.
- Add retention KPIs and drill-down analysis.
- Test whether retention actions improve churn outcomes over time.

## Conclusion

This project demonstrates how customer data can be summarized into churn KPIs and segment-level comparisons. It provides a starting point for investigating customer retention, while highlighting the need for larger samples, complete data, and validated dashboard calculations.

---

**Project:** Customer Churn & Subscription Analytics  
**Primary focus:** Customer churn, subscriptions, customer value, and retention insights
