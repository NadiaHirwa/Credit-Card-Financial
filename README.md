# Credit Card Financial Data Insights - 2023 Analysis

## 📁 Project Structure
```
Credit-Card-Financial/
├── data/
│   ├── raw/                    # Original dataset files
│   │   ├── credit_card.csv     # Credit card transaction data
│   │   └── customer.csv        # Customer demographic data
│   └── processed/              # Cleaned and merged datasets
│       └── Credit_Card_Financial.csv
├── notebooks/
│   ├── Data_Cleaning.ipynb     # Data preprocessing and cleaning
│   └── Data_Analysis.ipynb     # Exploratory data analysis and visualizations
├── results/                    # Generated visualizations (PNG, JPG, HTML)
│   ├── Correlation_Matrix_Heatmap.png
│   ├── Gender_Distribution_Pie_Chart.png
│   ├── Avg_Income_by_EdLevel.png
│   ├── Customers_by_Marital_Status.png
│   ├── Avg_Credit_Limit_by_Card_Type.png
│   ├── Avg_Interest_by_Card_Type.png
│   ├── Usage_Mode_vs_Total_Spend.png
│   ├── Total_Transaction_Amount_Over_Time.png
│   ├── Spending_by_Expense_Type.png
│   ├── Delinquent_Accounts_by_State.png
│   ├── Customer_Count_by_Satisfaction_Bar.png
│   ├── Customer_Job_Breakdown.png
│   └── Credit_Limit_Boxplot.png
└── docs/                       # Documentation and reports
    ├── Credit_card_Finacial_data_analysis_report.html
    ├── credit_card_financial_data_insights_slides.qmd
    ├── credit_card_financial_data_insights_slides.html
    ├── Data_Analysis.pdf
    ├── cleaning.pdf
    └── Credit_Card_Financial_Dashboard.pdf
```

## 📌 Project Overview
This project performs comprehensive analysis of customer credit card data from **2023** to uncover insights into user behavior, income distribution, credit limit usage, satisfaction levels, and demographic patterns. The analysis supports both exploratory data analysis and business intelligence dashboard creation using modern data science tools.

## 🎯 Key Objectives
- **Customer Behavior Analysis**: Understand credit card usage patterns and spending habits
- **Demographic Insights**: Analyze customer profiles by age, gender, education, and location
- **Financial Performance**: Examine credit limits, interest earned, and transaction patterns
- **Risk Assessment**: Identify delinquency patterns and customer satisfaction trends
- **Business Intelligence**: Create interactive visualizations for stakeholder presentations

## 🧼 Data Processing Pipeline

### Data Cleaning (`Data_Cleaning.ipynb`)
- **Data Loading**: Two separate datasets (credit card transactions and customer demographics)
- **Data Merging**: Combined datasets using `Client_Num` as primary key
- **Data Cleaning**: 
  - Removed null values and standardized data types
  - Cleaned categorical variables (Card_Category, Education_Level, Marital_Status)
  - Created new features for temporal analysis
  - Replaced inconsistent values for better grouping
- **Output**: Clean, merged dataset with 10,108 records and 32 variables

### Data Analysis (`Data_Analysis.ipynb`)
Comprehensive exploratory analysis covering:

#### 📊 Statistical Analysis
- **Dataset Overview**: 10,108 customers, 32 variables
- **Correlation Analysis**: Key relationships between financial variables
- **Distribution Analysis**: Skewness and kurtosis of credit limits
- **Statistical Testing**: Gender differences in credit limits

#### 📈 Key Visualizations (15+ charts)
1. **Demographics**:
   - Gender Distribution (Pie Chart)
   - Customer Distribution by Marital Status
   - Customer Occupation Breakdown
   - Average Income by Education Level

2. **Financial Metrics**:
   - Average Credit Limit by Card Type
   - Average Interest Earned by Card Type
   - Credit Limit Distribution by Gender (Boxplot)
   - Correlation Matrix Heatmap

3. **Usage Behavior**:
   - Usage Mode vs Total Spend
   - Total Transaction Amount Over Time
   - Spending by Expense Type

4. **Risk & Satisfaction**:
   - Delinquent Accounts by State
   - Customer Count by Satisfaction Level

## 🔍 Key Insights

### 💰 Financial Relationships
- **Strong Income-Spending Correlation**: 0.97 correlation between Income and Total_Trans_Amt
- **Weak Credit Limit Influence**: Only 0.17 correlation between Credit_Limit and Trans_Amt
- **Annual Fees Irrelevance**: No meaningful correlation with spending behavior

