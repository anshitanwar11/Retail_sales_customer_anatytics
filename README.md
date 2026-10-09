# Retail Sales & Customer Analytics

**End-to-End Data Analytics Project | Python | Pandas | NumPy | Matplotlib | Seaborn**

## 1. Project Overview

This project analyzes retail customer, transaction, and product data to understand purchasing behavior, evaluate product performance, compare sales channels, and identify business opportunities.

Using Python, I follow a structured analytics workflow covering data quality assessment, data cleaning, dataset integration, feature engineering, exploratory data analysis (EDA), KPI analysis, and data visualization.

The objective is to convert raw retail data into meaningful business insights that can support better-informed decisions related to product performance, customer engagement, sales planning, and return management.

## 2. Business Context

Retail businesses generate large volumes of customer and transaction data. Analyzing this information helps identify customer purchasing patterns, evaluate product performance, understand channel contribution, and monitor changes in transaction value over time.

This project combines customer information, retail transactions, and product classification data to develop a consolidated view of retail performance. The analysis focuses on understanding where transaction value is concentrated, how different products and channels perform, and which areas may require further investigation.

## 3. Business Problem

The business needs a structured approach to analyze historical retail data and identify opportunities for improvement.

The analysis addresses the following questions:

- Which product categories and sub-categories contribute the most to transaction value?
- Which store or sales channel performs best?
- How do customers differ in their contribution to transaction value?
- What patterns can be observed in monthly and yearly performance?
- How significant are negative-quantity transactions?
- What opportunities can be identified through customer, product, and channel analysis?

## 4. Project Objectives

- Assess the quality, structure, and consistency of the available datasets.
- Identify missing values, duplicate records, and potential data issues.
- Clean and standardize relevant data fields.
- Integrate customer, transaction, and product information.
- Analyze retail performance using business KPIs.
- Evaluate product category and sub-category contribution.
- Compare transaction value across store channels.
- Understand customer purchasing behavior and customer-level contribution.
- Examine time-based transaction patterns.
- Investigate negative-quantity transactions and their impact on transaction value.
- Develop evidence-based insights and practical recommendations.

## 5. Dataset Overview

The project uses three related datasets.

| Dataset | Description |
|---|---|
| Customer | Customer identifiers, date of birth, gender, and city codes |
| Transactions | Transaction identifiers, customer identifiers, dates, product codes, quantity, rate, tax, transaction amount, and store type |
| Product Information | Product category and sub-category codes and descriptions |

### Data Integration

The customer dataset is joined to transaction records using customer identifiers. Product information is then integrated using product category and sub-category codes.

The resulting analytical dataset supports combined analysis of transaction performance, customer behavior, and product contribution.

The original transaction dataset contained 23,053 rows. After removing 13 exact duplicate records, 23,040 rows remained for subsequent analysis. The customer dataset contained 5,647 rows, while the product information dataset contained 23 rows.

## 6. Tools and Technologies

- **Python:** Analytical programming and data processing.
- **Pandas:** Data cleaning, integration, aggregation, and analysis.
- **NumPy:** Numerical operations and feature engineering.
- **Matplotlib:** Data visualization.
- **Seaborn:** Statistical and comparative visualizations.
- **Jupyter Notebook:** Interactive analysis and documentation.
- **Excel:** Source data inspection.
- **GitHub:** Project documentation and portfolio presentation.

## 7. Analytical Workflow

The project follows an end-to-end data analytics process.

### 7.1 Data Understanding
- Loaded and inspected all three datasets.
- Examined dataset dimensions, column names, data types, and sample records.
- Reviewed the structure and business relevance of the available fields.

### 7.2 Data Quality Assessment
- Evaluated missing values and duplicate records.
- Standardized date fields and reviewed numerical data.
- Investigated potential data inconsistencies.
- Examined negative-quantity transactions separately rather than automatically treating them as invalid records.

### 7.3 Data Cleaning and Integration
- Removed exact duplicate records from the transaction dataset.
- Prepared date and numerical fields for analysis.
- Integrated customer information with transaction records.
- Added product category and sub-category descriptions.
- Validated the resulting master dataset.

### 7.4 Feature Engineering
- Extracted year, month, month name, and quarter from transaction dates.
- Derived customer age at the transaction date, subject to data validation.
- Classified records into sale and return indicators using transaction quantity.

### 7.5 Exploratory Data Analysis
- Examined transaction values and quantities.
- Compared product categories and sub-categories.
- Evaluated store/channel performance.
- Analyzed customer-level contribution and selected demographic characteristics.
- Investigated transaction patterns across time.

### 7.6 Business KPI Analysis
- Summarized transaction value and quantity.
- Evaluated unique transaction and customer counts.
- Compared product and channel contribution.
- Examined gross sales value, return-related value, and net transaction value.
- Analyzed monthly and yearly transaction-value trends.

