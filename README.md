# Customer_Conversion_Audiobook_App
## Problem statement
  Can we predict which customers will convert? if yes, it will help the company's marketing team in target ads to consolidate and possible increase the conversion rate     with target ads and possible insentives.

## Data gathering process:
  Data was gathered from the audiobook app, and it represents 2 years and 6 months’ worth of engagement on the audiobook app, we will take an additional 6 months after     the 2 years to check for conversion as we are going to assume that if a user does not return after 6 months, they might never return.

## Features
  1.	ID: equivalent to customers names, hence it is not relevant to our model training
  2.	Book Length(mins)_overall: Sum of the length of all purchases
  3.	Book Length(mins)_avg: sum divided by all purchases
  4.	Price_overall: sum paid for all purchases
  5.	Price_avg: average sum paid, i.e. overall price divided by number of audiobooks purchased
  6.	Review: Boolean, if the customer left a review; shows if there was engagement with the platform.
  7.	Review 10/10: the review left, most people don’t leave a review, so null values will be substituted with the average; 8.91
  8.	Minutes Listened: Measure of engagement
  9.	Completion: total mins listened divided by the length of the books
  10.	Support Requests: total number of support requests the user opened; it is a measure of engagements
  11.	Last visited minus Purchase date: difference between the last time the person visited and the first time they visited, hence the bigger the value the better.
  12.	Targets: if the customer converted within 6 months

## Approach:
  1.	Preprocess the data
  a.	Balance the dataset
  b.	Divide the dataset into training, validation and test to prevent overfitting
  c.	Save the data in a tensor friendly format. i.e. npz
  2.	Create a class that handles batching.
  3.	Create the machine learning algorithm artificial neural network.

