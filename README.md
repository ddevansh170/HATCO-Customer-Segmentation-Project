# HATCO Customer Segmentation

## Problem Statement

Hacto dataset was obtained from the Hair, Anderson, and Tatham Company (HATCO), a large (though
nonexistent) industrial supplier. It represents surveys of HATCO customers that
were collected through an established marketing research firm. 
The data provided should give HATCO a better understanding of both the
characteristics of its customers and the relationships between their perceptions of
HATCO and their actions toward HATCO (purchases and satisfaction).

## Data Defination

The dataset consists of 100 observations on 14 separate variables and is an example of a segmentation study for a B2B situation, specifically a survey of existing customers of HATCO. Three types of information were collected:

- First is the perception of HATCO on seven attributes identified in past studies as the most influential in the choice of suppliers. The respondents, purchasing managers of firms buying from HATCO, rated HATCO on each attribute.
- Second are actual purchase outcomes, either the evaluations of each respondent's satisfaction with HATCO or the percentage of his or her product purchases from HATCO.
- Third are general characteristics of the purchasing companies (e.g., firm size, industry type).

#### 1.) Perceptions of HATCO
- X1 Delivery speed---amount of time it takes to deliver the product once an order has been confirmed
- X2 Price level---perceived level of price charged by product suppliers
- X3 Price flexibility---perceived willingness of HATCO representatives to negotiate price on all types of purchases
- X4 Manufacturer's image---overall image of the manufacturer/supplier
- X5 Service---overall level of service necessary for maintaining a satisfactory relationship between supplier and purchaser
- X6 Salesforce's image---overall image of the manufacturer's sales force
- X7 Product quality---perceived level of quality of a particular product (e.g., performance or yield) 

#### 2.) Purchase Outcomes
- X9 Usage level---how much of the firm's total product is purchased from HATCO, measured on a 100-point percentage scale, ranging from 0 to 100 percent
- X10 Satisfaction level---how satisfied the purchaser is with past purchases from HATCO, measured on the same graphic rating scale as the perceptions X1 to X7

#### 3.) Purchaser Characteristics 
- X8 Size of firm---size of the firm relative to others in this market. This variable has two categories: 1=large, and 0=small
- X11 Specification buying---extent to which a particular purchaser evaluates each purchase separately (total value analysis) versus the use of specification buying, which details precisely the product characteristics desired. This variable has two categories: 1=employs total value analysis approach, evaluating each purchase separately, and 0=use of specification buying
- X12 Structure of procurement---method of procuring/purchasing products within a particular company. This variable has two categories: 1=centralized procurement, and 0=decentralized procurement
- X13 Type of industry---industry classification in which a product purchaser belongs. This variable has two categories: 1=industry A classification, and 0=other industries
- X14 Type of buying situation---type of situation facing the purchaser. This variable has three categories: 1=new task, 2=modified rebuy, and 3=straight rebuy 

## Modeling :-
- Multiple linear regression is a the best model when the response variable is numeric in nature. It helps in the prediction of future values from given values of predictors. 
- In this study X9 Usage level of the customers is predicted using the perception of the Hacto customers.
- Then X8 Size of Firm is added to Independent variables to check the change in the robustness of the model for X9 Usage Level.
- K-means clustering is used to group/segment customers into distinct groups having similar perception for Hatco customers.

## Insights :-
- The Usage level of HATCO customers were dependent on the Delivery Speed of the products, Price Level, Price flexibility, Manufacturer’s image, Service for maintaining a satisfactory relationship with purchaser, overall image of HATCO’s sales force and its product quality.
- K means clustering with K=2 grouped the customers according to their perception towards their purchase with HATCO in following
- Cluster 1 :- Customers whose perception towards HATCO is that they are okay with low delivery speed and high price level, but they demand very permium product quality.
- Cluster 2 :- Customers who are looking for high delivery speed with low price level for supplies and high price flexibility.
- K means clustering with K=4 grouped the customers according to their perception towards their purchase with HATCO.
- Cluster 1:-This group has customers who demand low price level, high price flexibility and they don’t mind if the salesforce’s image and product quality of the supplies is not good.
- Cluster 2:-This group has customers who have no issues with low delivery speed, service level for healthy relationship but at the same time they are looking for very high product quality for supplies from HATCO
- Cluster 3:- These customers demand high delivery speed, low price level, very high price flexibility and high HATCO’s salesforce image.
- Cluster 4:- This group doesn't mind paying high prices, but they want the manufacturer's image to be good along with services they provide should be very satisfactory. They also looking for salesforce’s image and product quality.

## Model Performance :-
- Linear Regression with predictors X1 to X7 gave R2 value of 77.5, Adj R2 value of 75.8, AIC value of 588.8 and BIC value of 609.7
- Linear Regression model with predictors X1 to X8 gave R2 value of 80.2, Adj R2 value of 78.5, AIC value of 577.8 and BIC value of 601.3
- Adding Firm Size X8 in the predictors significantly increased the robustness of the model.
- K-Means clustering with K= 2 grouped the customers into 2 separate groups with certain characteristics, with Silhouette Score of 35.89
- Similarly, K-Means clustering with K= 4 grouped the customers into 4 separate groups with certain characteristics, with Silhouette Score of 33.81

## Recommendation :-
- Proper marketing strategy could be adopted for each group of customers to increase their perception level towards HATCO.
- Expanding into new markets can be costly, but it can increase your client base. Market research will help you understand the potential new market and help you devise a strategy. You'll also need to consider marketing, sales, distribution, and increasing your production to meet the new demand.
- Changing your prices, terms, or conditions of billing could stimulate market demand for your products or services. Be aware of what your competitors are offering and what your own profit margins are to determine if you can reduce your cost. If lowering your price isn’t an option, improving a deal with favorable terms can often influence customers.
- Always be aware of what your competitors are doing. This information helps you understand their behaviors, capabilities and limitations. If you have this knowledge, you will be better prepared to defend your market position, react to changes, and find new markets.
- Increase your presence and visibility in your community. Activities such as sponsoring community events, speaking at engagements, or supporting a local sports team can raise awareness of your business and stimulate sales.
- Be aware of the customer's perception of your customer service quality or responsiveness. Positive word of mouth from a happy customer is valuable to your business.


