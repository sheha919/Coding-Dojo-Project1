# Project 1 - Part 1
- Author: Shehani Wetthasinghe
- Last modified: 10/13/2022
##Overview

## Data Types
| Column Name               | Data Type      | Description                                                                                           |
| -------------             | -------------  |-------------------------------------------------------------------------------------------------------|
| Item_Identifier           | object         | Unique product ID                                                                                     | 
| Item_Weight               | float          | Weight of product                                                                                     |
| Item_Fat_Content          | object         | Whether the product is low fat or regular                                                             |  
| Item_Visibility           | float          | The percentage of total display area of all products in a store allocated to the particular product   |
| Item_Type                 | object         | The category to which the product belongs                                                             |
| Item_MRP                  | float          | Maximum Retail Price (list price) of the product                                                      |
| Outlet_Identifier         | object         | Unique store ID                                                                                       | 
| Outlet_Establishment_Year | int            | The year in which store was established                                                               |
| Outlet_Size               | object         | The size of the store in terms of ground area covered                                                 |
| Outlet_Location_Type      | object         | The type of area in which the store is located                                                        |
| Outlet_Type               | object         | Whether the outlet is a grocery store or some sort of supermarket                                     |
| Item_Outlet_Sales         | float          | Sales of the product in the particular store. This is the target variable to be predicted             |


## Exploratory Visuals
![image](https://user-images.githubusercontent.com/50593017/194176046-46d7a187-0ec4-41cb-a2bc-a9a31eb5e238.png)
![image](https://user-images.githubusercontent.com/50593017/194176065-a71e04d2-6ccb-40d7-b88c-8904c01e15e7.png)
![image](https://user-images.githubusercontent.com/50593017/194176077-23bf57be-ee91-45e8-b351-73aec1633ddd.png)
![image](https://user-images.githubusercontent.com/50593017/194176127-48c02af3-5ff2-4e7f-ba3f-b32e1b455ca7.png)

## Explanatory Visuals
![image](https://user-images.githubusercontent.com/50593017/194176181-b80af4dc-5587-436b-ae13-91237bc8390d.png)
![image](https://user-images.githubusercontent.com/50593017/194176205-e1ac7dfd-5275-4872-9af7-6b2e443423a5.png)
![image](https://user-images.githubusercontent.com/50593017/194176232-0f6571e6-9c11-49a9-b8d0-2bb33f37ee70.png)

## Performance of ML models 
|Model|Train R2|Test R2|Train RMSE|Test RMSE|
|---|---|---|---|---|
|Linear Regression|0\.560571|0\.565842|₹1140\.38|₹1094\.46|
|Decision Tree    |0\.603933|0\.594709|₹1082\.66|₹1057\.44|

- Above table illustrated the summary of the performance of the two models used in this work.
- In both models, corresponding train and test R2 scores are approximately equal to each other. That says they are not overfitting.
- Since all R2 score values are above 0.3, the models are not underfitting too.
- Here I conclude that the decision tree model is the best performing model since it obtained;
    - highest test R2 score
    - lowest train and test RMSE values
    - lowest diffrence value between train and test RMSE

