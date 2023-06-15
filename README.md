# Capstone-Module-2
## Online Retail Shipping
### By: Revalde Raditya Candra

In this Capstone project, I will analyze Online Retail Shipping data. The main objective of this data is to tackle the number of Not Reached on Time, almost half of the total data.

## Findings and Cleaning

Findings from the analysis of the Online Retail Shipping dataset are as follows: The dataset consists of 12 columns and 10,999 rows. There are no columns that contain NaN values. The ID column contains unique customer identification numbers without any duplicates. Among the columns, only Warehouse_block, Mode_of_shipment, Product of importance, and Gender are of object type, while the remaining columns are of integer type. Certain columns, such as Customer_rating and Reached.on.Time_Y.N, can be defined based on the presence of codes. The correlation between variables is generally low, with no significant values above 0.05, indicating that descriptive analytics will be the primary focus. Null or NaN values were not found in the dataset using the isna() and isnull() methods. Duplicate data was also not detected using the duplicated() method. Outliers were not identified after performing outlier detection using the interquartile range (IQR). Notably, out of the total 10,999 orders, more than half (6,563) were labeled as '1', indicating they were not delivered on time.

## Data Analysis
### Mode of Shipment

Upon analyzing the Mode of Shipment, it can be concluded that the shipping method is often late compared to other modes of shipment. The shipping method is notably the most widely used method for shipment. To address this issue, the most effective alternative could be road transport, as it shows the lowest percentage of late deliveries. However, the road method has its limitations, especially when the shipment needs to pass over a body of water, making this method quite challenging. 

The second option is air transport, which, although potentially expensive, has a comparatively lower percentage of late deliveries and could therefore be considered a viable alternative. The last option is shipping, which is capable of traversing seas and is more cost-effective than air transport; however, it has a significantly higher percentage of late deliveries. 

In order to improve this situation, several recommendations could be considered when using shipping as the transport option:

* Implement a buffer in the Estimated Time of Arrival (ETA) to prevent late deliveries.
* Consider engaging with a Third Party Logistics (3PL) provider known for on-time deliveries.
* Implementing real-time tracking systems to monitor the progress of shipments will make the delivery process easier to identify and address any delays as soon as they occur.
* Use advanced routing software to find the most efficient routes. This can help to reduce transit times and increase the likelihood of on-time delivery. Consider factors like traffic, road conditions, and weather.

### Prior Purchases
From the graph and the chi-square test, it can be concluded that orders with three prior purchases have the highest incidence of not being delivered on time. Moreover, the rate of late deliveries decreases as the number of prior purchases increases. The chi-square test also confirms a significant relationship between the number of prior purchases and the "Reached on Time" metric.

### Warehouse Block
Upon examining the Warehouse Block, we observe that warehouse F stands out as the primary contributor to deliveries that did not reach on time. This could lead to the initial conclusion that warehouse F is the least efficient among all the warehouses. However, upon closer inspection, we find that warehouse F's performance is not the most subpar. 

Consider warehouse B, for example: it only contributes to 16.4% of on-time deliveries, whereas its contribution to late deliveries is slightly higher at 16.8%. The only warehouse that has a "surplus" - defined as a higher percentage contribution to on-time deliveries than to late deliveries - is warehouse A. It contributes to 17.1% of on-time deliveries and only 16.4% of late deliveries.

To address the inefficiencies in the warehouses that do not have an on-time delivery surplus, a few measures can be taken. The transport manager could consider increasing loading space to allow for more efficient product loading onto vehicles. In addition, the location of the warehouse itself can significantly impact delivery times. For instance, if a warehouse is located in a less accessible area, it can delay deliveries. Therefore, gathering feedback from the drivers about warehouse locations could provide valuable insights for improving delivery efficiency.

### Customer Rating
Products with a customer rating of 1, indicative of the lowest customer satisfaction, oddly exhibit the most instances of 'reached on time' or a value of '0'. On the other hand, products with a rating of 5, reflecting the highest customer satisfaction, record the fewest instances of 'reached on time'. This suggests that a high customer rating does not merely represent timely delivery but implies an overall customer satisfaction with the service.

In the delivery process, several factors could affect the customer rating, even when the delivery was made on time, including:

* The delivery arrived on schedule, but the quantity of the product sent was not complete.
* The product was damaged during the delivery process.
* The product delivered differed from the customer's original request.
* The product received was not up to the quality standard expected by the customer.
* Lack of proper updates or tracking information provided during the shipping process.

## Conclusions
* Every mode of shipment comes with unique challenges, hence, a well-thought-out shipment plan is crucial to meet the promised ETA.
* Regular orders are advantageous for shipments as familiarity with the area increases the driver's chances of successful on-time deliveries.
* Each warehouse might face unique challenges, like Warehouse F dealing with a large volume of products. Despite being part of the warehousing, not the transport sector, such challenges can impact on-time delivery rates. Hence, process improvement within the warehouse is essential.
* While customer rating might not reflect the entire end-to-end process, a mishap in any part, such as a mistake during the picking process, can lead to customer dissatisfaction. This might result in poor customer ratings, even if the delivery was on time.

## Recommendations
* Incorporate buffer time into the Estimated Time of Arrival (ETA) to mitigate the risks of late deliveries.
* Engage with a Third Party Logistics (3PL) provider that is recognized for timely deliveries.
* Adopt real-time tracking systems for the transport team to oversee shipment progress. This will help identify and address any potential delays promptly.
* Utilize advanced routing software to determine the most efficient routes, factoring in variables such as traffic, road conditions, and weather. This could help reduce transit times and increase the likelihood of on-time delivery.
* Where feasible, retain the same driver or the same 3PL for repeat customers. This ensures familiarity with the customer's location and potentially speeds up the delivery process.
* Strive to maintain a "surplus" percentage in each warehouse block to prevent potential shortfalls.
* Encourage Warehouse A to share its loading method and area layout plans with the other warehouses. Regular comparisons could foster improvements across all locations.
* Implement a tracking system that allows customers to monitor the delivery process. This transparency can enhance customer satisfaction and operational efficiency.

**THANK YOU**
