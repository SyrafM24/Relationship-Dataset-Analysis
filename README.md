# Cyberbullying Data analysis and visualisaiton

## Description
This was a group project I did in the module Intro to Data science and AI where we took a dataset from kaggle and analyzed the trends and predict whether a person is in a relationship or not. Using Python, we visualised the data using NumPY and Pandas to understand the trends of each variable. We then took the variables and analyzed which affects the variable "Relationship status" as the prediction and "Mental_Health_Score", "Sleep_Hours_Per_Night", "Avg_Daily_Usage_Hours" as their predictors.

## My Role
I used a Multivariate logistic Regression with ordinal encoder and attempted One-Hot Vector on the variable relationship status as it was a binary input variable "In relationship", "Complicated" and "Single" against thhe predictors. This analysed whether a student is n a relationship based on other patterns

## Tools Used
- Jupyter
- Python (NumPy and Pandas)

## Dataset used
https://www.kaggle.com/code/adilshamim8/social-media-addiction-among-students/notebook 

## Data Visualisation
Using Pandas, I made a table to see the overall details of the dataset. I saw that complicated had a very low sample count and decided to remove that variable because it might affect the results.
<img width="1107" height="374" alt="Screenshot 2026-04-25 210246" src="https://github.com/user-attachments/assets/d3eb2c90-b6f7-4e59-8e91-e7307d3039f4" />
<img width="495" height="504" alt="Screenshot 2026-04-25 212113" src="https://github.com/user-attachments/assets/9018b2a2-c800-446f-ab6b-c8ab917f6e4d" />

## Data Cleaning
In order to "clean" the data, I used the "cat.remove_categories[]" to remove the complicated variable. After removing the variable, I used sb module to display the bar graph
<img width="493" height="505" alt="Screenshot 2026-04-25 212129" src="https://github.com/user-attachments/assets/33da2812-aa9c-47da-84aa-48bfaba1655f" />

## Data Analysis
I used Logistical regression with the use of classification report instead of R^2 and Mean Squared error due to the categorical prediction. From there I developed the prediction and see the trends.
<img width="396" height="147" alt="Screenshot 2026-04-25 212206" src="https://github.com/user-attachments/assets/b8e5c5d6-51fd-44c3-b7ee-9607a8f109c7" />

In the classification report, it shows how strong the model predicts between 1(single), 0(In Relationship)

## Conclusion
In conclusion, from the report we can infer that,
- The model is more biased in predicting single than In relationship. As we can see the recall is described as how correctly the model has predicted
- The 2 categories where 94% of single were predicted correct with the "Mental_Health_Score", "Sleep_Hours_Per_Night", "Avg_Daily_Usage_Hours".
- While those in relationship, the "Mental_Health_Score", "Sleep_Hours_Per_Night", "Avg_Daily_Usage_Hours"  Could only be predicted correct 11% of the time.


This can be affected by outside factors where relationship situations matters. For example, some relationshops are more low maintenenace which could be more sleep and  less usage of internet, while the other way also. While singles, they may have outside factors but their prediciton is relatively accurate. Hence, This model can be used to estimate single people patterns in terms of social media addiction better while relationship is a bit mroe difficult due to their outside factors.