### 7.7 Business Insights
- Identified leading product categories and sub-categories.
- Compared store/channel contribution.
- Evaluated customer and transaction patterns.
- Developed recommendations based on the findings and limitations of the data.

## 8. Key Business Questions

### Sales Performance
- What is the overall transaction value?
- How does transaction value vary over time?
- Which store/channel contributes the most?

### Product Performance
- Which product categories have the highest transaction value?
- Which sub-categories perform best?
- Which product areas warrant further investigation?

### Customer Analytics
- How many unique customers are represented in the transaction data?
- Which customers contribute the most to transaction value?
- What patterns appear across customer groups?

### Returns Analysis
- How many transaction records have negative quantities?
- How does negative-quantity activity vary across categories and channels?
- How do negative transaction amounts affect the overall transaction-value calculation?

## 9. Initial Business Findings

The initial category-level and channel-level analysis indicates the following patterns:

- **Product category:** Books recorded the highest aggregate transaction value among product categories, followed by Electronics and Home and Kitchen.
- **Store/channel performance:** E-Shop recorded the highest aggregate transaction value among the store/channel types analyzed.
- **Further investigation:** Sub-category contribution, customer purchasing patterns, time-based trends, and negative-quantity transactions provide additional areas for analysis.

These are descriptive findings based on the available transaction data. Transaction value should not be interpreted as profit, and the observed patterns do not establish the causes of business performance.

The final notebook should contain the supporting tables, charts, and validated metrics for these findings.

## 10. Business Recommendations

The following areas can be considered in light of the analysis:

- **Product planning:** Review category and sub-category contribution when evaluating product assortment and inventory priorities.
- **Channel strategy:** Investigate the factors associated with higher transaction value in leading channels and assess whether successful practices can be replicated.
- **Customer engagement:** Use customer-level analysis to identify potential opportunities for retention and targeted engagement.
- **Return management:** Investigate negative-quantity records to better understand potential returns, reversals, or adjustments.
- **Sales planning:** Use historical monthly and yearly patterns to support business planning, while accounting for the limitations of the available data.

These recommendations are analytical opportunities rather than proven outcomes. Further investigation would be needed before implementing changes or estimating their financial impact.

## 11. Project Deliverables

- Data quality assessment
- Data cleaning and standardization
- Integrated retail dataset
- Feature engineering
- Exploratory data analysis
- Sales and business KPI analysis
- Product category and sub-category analysis
- Store/channel performance analysis
- Customer and demographic analysis
- Negative-quantity and return-related analysis
- Monthly and yearly trend visualizations
- Business insights and recommendations

## 12. Repository Structure

```text
retail-sales-customer-analytics/
│
├── Retail_Sales_Customer_Analytics.ipynb
├── README.md
├── requirements.txt
└── visualizations/
```

The notebook contains the analytical workflow, code, outputs, tables, and charts. The README documents the business context, methods, and findings. The optional `visualizations/` directory can contain exported charts used in project documentation.

## 13. How to Run the Project

1. Clone or download the repository.
2. Install Python and Jupyter Notebook or JupyterLab.
3. Install the dependencies listed in `requirements.txt`:

   ```bash
   pip install -r requirements.txt
   ```

4. Place the authorized source Excel files in the location expected by the notebook.
5. Open `Retail_Sales_Customer_Analytics.ipynb` in Jupyter Notebook or JupyterLab.
6. Run the notebook cells sequentially from beginning to end.

The source datasets must be available locally for the notebook to run unless the notebook has been configured to use another authorized data source.

## 14. Limitations and Data Considerations

- The analysis is based on historical data and may not represent current business conditions.
- Negative quantities are treated as indicators of potential return or reversal activity; the underlying business meaning should be verified where possible.
- Transaction value is not equivalent to profit because the dataset does not necessarily capture all costs and expenses.
- Customer demographic conclusions depend on the accuracy and reliability of the source fields.
- Descriptive patterns show associations within the available data and do not establish causation.
- Recommendations should be evaluated against additional business information before implementation.

## 15. Data Privacy and Usage

This project is intended for educational and professional portfolio purposes. Original datasets should only be redistributed when permission has been confirmed.

Where data redistribution is not authorized, the public repository should contain the notebook, documentation, and permitted visualizations without exposing restricted source data.

## 16. Conclusion

This project demonstrates an end-to-end approach to retail data analytics, from assessing raw data quality and integrating multiple datasets to evaluating product, customer, channel, and transaction performance.

It showcases practical applications of Python, data preparation, exploratory analysis, KPI development, visualization, and business interpretation.

The focus is on converting available retail data into clear, evidence-based findings and actionable opportunities for business improvement.

---

**Project Type:** Data Analytics | Retail Analytics | Customer Analytics  
**Status:** Portfolio Project
