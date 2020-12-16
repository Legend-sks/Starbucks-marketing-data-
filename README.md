# Capstone-Project-Starbucks
This is Capstone Project for Udacity Data Scientist Nano Degree Program. 

## Project Overview
This Capstone Project is done as part of final delivarable to Udacities Data Scientist Nano Degree Program. Project choosen for this is the "Starbucks Project". This is a  classification problem which can help Starbucks to optimize app offers for their customers. it very crucial to identify right customers and send them just the write offer to maximize the customer value for company and at the same time provide the offer that best suits the customer. A customer will react to an offer based on various individual traits. Here I will analyze the dataset provided by Starbucks and try to answer few problems using model and visualization.

## Problem Statement:
I want to answer below two questions in this analysis:
1. What offers to send a customer, so that the chances of offer getting completed is high?
  I will address this problem with a model. The model will be able to predict that if an offer is sent to a customers will it be completed or not. (Definition of complete is shared below).
2. Set of heuristics that determine what offer should be sent to group of customers?
  This problem will be address using visualizations and exploratory analysis.
  
## Evaluation Metrics
For model evaluaiton, I will be using f1-score metric to assess models performance. We will also measure accuracy of the model on test data to see how well our model predicts if the offer is successfull or not.

## Dataset Introduction
Starbucks has provided a simulated dataset that contains details about customer, offers and transactions. Each person in the simulation has some hidden traits that influence their purchasing patterns and are associated with their observable traits. People produce various events, including receiving offers, opening offers, and making purchases. There are three types of offers that can be sent: buy-one-get-one (BOGO), discount, and informational. In a BOGO offer, a user needs to spend a certain amount to get a reward equal to that threshold amount. In a discount, a user gains a reward equal to a fraction of the amount spent. In an informational offer, there is no reward, but neither is there a requisite amount that the user is expected to spend. Offers can be delivered via multiple channels. 

### Data Dictionary:

1. profile.json :Rewards program users (17000 users x 5 fields)
gender: (categorical) M, F, O, or null
age: (numeric) missing value encoded as 118
id: (string/hash)
became_member_on: (date) format YYYYMMDD
income: (numeric)

2. portfolio.json : Offers sent during 30-day test period (10 offers x 6 fields)
reward: (numeric) money awarded for the amount spent
channels: (list) web, email, mobile, social
difficulty: (numeric) money required to be spent to receive reward
duration: (numeric) time for offer to be open, in days
offer_type: (string) bogo, discount, informational
id: (string/hash)

3. transcript.json : Event log (306648 events x 4 fields)
person: (string/hash)
event: (string) offer received, offer viewed, transaction, offer completed
value: (dictionary) different values depending on event type
offer id: (string/hash) not associated with any "transaction"
amount: (numeric) money spent in "transaction"
reward: (numeric) money gained from "offer completed"
time: (numeric) hours after start of test






























