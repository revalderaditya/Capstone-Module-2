# Capstone-Module-2
## Online Retail Shipping
### By: Revalde Raditya Candra

In this Capstone project, I will analyze Online Retail Shipping data. The main objective of this data is to tackle the number of Not Reached on Time, almost half of the total data.

## Findings and Cleaning

Findings from the analysis of the Online Retail Shipping dataset are as follows: The dataset consists of 12 columns and 10,999 rows. There are no columns that contain NaN values. The ID column contains unique customer identification numbers without any duplicates. Among the columns, only Warehouse_block, Mode_of_shipment, Product of importance, and Gender are of object type, while the remaining columns are of integer type. Certain columns, such as Customer_rating and Reached.on.Time_Y.N, can be defined based on the presence of codes. The correlation between variables is generally low, with no significant values above 0.05, indicating that descriptive analytics will be the primary focus. Null or NaN values were not found in the dataset using the isna() and isnull() methods. Duplicate data was also not detected using the duplicated() method. Outliers were not identified after performing outlier detection using the interquartile range (IQR). Notably, out of the total 10,999 orders, more than half (6,563) were labeled as '1', indicating they were not delivered on time.
