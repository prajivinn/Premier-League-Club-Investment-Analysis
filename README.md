# Premier-League-Club-Investment-Analysis

Project_link: https://prajivinn.github.io/2023/05/15/Premier-League-Club-Investment-Analysis.html

## Context:

An investment company aims to invest in one of the top-performing club in the English Premier League. To aid in their decision-making process, the analytics department has been tasked with creating a comprehensive report on the performance of various clubs. However, some of the more established clubs have already been owned by the competitors. As a result, Company ABC wishes to identify the clubs they can approach and potentially invest to ensure a successful and profitable deal.

Data: Premier League Final Data.csv- : The data set contains information on all the teams so far participated in all the premier league tournaments.

## Data Dictionary:

* Club: Name of the football club
* Matches: Number of matches the club has played in the Premier League
* Wins: Number of matches won by the club in the Premier League
* Loss: Number of matches lost by the club in the Premier League
* Goals: Number of goals scored by the player in the Premier League
* Draws: Number of matches drawn by the club in the Premier League
* Clean Sheets: Number of matches in which the club has prevented the opposing side from scoring
* Team Launch: Year in which the club was founded
* Winners: Number of times the club has won the Premier League
* Runners-up: Number of times the club has finished as runners-up in the Premier League
* Project Objective

## Actions

We collected the data of all the clubs from premierleague.com

We undertook data cleaning on the dataset to replace null values as well as dealing with incorrect data on the columns.

We performed EDA on the data starting from identification of outliers using .describe method in each column with respect to the measures of dispersion i.e using Mean and Median. As per the project requirements, the more established clubs meaning clubs with high experience have already been owned by the competitors. Using Histogram, we identifed and removed those most established clubs( established clubs = higher experience/ high number of matches played) becasue it will skew our results in finding the potential club.

Since it is a cumulative data, It is essential to understand that the values in all the columns represent the cumulative scores over all the “matches played” . So we normalized the data by dividing the no. of wins, loss, drawn, clean sheet, goals by the number of matches played column.

With the help of box plot, we plotted the winning rate, loss rate, drawn rate, clean sheet rate. By visualizing it, we found outliers in Winning rate column. It is safe to say that these outlier clubs have exceptionally higher winning rate which can be a potential club to look on further. We also found the club with least winning rate so that we don’t want to provide wrong suggestions to the client at the end of analysis.

A potential club can be a club with a high winning rate ( or ) a club with high winning rate & high drawn rate meaning the club/team is able to stand up strong & ensure not loosing. They are winning or they are making sure its a “Draw”. Also a Club/team with low Loss rate and high drawn rate is a good combination. Following, we identified the clubs with high winning rate, low winning rate, high drawn rate and also the clubs who are currently playing in the premier league(2023).

Based on a recommendation framework, We created a score column which gives weightage/points to each club upto a total of 100 points per club. We gave more weightage/points to clubs who has/is:

High Winning Rate
Won the premier league
Currently playing in the premier league 2023
Finally with the help of Bar Chart, we plotted the clubs with their respective “Scores”.


## Results

The club which has highest score is **Leicester City**. Given this information, we recommend that stakeholders consider investing in Leicester City instead. We believe that Leicester City’s recent form and performance make them a better choice for investment.

**To support our claim, we conducted further secondary research to provide additional evidence of Leicester City’s current form and potential for success**


## Growth/Next Steps

Since it is an investment decision, the Price would need to be in the equation too.

We could discuss with client about their budget. Based on their budget, we could filter the teams.

From the data point of view, we can try to collect each team’s price/value to ensure that we have as much useful information available in making the final decision.

## Key learning after this project:

* Data cleaning is the process of identifying and correcting or removing errors, inconsistencies, and inaccuracies in a dataset.
* Observation writing involves examining the data and noting any notable findings, anomalies, or areas of interest.
* Exploratory Data Analysis (EDA) is the process of examining and visualizing a dataset to understand its main characteristics, such as the distribution of data, the relationships between variables, and any anomalies or patterns that may exist. The goal of EDA is to uncover insights and trends that can help inform further analysis or decision-making. It is often the first step in any data analysis project, as it provides a foundation for more advanced statistical methods and models.
* Treat Null values basis domain knowledge aka using Domain-specific imputation.
