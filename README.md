# Analytics_vidhya_Hackathon_05_May

This code was written for Hackathon in Analytics Vidhya.

Approach is explained below:

> Initially I read the data and check for null values. There were null values at Products purchased and Signup date.
> Products purchased data's null values was replaced with 0. Signup_date was replaced with Created_at date.
> A feature was created with the difference of Signup_date and Created_at. And then both rows were dropped.
> The new created feature above had both negative, positive and Zero values. It was important to have diversity in this column for our final model.
> Then random forest classifier was called and data was trained with 80% train and tested on rest of it.
> Accuracy obtained was 97.52% but it is of no use as the data is imbalanced.
> F1 score was calculated on Test data and it came to be 0.7329.
> Model was fitted on Test Data and final results were published.

Note:
> Though, the data was imbalanced, no technique was used to make it balanced.
> No imputation method was used to fill null values, this was because the columns with null values are important features and cannot be imputed with any information.

Scope for Improvement:
> I could have worked on finding Correlation between features and thus reduced featured from 16 to 12-13. This was not done earlier because I had used all 40k data points for my model.
> For imbalanced dataset, I could have done Smoting which might give more accuracy and F1 score above 0.80. 
