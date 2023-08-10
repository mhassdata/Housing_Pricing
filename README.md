# Housing_Pricing

In this notebook, I conducted Exploratory Data Analysis (EDA) to examine the relationship between dataset features and SalePrice. I identified detrimental features for our model by flagging those with high class imbalance, low correlation with SalePrice, and significant skewness among continuous numerical features.

Subsequently, I performed data cleaning, excluding flagged features and those with excessive missing values. For partially missing features, I implemented target encoding using mean or mode for numerical and categorical features respectively. Additionally, I removed outliers from the train dataset to prevent negative influence on our model.

Following data cleaning, I engaged in feature engineering, utilizing one-hot encoding for categorical features and filling test dataset gaps with zeros to maintain shape post-encoding. To ensure model consistency, I performed a train-test split over 100 iterations, computing metrics for the linear regression model. This validation reinforced our progress.

Finally, I constructed a Random Forest model using the train dataset and generated SalePrice predictions for the test dataset. 

To summarize, our refined process involves dropping problematic features,  addressing missing values, encoding categorical variables, and validating model stability through iterative train-test splits. These steps collectively form an effective framework for analyzing and predicting SalePrice in this dataset.
