# Predict-Dividend, 배당금 예측모델

To use the [Rapidminer](https://rapidminer.com/), Python and [KISVALUE](https://www.kisvalue.com/web/index.jsp) to make a predict model to which company will payout the dividend.


[Rapidminer](https://rapidminer.com/), Python, [KISVALUE](https://www.kisvalue.com/web/index.jsp)를 사용하여 배당금 예측 모델을 만들었습니다.


## Project overview
How much the company can pay out the dividend to the investors. That’s the one of the keys to decide the invest. So, we need to know what kind of financial statement effect to dividend is for wise invest decision making. Using the KOSPI, KOSDAQ listing company’s financial statement to find out what kind of statements are sufficient to predict the dividend. And make the model to test the statements what we chose is important factor in investment decisions.

### 1. Program I use: Rapidminer, KISVALUE
KISVALUE – The program provides the company’s financial data as CSV in the Korea stock market.


### 2. Model I use: Logistic Regression, Decision Tree(C5, CART), Neural Network
1.	Logistic Regression
  - Reason why I choose: Dependent variable is binary. So, it’s easy to categorize the plus and minus value of the data

2.	Decision Tree – C5


  - The root node decision of C5 determines that the more pure the value of the node of the variable, the clearer the true and false values of the value, and that more accurate analysis is possible with less information.
  
3.	Decision Tree – CART


  -	In CART, if the nodes are pure, they are grouped into the same class, and this probability is considered 1. Therefore, the larger the CART value, the greater the homogeneity and the greatest homogeneity is the root node.
  
4.	Neural Network


  -	Through the number of hidden layers and the number of hidden nodes, prediction through learning between variables is possible. The most effective modeling is modeling using the least nodes while showing the highest predictive accuracy
  
### 3. Data: 2016, 2017, 2018 KOSPI, KOSDAQ-listed non-financial company
+ Independent variable(binary): Increase or decrease of dividend (increase: 1, decrease: 0)

+ Dependent variable: retained earnings, dividends per share, dividend, cash dividend, current ratio, quick ratio, net income, debt ratio, gross sales, gross sales per capita, accounts receivables turnover, inventory turnover, revenue growth, ROE, internal possession rate of stocks, beta(5Y Monthly), market cap, capita, credit score, company size
