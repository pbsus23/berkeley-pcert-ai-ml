# Practical Application Assignment 11.1: What Drives the Price of a Car?

### 1) Overview**

In this application, we are exploreing a dataset from kaggle. The original dataset contained information on 3 million used cars. The provided dataset contains information on 426K cars to ensure speed of processing. Our goal is to understand what factors make a car more or less expensive. As a result of this analysis, we can provide clear recommendations to our client -- a used car dealership -- as to what consumers value in a used car.

Here is link of my Jupyter notebook with all details together with analysis, coding evaluation, findings and conclusiuon.


Below are the brief description of the solution approach to findings and conclusion:
[Jupyter Notebook](https://github.com/pbsus23/berkeley-pcert-ai-ml/tree/main/PracticalApp2/prompt_II.ipynb)

### 2) Standard Process: CRISP-DM Framework**

To frame the task, throughout our practical applications we will refer back to a standard process in industry for data projects called CRISP-DM. This process provides a framework for working through a data problem. 
<img src="images/crisp" alt="Figure: CRISP-DM Framework">

### 3) Business Understanding

From a business perspective, we are tasked with identifying key drivers for used car prices. In the CRISP-DM overview, we are asked to convert this business framing to a data problem definition. Using a few sentences, reframe the task as a data task with the appropriate technical vocabulary.

**3.1) About Used Cars Business**

A used car, a pre-owned vehicle, or a secondhand car, is a vehicle that has previously had one or more retail owners. Established in 1898, the Empire State Motor Wagon Company in Catskill, New York was one of the first American used car lots. Used Car busines is multi billion dollar industry, there is a huge market outside of USA too.

Used cars are sold through a variety of outlets, including franchise and independent car dealers, rental car companies, buy here pay here dealerships, leasing offices, auctions, and private party sales. Some car retailers offer no-haggle prices, certified used cars, and extended service plans or warranties.

The growth of the Internet has fueled the availability of information on the prices of used cars. This information was once only available in trade publications that dealers had access to. There are now numerous sources, such as online appraisal tools and internet classified ads, for used car pricing.

**3.2) AI/ML Based Price recommendation / prediction System**

In this highly competitive age, creation of a Price recommendation/prediction System based on sales data from 1909 to 2014 would be very useful for clients in setting up price for end consumers to achieve substantial growth in sale.
The recommendation system is based on a regression model which is trained on clean data with relavent features and it should have maximum accuracy in predicting prices.

**3.3) Technical Landscape of the Solution**

In the recommendation system, we are leveraging Python ML models together with Scikit-Learn Python library, which is most used accros the industry. The data mining decisions will be made based on modeling and analysis.
Visualization will add more user friendly representation of the outcomes and help understand the predictive model recommendation for non-technical business users.

### 4) Data Understanding

After considering the business understanding, we want to get familiar with our data. Write down some steps that you would take to get to know the dataset and identify any quality issues within. Take time to get to know the dataset and explore what information it contains and how this could be used to inform your business understanding.

**4.1) Data Source**

This data comes to us from dataset from kaggle. The original dataset contained information on 3 million used cars. The provided dataset contains information on 426K cars to ensure speed of processing.

**4.2) Data Overveiw**

Using basis Python imports / libraries to import data from the csv file and do some basic lookup and analysis. More detail analysis is provided in the code file.

### 5) Data Preparation

After our initial exploration and fine tuning of the business understanding, we construct our final dataset prior to modeling. Here, we want to make sure to handle any integrity issues and cleaning, the engineering of new features, any transformations that we believe should happen (scaling, logarithms, normalization, etc.), and general preparation for modeling with sklearn. This includes: 

5.1) Cleaning data
5.2) Data Visualization
5.3) Transformation
5.4) Correlation Heatmap for Clean Used Cars Dataset & Encoded Dataset

### 6) Modeling

With our final dataset in hand, it is now time to build some models. Here, wee build a number of different regression models with the price as the target. In building models, you explore different parameters and be sure to cross-validate your findings. This includes:

6.1) Data Preparation for Modeling: Spliting dataset into Training ser and Test set
6.2) Regression Models


### 7) Evaluation

With some modeling accomplished, we aim to reflect on what we identify as a high quality model and what we are able to learn from this. We review our business objective and explore how well we can provide meaningful insight on drivers of used car prices. Goal now is to distill our findings and determine whether the earlier phases need revisitation and adjustment or if we have information of value to bring back to our client. This includes:

7.1) Prediction vs Actual Comparasion
7.2)-7.5) Prediction and Comparasion with Actuals: with different random samples: I used samples of size 5, 10, 20 and 50

### 8)Deployment

Now that we've settled on our models and findings, it is time to deliver the information to the client. We organize our work as a basic report that details our primary findings. Keeping in mind that our audience is a group of used car dealers interested in fine tuning their inventory.

### 9) Findings

Now that we've solution deployed, we are highlighting our findings based on regeression model selected. Together with I am outlining the challenges we faced throught from data import to cleansing to modeling and evaluation and deployment.
Finally, putting recommendation and further improvement in form of conclusion drwan from data analysis to modeling and evaluation.

**9.1) Key Observations**

**1) Top 5 manufacturer's cars in the used cars inventory are:**
a) Chevrolet
b) Ford
c) Honda
d) Jeep
e) Toyota

**2) Top priced used cars on an average are from these manufacturers:**
a) Ferrari
b) Jeep
c) Mercedes-benz
d) Toyota
e) Volvo

**3) Top 5 states that have maximum number of used car inventory are:**
a) California
b) Florida
c) Ohio
d) New York
e) Texas

**4) Impact of cars's age on used cars price**
a) Less old cars are more expensive in regular car segment. 
b) In vintagee cars segment, old cars are more expensive.

**5) Impact of number of cylinders in cars on used cars price**
Cars having 8 cylinders or 6 cylinders are more expensive.

**6) Impact of cars's Title classificstion on used cars price**
Clean status are sold high in number than rebuild,salvage,Lien & missing

**9.2) Data Complexities & Challenges:**
a) There were lots of null, missing or zero vaues. 
b) There were cars data in the dataset but could be related to abandoned cars, as haveee zero price. 
c) Price distribution was skewed towards left. d) Data cleansing is an important aspect to avoid rerelevant data in the analysis, for example cars those were abonded and marked as zero price.

**9.3) Conclusion & Recommendations for further improvement**
a) The selected model is approx 90% accurate, so shlould be train on more ensable regression models
b) This model is analysis was done in raw manner, it would be helpful if can be integrated as part of APP or GUI, so even non technical salesperson can input data and get projected price from model in user friendly manner wihtout too much technical details.
c) There should be continous learning / update process based on further business models to keep updating models to adopt real world challenges, negotiations, sessional discounts, inventory clearness etc, to make the prediction more robust based on other external factors.

Thank You!