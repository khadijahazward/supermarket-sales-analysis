# Supermarket Sales Analysis

This project analyzes a supermarket sales dataset from January 2019 to March 2019 to identify key factors affecting profitability. By understanding how different attributes such as customer type, product categories, purchase times, and payment methods influence gross income, this analysis provides actionable insights to improve revenue generation.

## Dataset Information

- **Source**: [Supermarket Sales Dataset](https://www.kaggle.com/datasets/aungpyaeap/supermarket-sales/data) from Kaggle
- **Time Period**: January 2019 - March 2019
- **Attributes**:
  - Invoice ID
  - Branch
  - City
  - Customer Type
  - Gender
  - Product Line
  - Unit Price
  - Quantity
  - Tax
  - Total
  - Date
  - Time
  - Payment Method
  - COGS (Cost of Goods Sold)
  - Gross Margin Percentage
  - Gross Income
  - Customer Rating

## Technologies Used

- **Programming Language**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
- **Environment**: Jupyter Notebook

## Data Analysis Process

### 1. Data Collection
- Loaded the dataset from Kaggle.

### 2. Data Preprocessing
- Cleaned the data by ensuring there were no missing values.
- Derived new features such as:
  - **Hour**: Extracted from Date & Time.
  - **Day Type**: Classifying days as Weekday or Weekend.
- Removed redundant columns such as:
  - Gross Margin Percentage
  - City
  - Date/Time (after extraction)
  - Tax 5%
  - Total

### 3. Exploratory Data Analysis (EDA)
- Conducted summary statistics and visualized key trends in the dataset.
- Analyzed how various attributes influence gross income.

### 4. Statistical Analysis
- Performed correlation analysis on numerical attributes.
- Applied one-hot encoding to categorical attributes and analyzed their correlation with gross income.

## Findings & Recommendations

- **Membership Programs**: Both members and non-members contribute similarly to sales. Personalized promotions can drive more effective engagement.
- **Payment Methods**: Payment methods don’t directly impact gross income, but offering discounts for preferred payment methods may encourage increased spending.
- **Weekend Sales Strategy**: Peak sales occur on weekends, suggesting a strategy of more staff and promotions to maximize weekend sales.
- **Product Line Optimization**: Health & Beauty and Sports & Travel are the most profitable categories. Focus efforts on optimizing these and consider changes to low-performing categories.
- **Bulk Purchasing Incentives**: Implement bulk purchasing deals or combo offers to increase revenue.
- **Strategic Pricing**: A/B testing and time-limited discounts can be used to optimize product pricing.
- **Branch Performance**: No significant difference in branch performance; improvements should be made across all locations.
- **Weekday Sales Improvement**: Consider offering time-based discounts to target office workers and students during weekdays.
- **Gender & Marketing**: The correlation with income is weak. A more targeted approach should focus on other factors such as age, lifestyle, and behavior.

## How to Run

1. Clone the repository:

    ```bash
    git clone https://github.com/khadijahazward/supermarket-sales-analysis.git
    ```

2. Install the necessary dependencies:

    ```bash
    pip install -r requirements.txt
    ```

3. Launch the Jupyter Notebook:

    ```bash
    jupyter notebook
    ```

4. Open the notebook `Supermarket_Sales_Analysis.ipynb` to explore the analysis.