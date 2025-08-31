Effective inventory and sales management are critical for optimizing 
profitability in the retail and wholesale industry. Companies need to ensure 
that they are not incurring losses due to inefficient pricing, poor inventory 
turnover, or vendor dependency. The goal of this analysis is to: 
● Identify underperforming brands that require promotional or pricing 
adjustments. 
● Determine top vendors contributing to sales and gross profit. 
● Analyze the impact of bulk purchasing on unit costs. 
● Assess inventory turnover to reduce holding costs and improve 
efficiency. 
● Investigate the profitability variance between high-performing and 
low-performing vendors.

Exploratory Data Analysis Insights  
Summary Statistics
Negative & Zero Values: 
Gross Profit: Minimum of -52,002.78, indicating potential losses due to 
high costs or heavy discounts. This could be due to selling products at 
lower prices than their purchase costs. 
Profit Margin: Has a minimum of -∞, which suggests instances where 
revenue is zero or even lower than the total cost, leading to extreme 
negative profit margins. 
Total Sales Quantity & Sales Dollars: Some products show zero sales, 
indicating they were purchased but never sold. These may be slow-moving 
or obsolete stock, leading to inventory inefficiencies. 
Outliers Detected by High Standard Deviations:  
Purchase & Actual Prices: The maximum values (5,681.81 & 7,499.99) 
are significantly higher than the mean (24.39 & 35.64), indicating premium 
product offerings. 
Freight Cost: Extreme variation from 0.09 to 257,032.07 suggests logistics 
inefficiencies, bulk shipments, or erratic shipping costs across different 
products. 
Stock Turnover: Ranges from 0 to 274.5, suggesting some products sell 
rapidly while others remain unsold for long periods. A value greater than 1 
indicates that sales for a product exceed the purchased quantity due to 
older stock fulfilling orders.

Data Filtering 
To enhance the reliability of the insights, we removed inconsistent data 
points where: 
● Gross Profit ≤ 0 (to exclude transactions leading to losses). 
● Profit Margin ≤ 0 (to ensure analysis focuses on profitable 
transactions). 
● Total Sales Quantity = 0 (to eliminate inventory that was never sold).

Purchase Price vs. Total Sales Dollars & Gross Profit: Weak correlation 
(-0.012 and -0.016), indicating that price variations do not significantly 
impact sales revenue or profit. 
Total Purchase Quantity vs. Total Sales Quantity: Strong correlation 
(0.999), confirming efficient inventory turnover. 
Profit Margin vs. Total Sales Price: Negative correlation (-0.179), 
suggesting increasing sales prices may lead to reduced margins, possibly 
due to competitive pricing pressures. 
Stock Turnover vs. Gross Profit & Profit Margin: Weak negative 
correlation (-0.038 & -0.055), indicating that faster stock turnover does not 
necessarily equate to higher profitability. 
