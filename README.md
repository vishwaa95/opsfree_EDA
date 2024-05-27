# Exploratory Data Analysis (EDA) of Microservice Tracing Data
Microservices architecture is a software development approach where an application is composed of small, independent services that communicate over well-defined APIs. 
This project focuses on analyzing microservice traces to gain insights into the performance and behavior of these services. <br>

## Table of Content
- General Info
- Technologies Used
- Conclusions

## General Info
- Microservices architecture is a software development approach where an application is composed of small, independent services that communicate over well-defined APIs. 
This project focuses on analyzing microservice traces to gain insights into the performance and behavior of these services. 
The primary goal is to perform exploratory data analysis (EDA) on the provided trace data, which will help identify patterns, trends, 
and potential anomalies in the duration of various operations.<br>

## Technologies Used
- Pandas - 2.0.3
- Numpy - 1.25.2
- Seaborn - 0.13.1

## Conclusion 
- The average duration for the different services is 5.41 * 10^6 Nano seconds
- From the above plot for ServiceName we can see that the microservice that is used most is frontend followed by cartservice, productcatalogservice and loadgenerator.
- From the Name plot we can see that the method being executed are HTTP GET followed by oteldemo.Productcatalogservice/GetProduct, grpc.oteldemo.ProductCatalogService/Getproduct and HTTP Post
- From the boxplot we can observe that in the boxplot for ServiceName vs DurationNano we have extreme outlier in case of frontend-proxy and loadgenerator.
- From the boxplot between Name vs DurationNano We can observe that ingress and HTTP GET has clear outliers
- From the above plot we can see that loadgenerator has the highest average time among ServiceName which is consistent with our previous findings.
- From the plot above we can see that documentload has the highest average time in Name
