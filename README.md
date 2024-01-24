# Customer-Segmentation-in-Airline-Industry-
One of the challenges in the airline industry is to improve revenue management and optimize resource allocation through a data-driven approach that segments users, enabling differentiated pricing and services. Customer segmentation has been crucial to business because such clustering allows businesses to offer better products that accommodate different needs, create great traveling experiences, and attract various types of travelers through individualized product design. Implementing restriction management will optimize revenue and airline occupancy by offering tickets at varying prices with different restrictions. Failure to do so leads to customers not feeling the travel experience is worth the value of the ticket price paid, which leads to decreased purchase frequency. 

Many companies segment customers by demographic, geographic, and behavioral characteristics. In our research, we propose a model to divide customer segmentation by behaviors, which involves placing the right passenger in the right seat at the right price and at the right time. By categorizing seats into appropriate types of seats and understanding the travel purpose of passengers, which could be business, bleisure, vacation, visiting friends and relatives (VFR), or personal, a systematic, data-driven pricing model could be developed that maximizes fare value per passenger. 

## Instructions
All Codes and more detailed notes can be found in the python notebook

### I．	Data Process
a)	Data Preparation (Prepare Data for Processing)
i.	Combine Rows from all Sheets (Combine 5 sheets of data into 1)
ii.	Data Cleaning (Cleaning data types and missing values)
1.	Convert Missing Value Type
2.	Drop Missing Rows in Channel Column
3.	Convert Data Format for Modeling
4.	Convert Origin/Dest/OD Columns into Route
5.	Complete Travelling Probability Columns and Create Top Purpose Column
6.	One-Hot Encode Channel and Travelling Purpose
b)	Feature Engineering (Engineer New Features for Modeling)
i.	Date
1.	PNR Create Date
2.	PNR Depart Date
ii.	Advance Purchase Date
iii.	Round Trip
iv.	Distance
v.	Revenue
vi.	Travelling Alone
vii.	Bin Advance Purchased Time
1.	Advance Purchase Day
2.	Advance Purchase Month

### II．	Modeling
a)	Data Load
b)	Modeling
i.	Determine the Number of Clusters (WCSS and Elbow Method)
ii.	Actual Model (Kmeans with nCluster=4)
iii.	Accuracy of Kmeans Model
c)	Summarize Clusters
i.	Averages of Clusters
ii.	Number of Observations in Clusters
d)	Graph and Insight about Clusters (Understand the distribution in each cluster)
i.	RPP
1.	Ratio to MedRPP Pies
2.	Ratio to MedRPP Bars
ii.	Channel Pies
iii.	Round Trip Pie
iv.	Travel Alone Pies
v.	Travelling Purpose Pies
vi.	Advance Purchase
1.	Advance Purchase Day Stacked Bar Charts
2.	Advance Purchase Month Stacked Bar Charts
e)	Visualization of Clusters

