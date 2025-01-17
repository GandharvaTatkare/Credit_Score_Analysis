# Credit Score Analysis

## Project Overview
This project focuses on analyzing customer data to understand the factors influencing credit scores and providing actionable insights for financial institutions. The aim is to identify high-value customers, streamline loan approval processes, and improve customer retention through advanced data analysis and machine learning techniques.

## Key Objectives
- Identify high-value customers with good credit scores.
- Automate loan approval processes based on credit scores.
- Improve financial health management for customers through actionable insights.

## Dataset
The analysis utilized a dataset comprising information on 100,000 customers, including:
- Personal attributes (e.g., age, gender, marital status).
- Financial metrics (e.g., income, debt, monthly investments).
- Credit-related attributes (e.g., credit score, outstanding debt, payment behavior).

## Methodology
### Data Preprocessing
- **Data Cleaning**: Addressed missing values and converted mixed data types to appropriate formats.
- **Feature Engineering**: Created derived features like Debt-to-Income Ratio and Investment-to-Income Ratio.
- **Data Encoding**: Applied one-hot, ordinal, and CatBoost encoding for categorical variables.

### Exploratory Data Analysis (EDA)
- **Visualization Tools**: Used Matplotlib and Seaborn for histograms, scatter plots, box plots, and density plots.
- **Correlation Analysis**: Identified relationships between features such as income, debt, and credit scores.
- **Cluster Analysis**: Segmented customers into high-risk and low-risk groups based on financial behavior.

### Modeling
Implemented and compared the following machine learning models:
1. Random Forest
2. Decision Tree
3. Gradient Boosting
4. CatBoost Classifier
5. XGBoost Classifier

#### Performance Comparison:
| Metric        | Random Forest | Decision Tree | Gradient Boosting | CatBoost | XGBoost |
|---------------|---------------|---------------|--------------------|----------|---------|
| Accuracy      | 85%           | 74%           | 78%                | 75%      | 76%     |
| Avg. AUC      | 0.8533        | 0.8533        | 0.89               | 0.88     | 0.89    |
| Features Used | 43            | 43            | 43                 | 20       | 20      |

### Evaluation Metrics
- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**
- **AUC (Area Under the Curve)**

## Key Insights
1. **Income and Credit Scores**: Higher incomes strongly correlate with better credit scores.
2. **Outstanding Debt and Monthly Balance**: High debt levels are linked to lower balances, negatively affecting credit scores.
3. **Credit Utilization Ratio**: Maintaining a low credit utilization ratio significantly boosts credit scores.
4. **Payment Behaviors**: Consistent, on-time payments are critical for higher credit scores.
5. **Investment Patterns**: Regular monthly investments indicate financial stability and higher credit scores.

## Recommendations
1. **Retention Strategies**:
   - Create personalized offers and loyalty programs for high-income customers.
   - Use targeted communication to inform high-value customers about premium financial products.
2. **Debt Management**:
   - Educate customers on reducing debt and maintaining low credit utilization ratios.
   - Offer structured debt reduction plans.
3. **Automated Loan Approvals**:
   - Utilize predictive models like Random Forest for efficient credit evaluations.
   - Fast-track loan approvals for high-scoring customers.
4. **Investment Advisory**:
   - Provide tailored investment products and advisory services to regular investors.

## Dependencies
- Python 3.x
- Libraries:
  - Pandas
  - NumPy
  - Scikit-learn
  - Matplotlib
  - Seaborn
  - XGBoost
  - CatBoost


## Future Work
- Deployment of the solution as a web-based application using Flask or Streamlit.
- Expansion of the dataset to include additional financial metrics.

## Acknowledgments
- Professor Kusun Samarasinghe for guidance and support.
