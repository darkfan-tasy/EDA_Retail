# SampleSuperstore Exploratory Data Analysis Project Report


## Project Overview
<p>This project conducts Exploratory Data Analysis (EDA) on the SampleSuperstore dataset to identify weak areas and potential business problems where improvements can be made to increase profitability. The analysis includes summary statistics, correlation analysis, and profitability analysis by different segments.</p>


## Dataset Description
The SampleSuperstore dataset includes the following columns:

* __Ship Mode__: Shipping mode of the product (e.g., Second Class, Standard Class)

* __Segment___: Customer segment (e.g., Consumer, Corporate)
* __Country__: Country of the customer
* __City__: City of the customer
* __State__: State of the customer
* __Postal Code__: Postal code of the customer
* __Region__: Region of the customer
* __Category__: Product category (e.g., Furniture, Office Supplies)
* __Sub-Category__: Product sub-category (e.g., Bookcases, Chairs)
* __Sales__: Sales amount
* __Quantity__: Quantity of products sold
* __Discount__: Discount applied
* __Profit__: Profit amount
## Exploratory Data Analysis
### Summary Statistics
* __Sales__: 

1. Average : $229.86
2. Standard Deviation : $623.25
3. Minimum : $0.44
4. Maximum : $22,638.48
* __Profit__ :
1. Average : $28.66
2. Standard Deviation : $234.26
3. Minimum : -$6599.98
4. Maximum : $8399.98
* __Discount__ : 
1. Average: 15.62%
2. Minimum: 0%
3. Maximum: 80%
## Distribution of Profit and Sales
* __Profit Distribution__ :
The distribution is highly skewed with a long tail on the negative side, indicating several transactions with significant losses.

* __Sales Distribution__ : 
The distribution is skewed with many transactions having low sales amounts and a few with very high sales.
## Correlation Analysis
* Calculated the correlation matrix for numeric columns.
* Significant Correlations :
1. Positive correlation between Sales and Profit (0.48): Higher sales are generally associated with higher profits.
2. Negative correlation between Discount and Profit (-0.22): Higher discounts often lead to lower profits.
## Profit Analysis by Segments
### Profit by Region
* __West Region__ : Most profitable region with a total profit of $108,418.45.

* __East Region__ : Total profit of $91,522.78.
* __South and Central Regions__ : Lower profits, indicating potential areas for improvement.

### Profit by Category : 
* __Technology__ : Most profitable category with a total profit of $145,454.95.

* __Office Supplies__ : Total profit of $122,490.80.
* __Furniture__ : Lowest profit ($18,451.27), indicating potential issues or opportunities for optimization.
### Profit by Sub-Category 
* __Highly Profitable Sub-Categories__ : 
1. Copiers ($55,617.82)

2.  Phones ($44,515.73)
* __Unprofitable Sub-Categories__ :
1. Bookcases ($-3,472.56)
2. Supplies ($-1,189.10)
3. Tables ($-17,725.48)
## __High Discount, Low Profit Transactions__ 
* Identified 856 transactions with discounts greater than 50% resulting in negative profits.
* These transactions had an average discount of approximately 72%, with an average loss of $89.44 per transaction.
## __Business Insights and Recommendations__ :
1. Optimize Discount Strategy : High discounts are leading to significant losses. Reevaluate the discounting strategy to ensure it's driving profitable sales.
2. Focus on Unprofitable Sub-Categories : Address the issues in unprofitable sub-categories like Bookcases, Supplies, and Tables. This might involve cost reduction, renegotiation with suppliers, or altering the product mix.
3. Regional Strategy : Develop targeted strategies for the South and Central regions to enhance profitability. This could include regional marketing campaigns, localized promotions, or improved logistics and supply chain management.
4. Boost Furniture Category : Since the Furniture category is less profitable, explore opportunities to enhance its performance, such as new product introductions, better inventory management, or targeted promotions.
5. Review Transactional Data : Dive deeper into transactions with high discounts and low profits to identify patterns. Determine if certain customer segments or order types are consistently leading to losses.
## Conclusion
The EDA of the SampleSuperstore dataset provides valuable insights into the business's performance. By addressing the identified weak areas and optimizing strategies, the business can improve profitability and overall performance. The recommendations provided should be implemented and monitored for effectiveness.

## Usage 
To run the analysis, use the provided Python code snippets in a Jupyter Notebook or any Python environment with the necessary libraries installed.

## Requirements
* Python 3.x
* pandas
* seaborn
* matplotlib
 
## Installation 
```
pip install pandas seaborn matplotlib
```
