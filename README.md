# EDA_on_Marketing-Data
# Observation: 
1 Our dataset do not have any null/nan/missing values.
2 Our dataset is highly imbalanced.
3 The attribute pdays seems to be important feature as there is a clear distinction in quartile ranges of pdays for target variable yes and no. 
4 75% clients contacted through campaign are not previously contacted.
5 Mean of pdays is 40.20 There are outliers as we can see from boxplot.
6 The attribute duration seems to be important feature as there is a clear distinction in quartile ranges of duration for target variable yes and no. 
7 75% call duration are less than or equal to 5.32 duration have a mean of 4.30 and standard-deviation 4.29.
8 There are outliers points in duration.
9 75% of previous values equal 0 and 99% values <= 8.90 duration have a mean of 0.58 and standard-deviation 2.30 There are outliers points in duration.
10 People with age < 30 or 60+ have higher success rate. 
11 Only 3% of clients have age of 60+.
12 Top contacted clients are from job type: 'blue-collar', 'management' & 'technician'.
13 Success rate is highest for student.
14 Most of the clients contacted have previous outcome as 'unknown'.
15 Most of the people who are contacted have tertiray or secondary education.
16 Very few clients are contacted who are defaulter.
17 As seen for default variable, less client are contacted who have loan.
18 Most of the people are contacted through cellular.
19 Most of the clients (approx 1/3 of total) are contacted in the month of May but the success rate is only 6.7%. 
20 March have highest success rate.
21 For most of the variables our pair plot is overlapping a lot. Pair plots of age-campaign and day-campaign are much efficient in distinguishing between different   classes with very few overlapes.
22 Over numerical features have very less correlation between them. 
23 pdays and previous have higher correlation duration have a higher correlation with our target variable.

# Conclusion:
Our dataset consist of categorical and numerical features. 
We have 16 independent features, out of these only half of them are important.'duration' is the most important feature while 'education' is the least important feature. 
Month of May have seen the highest number of clients contacted but have the least success rate. 
Highest success rate is observed for end month of the financial year as well as the calendar year. So one can say that our dataset have some kind of seasonality. When visualized age in groups, it is found that clients with age less than 30 and greater than 60 are less contacted through the campaign but have a higher success rate. 
Different machine learning models are trained and tested on the dataset. Out of those Voting Classifier performs best. Logistic Regression is also an important model as it results in high AUC score.
