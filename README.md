# Starbucks-Project

# Introduction

Blog Post Report for this project present:
      https://medium.com/@nicotacor/starbucks-offer-study-1e74041774e0

## Installation

- NumPy

- Pandas

- Seaborn

- Matplotlib

- Sklearn


## File Descriptions
This repo contains 4 files.There is a notebook available here to showcase work related to the above questions and wrangling process. There are 3 data files used to address the above qustions

portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
profile.json - demographic data for each customer
transcript.json - records for transactions, offers received, offers viewed, and offers completed

## Important: unzip files from the "data" folder

## Results: 

- First of all, we saw that BOGO offers were highly demanding, the percentage of BOGO Offer viewer was 83 percent . The percentage of DISCOUNT Offer viewer was 70 percent.

- For gender predict: We can see that the model is not perfect, because the predicted genders are generally Male (almost 90%). However, given the few variables at the start, the result is not so bad, but we can ask ourselves if the low representation of women in the starting base is not the cause of this. 

- The events are wrongly predicted as 'offer received'. 

- Majority classes are performing well but the minorities are not. This is cause because of a problem of imbalanced dataset. 

- Most of the events are wrongly predicted as 'offer received'; offer received is the most occuring event or class.

- With this we can see that the precision method is not the most suitable for this data set, due to how unbalanced it is. It's important to say that I originally was going to only use the F₂ Score, but I realized I needed to look at multiple metrics to get a full picture. I discovered that on some models the F₂ Score was really high (~0.90), but the model marked everything as Positive (i.e. send the offer). This resulted in all TP and FP and no TN and FN.

- We obtained a solid solution for the problem, as we commented in the Model Evaluation and Validation section. There were only 13 % of false positive i.e the customer did not accept the offer but was predicted as success and 5% of false negatives.

## Conclusion

We got solve the basic tasks in this project: identify which groups of people are most responsive to each type of offer, and how best to present each type of offer. 

The results shows that the model identifies 13 % of false positive i.e the customer did not accept the offer but was predicted as success and 5% of false negatives i.e customer accepted the offer but was predicted as fail.

However, the data provided, namely offer characteristics and user demographics could not predict whether a user would take up an offer. We had got an imbalanced dataset. This was the higher difficulty I had studying this datasets. To try to solve this problem, the dataset should be balance and should has more data. Also, for improve results we can:

 - The accuracy could be improved significantly usingdeep neural networks, or using recommendation engines. 

 - Also, removing some custom features from the dataset and evaluating the model would be interesting.
 
 - Concerning feature engineering, there could be features developed regarding how much the customer has spent before viewing offers.

From the result of the project, it's likely to use machine learning model to predict whether the customer will respond to the offer or not, and the model also shows the main factors such as the length of membership, age, income which highly affect the possibility of customer's responding to the offer. This was very useful to respond: what features influence the effectiveness of an offer on the Starbucks app?
