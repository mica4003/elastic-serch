# elastic-serch
# Online Retail data set:
InvoiceNo: Invoice number. Nominal, a 6-digit integral number uniquely assigned to each transaction. If this code starts with letter 'c', it indicates a cancellation. 
StockCode: Product (item) code. Nominal, a 5-digit integral number uniquely assigned to each distinct product. 
Description: Product (item) name. Nominal. 
Quantity: The quantities of each product (item) per transaction. Numeric.	
InvoiceDate: Invice Date and time. Numeric, the day and time when each transaction was generated. 
UnitPrice: Unit price. Numeric, Product price per unit in sterling. 
CustomerID: Customer number. Nominal, a 5-digit integral number uniquely assigned to each customer. 
Country: Country name. Nominal, the name of the country where each customer resides.

create retails index,create index_config
group by invoice num,iterate over each group (each invoice)## iterate over rows in this invoice dataframe
fling to elasticsearch


Aggregation
Here we are querying
for documents that contain the ingredient "StockCodes": "21523".
Then we scrape inside those documents for other order that co-occur
with "StockCodes": "21523"
we use the aggregation "significant_terms"
which orders rarer correlated words first.

