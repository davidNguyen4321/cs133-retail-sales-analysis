# cs133-retail-sales-analysis

AUTHORS: DAVID NGUYEN
DATASET: Retail Sales Dataset
SOURCE: https://www.kaggle.com/datasets/danielsowah123/retail-sales-dataset

This is an amateur data analysis and visualization project to practice using Python and its relevant data analysis libraries. In business, sales reports and figures are highly important to make and gauge business decision. This project aims to create reports based on realistic data to help guide those decisions. The project will analye data to find clear trends in profitability and predict the value of investing in certain products. It will illustrate the report visually to highlight crucial information in an easily-digestible manner. This project will help businesses make informed decisions to catch unproffitable ventures and make sound investments on strong products.

## PROJECT OUTLINE

Using the dataset, there will be an interactive page separated into collapsible tabs, where each tab has a major statistical insight about the dataset, visualized. These insights may (but not necessarily) include high positive/negative correlations, common patterns in missing values, and other statistically significant results. Additionally, there will be a special tab with two dropdowns to select two columns. Upon selecting two columns, a small report will be generated, with an appropriate test based on the content type of each column (categorical, numerical). There will be an accompanying graph for each mini-report.

Data was collected from a publically available source, and is stored in the repository for ease of use, as the data is in the public domain. Ideally, data would be stored in a specialized content delivery network or database, but due to the small scope of the project, it is ouside the scope of the project.

Data will be analyzed and visualized using various Python libraries. Those libraries include (but are not strictly limited to): Pandas, NumPy, Seaborn, and Matplotlib.

## DATA DICTIONARY

For more information on each column, refer to the data dictionary that accompanied the dataset download. Note: some data is reported to be a different datatype than is in the dataframe, but that will be fixed during data cleaning. Also, the list of all possible values will be listed for columns with ten or fewer possible values.

Transaction_ID: Unique identifier for an individual transaction record (text)
Order_ID: Identifier for the customer order; multiple lines may share an order (text)
Customer_ID: Identifier for the customer (text)
Customer_Name: Customer name from CRM (text)
Customer_Age: Customer age at transaction, in years (integer)
Customer_Gender: Customer-reported gender {Male, Female, Non-Binary, male, FEMALE, nan, Non Binary} (text)
Customer_Segment: Commercial/lifecycle customer segment {Consumer, Corporate, New Customer Returning Customer, Small Business, Premium} (text)
Order_Date: Date transaction was placed (date)
Order_Time: Time transaction was placed (time)
Sales_Channel: Order channel {Online, B2B Portal, Retail Store, Phone Order} (text)
Store_ID: Store/location identifier (text)
Store_Name: Store/location name (text)
Country: Country of sale {United States, Australia, France, Canada, United Kingdom, Germany} (text)
Region: State/province/region (text)
City: City of sale (text)
Product_ID: Product identifier (text)
Product_Name: Product name (text)
Product_Category: High-level product category {Electronics, Office Supplies, Furniture, Appliances, FURNITURE, electronics, Office supplies} (text)
Product_Subcategory: Detailed product group (text)
Quantity: Units in transaction (integer)
Unit_Price: Price per unit before discount (decimal)
Discount_Percentage: Discount applied {5, 15, 0, 20, 10, 25, 30, 45, 60, 110} (decimal)
Sales_Amount: Recorded net sales amount (decimal)
Cost_Amount: Recorded transaction cost (decimal)
Profit: Recorded transaction profit (decimal)
Payment_Method: Payment method (text)
Order_Status: Operational order status {Completed, Shipped, Returned, Processing, Cancelled, SHIPPED, completed, processing} (text)
Shipping_Method: Fulfillment/shipping method {Standard, Next Day, Express, Pickup} (text)
Delivery_Days: Recorded delivery duration in days (integer)
Return_Flag: Whether transaction was returned {No, Yes} (text)
Return_Reason: Return reason if applicable {nan, Damaged, Changed Mind, Other, Defective, Late Delivery, Wrong Item} (text)
Sales_Representative: Sales representative (text)
Promotion_Code: Promotion/campaign code (text)
Customer_Rating: Customer rating, generally 1-5 {4, 5, nan, 2, 1, 3} (decimal)
Inventory_Level: Approximate inventory at transaction (integer)
Order_Year: Year derived from Order_Date {2022, 2024, 2025, 2023} (integer)

## MISSING VALUES

Columns with zero missing values are omitted

Customer_Name: 108 missing (0.599%)
Customer_Age: 218 missing (1.208%)
Customer_Gender: 162 missing (0.898%)
Product_Name: 144 missing (0.798%)
Payment_Method: 147 missing (0.815%)
Delivery_Days: 162 missing (0.898%)
Return_Reason: 16168 missing (89.598%)
Promotion_Code: 9737 missing (53.96%)
Customer_Rating: 3435 missing (19.036%)
Inventory_Level: 198 missing (1.097%)