### 📊 Distribution Patterns
- **Credit Limit Distribution**: Right-skewed (skewness ≈ 1.67) with heavy tails (kurtosis ≈ 1.80)
- **Income Inequality**: Mean $56,976 vs Median $44,768, indicating income skewness
- **Gender Differences**: Statistically significant difference in credit limits between genders

### 🎯 Customer Segments
- **Card Types**: 91.16% Blue cards, 6.32% Silver, 1.86% Gold, 0.66% Platinum
- **Demographics**: 58.17% Female, 50.73% Married, 40.90% Graduates
- **Occupations**: 25.47% Self-Employed, 18.81% Business, 15.62% Blue-collar

## 💡 Data-Driven Recommendations

### 1. Income-First Strategy
- Use income data (0.97 correlation with spending) as primary business driver
- Target high-income customers for premium products
- Set credit limits based on income, not traditional scoring

### 2. Fee Structure Redesign
- Eliminate annual fees (no correlation with spending behavior)
- Implement usage-based pricing or value-added services
- Focus on transaction fees and rewards programs

### 3. Risk Management Optimization
- Set conservative credit limits (weak correlation with spending)
- Implement outlier monitoring for unusual credit limits
- Use income and spending patterns for limit decisions

### 4. Customer Segmentation
- Develop tiered products based on natural distribution
- Create targeted marketing campaigns for different segments
- Focus on the majority with lower limits while nurturing premium customers

## ✅ Deliverables

### 📊 Analysis Reports
- **HTML Report**: `docs/Credit_card_Finacial_data_analysis_report.html` (47MB comprehensive report)
- **PDF Documentation**: Data analysis and cleaning reports
- **Jupyter Notebooks**: Clean, modular code with reproducible analysis

### 🎯 Presentation Materials
- **Quarto Presentation**: `docs/credit_card_financial_data_insights_slides.qmd`
- **Interactive Slides**: Professional presentation with embedded visualizations
- **Business Recommendations**: Strategic insights and implementation plans

### 📈 Visualization Assets
- **15+ Interactive Charts**: PNG, JPG, HTML formats
- **Statistical Visualizations**: Correlation matrices, distribution plots
- **Business Intelligence**: Customer segmentation and behavior analysis

### 🔗 Interactive Dashboard
- **Looker Studio Dashboard**: Live interactive dashboard for stakeholder access
- **Real-time Analytics**: Dynamic filtering and exploration capabilities

## 🛠️ Technologies Used
- **Python**: Primary programming language
- **Pandas & NumPy**: Data manipulation and analysis
- **Plotly**: Interactive visualizations
- **Seaborn & Matplotlib**: Statistical plotting
- **Jupyter Notebooks**: Development environment
- **Quarto**: Professional presentation creation
- **Looker Studio**: Interactive dashboard creation
- **Scipy**: Statistical testing and analysis

## 📊 Dataset Characteristics
- **Size**: 10,108 customer records with 32 variables
- **Time Period**: 2023 data only (temporal limitation)
- **Key Variables**: 
  - Customer demographics (age, gender, education, marital status)
  - Financial metrics (income, credit limits, transaction amounts)
  - Behavioral data (card usage, satisfaction scores, delinquency)

## 🔗 Dashboard Access
**Live Looker Studio Dashboard**: [Credit Card Financial Dashboard](https://lookerstudio.google.com/u/0/reporting/d29f32ef-cbc1-4b61-91a4-120c2888e857/page/p_tgd5vudltd)

## 📈 Success Metrics
- Revenue per customer by income segment
- Fee acceptance rates across different customer segments
- Spending velocity (transactions per month) by income level
- Customer lifetime value based on income and spending patterns
- Credit limit utilization rates vs. actual spending capacity

## ⚠️ Limitations & Considerations
- **Temporal Constraint**: 2023-only data (no multi-year trends)
- **Seasonal Effects**: Cannot capture year-over-year patterns
- **Economic Context**: Limited to 2023 economic conditions
- **Sample Representation**: May not represent all demographics equally

## 🚀 Future Research Directions
- **Longitudinal Analysis**: Multi-year data collection (2022-2024+)
- **Seasonal Trend Analysis**: Year-over-year pattern identification
- **Economic Impact Studies**: Cross-temporal economic factor analysis
- **Machine Learning Models**: Advanced predictive analytics
- **Real-time Monitoring**: Dynamic outlier detection systems

---

**Project Status**: ✅ Complete  
**Last Updated**: June 2025  
**Data Period**: 2023 Only  
**Authors**: Nadia Iradukunda Hirwa
