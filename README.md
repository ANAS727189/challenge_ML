# challenge_ML
Overview
A data collection firm gathered information on housing prices across different locations. However, upon analysis, they discovered that the dataset they compiled was not clean. Now they need your help with cleaning this housing dataset to facilitate subsequent analysis or predictive modeling, aiming to support the firm in making more informed decisions. The dataset encompasses a diverse set of features related to housing properties, such as price, area, number of bedrooms, bathrooms, stories, and a binary indicator to determine whether the house is situated near the main road.


Participants must perform the following data tasks :

Price Range Filtering: The dataset includes house prices, but some values are outside the realistic range for this dataset (1750000 to 13300000). Participants need to filter out entries that fall outside this price range.

Handling Missing Values: The dataset contains missing values (NaNs) across various columns. Participants are required to identify and remove rows with any missing values.

Removing Rows with Negative Values: Some rows in the dataset have negative values in numerical columns (except for the 'mainroad' column). These rows need to be identified and removed as they represent incorrect data.

Correcting Main Road Category: The 'mainroad' column is a categorical feature represented by 0 and 1. Any row with a value in the 'mainroad' column outside of these two categories should be corrected to 0 by default.

Keep in mind!!! There can be a scenario when the negative value or the null value is only present in the mainroad column. What do you do then? Do you drop the whole column or do you set it to default value?

And make prompt visualizations which can help the firm draw conclusions in any way.

Submission
Only the correct submission will get accepted and any errors or issues with the cleaned data in your notebook will be prompted to you after submission error
To make your submission, once you have completed all the cleaning and exploration objectives ,sort the datset in descending order based on price(do it on your own) and simply copy the below code to export the dataset into a csv file named submission.csv
For your convenience you can use this code below :

data.to_csv('/kaggle/working/submission.csv', index=False)
