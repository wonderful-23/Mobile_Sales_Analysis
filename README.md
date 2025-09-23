# Mobile_Sales_Analysis
## Overview:
**This is the sales report for Mobile Sales Product**

---

## Contents
Project Overview/Data Source/Tools used/Table Outlay/Query Language (SQL)/Visualization

---
## Project Overview:
> > This project analyses the sales of mobile sales product to uncover insights on sales distribution by various atttributes such as Brands,Customer Gender,Payment Method using pivot table, I explored metrics like total sales by Payment Method and Gender ,Average income of buyers, Gender distribution and Overall Revenue. This analysis helps to undestand the key factors driving sales in the dataset provided

## Data Source:
www.kaggle.com/dataset

## Tools Used:
+ Pivot Table/ Charts
+ PowerBI
+ SQL

  ## Table Outlay:
 First three Record
 
|TransactionID|	Date	|MobileModel	|Brand	|Price	|UnitsSold	|TotalRevenue	|CustomerAge	|CustomerGender	|Location	|PaymentMethod|
|-----|-----|------|-----|-------|------|------|------|-------|-------|------|
|79397f68-61ed-4ea8-bcb2-f918d4e6c05b|	1/6/2024|	direction|	Green Inc|	1196.95|	85|	28002.8|	32|	Female|	Port Erik|	Online|
|4f87d114-f522-4ead-93e3-f336402df6aa|	4/5/2024|	right|	Thomas-Thompson|	1010.34|	64|	2378.82|	55|	Female|	East Linda|	Credit Card|
|6750b7d6-dcc5-48c5-a76a-b6fc9d540fe1|	2/13/2024|	summer|	Sanchez-Williams|	400.8|	95|	31322.56|	57|	Male|	East Angelicastad|	Online|

## Query Language: (SQL)
Some of the query language to retrieve records are displayed here.

```SQL
---calculate the TotalRevenue by Price---
SELECT PaymentMethod, SUM(Price) AS TotalRevenue
fROM Mobile_Sales
GROUP BY PaymentMethod
ORDER BY TotalRevenue DESC;
```

```SQL
---categorise the data into gold,ilver and diamond---
SELECT*,
CASE
WHEN Price < 500 THEN 'Silver'
WHEN Price BETWEEN 500 AND 1000 THEN 'Gold'
ELSE 'Diamond'
END AS 'Category'
FROM Mobile_Sales

```
## Visualization
### Pivot table 
<img width="1309" height="467" alt="mobile_sales (2) - Excel 9_19_2025 1_32_54 PM" src="https://github.com/user-attachments/assets/967a17fc-882c-4eb7-8615-13211fe02a53" />

### PowerBI Dashboard
 
<img width="1029" height="595" alt="powerbi_august_13 (1) pdf - Profile 1 - Microsoft​ Edge 9_23_2025 2_32_37 PM" src="https://github.com/user-attachments/assets/74399123-f945-4d41-a581-f8ac68dbbda4" />

### link to chart
[link to profilling](https://ibb.co/fGxx0Rdm)

[view my linkedIn profile](www.linkedin.com/in/wonderful-ajiboye)
