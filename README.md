# What Makes a Happy Airline Passenger?

# Introduction
  By BayTech
- Warren Ngoun (wngoun@csumb.edu)
- Yukio Rivera (yrivera@csumb.edu)
- Jennah Yasin (jyasin@csumb.edu)
- Luis Jimenez Barrios (ljimenezbarrios@csumb.edu) 

---

- Why was the project undertaken? 
- What was the research question, the tested hypothesis or the purpose of the research?

We chose the Airline Passenger Satisfaction dataset for our final project because we are all interested in satisfying flight experiences and believe that it is important for airlines to take their passenger's reviews into consideration.

With this dataset, we are going to predict what factors may be most relevant and most correlated to the passenger's satisfaction. We will be analyzing which features are most correlated to our topic and dropping those that aren't as relevant/needed.

We plan to use the "satisfaction" feature as our target label for this project.
The features that we plan to use as predictors for our project are: Seat comfort, in-flight entertainment, cleanliness, and food & drinks.


# Selection of Data

What is the source of the dataset? Characteristics of data?
Any munging or feature engineering?
Source of dataset: https://www.kaggle.com/datasets/teejmahal20/airline-passenger-satisfaction
Characteristics of data:
- Gender: Gender of the passengers (Female, Male)
- Customer Type: The customer type (Loyal customer, disloyal customer)
- Age: The actual age of the passengers
- Type of Travel: Purpose of the flight of the passengers (Personal Travel, Business Travel)
- Class: Travel class in the plane of the passengers (Business, Eco, Eco Plus)
- Flight distance: The flight distance of this journey
- Inflight wifi service: Satisfaction level of the inflight wifi service (0: Not Applicable; 1-5 stars)
- Departure/Arrival time convenient: Satisfaction level of Departure/Arrival time convenient
- Ease of Online booking: Satisfaction level of online booking
- Gate location: Satisfaction level of Gate location
- Food and drink: Satisfaction level of Food and drink
- Online boarding: Satisfaction level of online boarding
- Seat comfort: Satisfaction level of Seat comfort
- Inflight entertainment: Satisfaction level of inflight entertainment
- On-board service: Satisfaction level of On-board service
- Leg room service: Satisfaction level of Leg room service
- Baggage handling: Satisfaction level of baggage handling
- Check-in service: Satisfaction level of Check-in service
- Inflight service: Satisfaction level of inflight service
- Cleanliness: Satisfaction level of Cleanliness
- Departure Delay in Minutes: Minutes delayed when departure
- Arrival Delay in Minutes: Minutes delayed when Arrival
- Satisfaction: Airline satisfaction level(Satisfaction or `0`, neutral/dissatisfied or `1`)


# Methods

- What materials/APIs/tools were used or who was included in answering the research question?

First, we gathered our data set from a Kaggle repo on Airline passenger satisfaction, it was a cleaned up data set from another Kaggle repo, but the source of the data from that repo was unknown.

Once we had the data, a lot of the pre-processing was already done, but we still had to do some work still on cleanup and encoding. After combing through the potential Classifier models and parameters, we ended up using Decision Trees and Forward Feature Selection to answer our question.

# Results

Based on our data analysis and manipulation, we were able to find the top 10 most effective features of our data set. The top 10 features were found to be: 
Online boarding
Type of Travel_Business travel
Inflight wifi service
Gate location
Baggage handling
Customer Type_disloyal Customer
Class_Business
Inflight Service
Seat comfort
Customer Type_Loyal Customer
However, from these top 10 features, we decided to use the first top 5 as our predictors since they better improved the accuracy of our model.

# Discussion

- What might the answer imply and why does it matter? How does it fit in with what other researchers have found? What are the perspectives for future research? Survey about the tools investigated for this assignment.

The answer from the project implies that Decision Trees can provide a quick and accurate prediction for customer satisfaction with air travel based on a set of predictors. This matters because it can provide airlines with valuable insights into what factors are most important for customer satisfaction and can help them prioritize their resources accordingly.
The finding that certain predictors, such as Online boarding and Inflight Wifi, are strong indicators of customer satisfaction is in line with previous research that has identified similar factors as important for customer satisfaction in the airline industry. However, the identification of the best 5 features from a larger list of 26 is a unique contribution to the field.
In terms of tools, the project investigated the use of Python libraries such as Pandas, NumPy, Scikit-learn, and Matplotlib, which are widely used in data analysis and machine learning. 

# Summary

Through analyzing the Airline Passenger Satisfaction dataset, we were able to get a better idea of:

Cleaning up data
The importance of converting categorical data into numerical values for testing
Experimenting with kNN and Decision Trees
Determining that Decision Trees were more significant for our project
Realizing how effective predictors really are in terms of calculating accuracy

Finally, we found that the most important feature in relation to the determination of passenger satisfaction is the rating of Online Boarding. This was surprising to us as other features would have been our personal preferences, like seat comfort or food and drink.  


