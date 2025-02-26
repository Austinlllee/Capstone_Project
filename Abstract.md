# Capstone_Project
# Analyzing the Impact of Donald Trump's Tweets on the Stock Prices of Major Tech Companies

## Background/Context
Social media platforms, particularly Twitter, have become essential tools for public figures like Donald Trump to communicate directly with the public. His tweets have garnered significant attention for their potential to influence stock market fluctuations. This study will explore how the sentiment in Trump's tweets correlates with stock price movements of major tech companies such as Amazon, Apple, Facebook, and Google.

## Objective/Research Question
This study aims to determine if the sentiment expressed in Donald Trump's tweets—manually classified as positive, neutral, or negative (1, 0, -1)—has any influence on the stock prices of Amazon, Apple, Facebook, and Google.

## Methods
The data for this analysis is sourced from two main components: Twitter data and stock price data. The tweets were collected using a custom script that loads data from JSON files for each company (Amazon, Apple, Facebook, Google) using the `jsonlite` package in R. Each tweet is manually classified into three sentiment categories—positive, negative, or neutral—and then aggregated weekly.

For stock prices, historical weekly data for each of the selected tech companies was retrieved using the `tidyquant` package and processed to compute the average weekly stock prices for Amazon, Apple, Facebook, and Google. The sentiment scores are then merged with stock data on a weekly basis for further analysis.

Correlation and Granger Causality tests will be employed to explore the relationship between tweet sentiment and stock price movements. A Vector AutoRegression (VAR) model will be used to forecast stock prices based on sentiment trends.
