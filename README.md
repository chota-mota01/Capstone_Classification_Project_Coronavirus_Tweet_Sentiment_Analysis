# Capstone_Classification_Project - Coronavirus_Tweet_Sentiment_Analysis

The given dataset comprises tweets sourced from Twitter, which have undergone manual sentiment tagging.The primary objective is to leverage machine learning techniques to accurately classify the sentiment conveyed in COVID-19 tweets.

# Problem Statement

The project entails the development of a classification model aimed at predicting the sentiment expressed in COVID-19-related tweets. The dataset comprises tweets sourced from Twitter, which have undergone manual sentiment tagging. To ensure privacy protection, both names and usernames have been anonymized through encoding.

The primary objective is to leverage machine learning techniques to accurately classify the sentiment conveyed in COVID-19 tweets. By building and deploying a robust classification model, we aim to gain insights into public sentiment surrounding the pandemic, enabling organizations to better understand public perception, sentiment trends, and potential areas of concern or positivity. Through this analysis, we seek to contribute to a deeper understanding of the public discourse surrounding COVID-19 on social media platforms.

# Dataset Information

The given dataset contains the coronavirus tweet information. The variables are described as follows:

**Username** **-** Unique user-IDs

**ScreenName** **-**  Unique screen name of the user

**Location** **-** Location of the user

**TweetAt** **-** Date of the tweet

**OriginalTweet** **-** The real tweet

**Sentiment** **-** Sentiment of the tweet

# Data Cleaning and Manipulation 

1.Handling Null & Duplicate Values

* The given dataset contains numerous null values.
* Null values in location were replaced by not specified.
 
2.Converting Datatypes

* Converted column TweetAt to datetime data type.


# Exploratory Data Analysis 

The data visualization is performed using mainly seaborn & matplotlib library. These visualizations helped to simplify complex data and make it more understandable. For visualization, the following charts are used:

Count plot

Bar Graph

Histplot

Line chart

Box plot

Correlation Heatmap

Pair Plot

# Prediction Analysis

For sentiment analysis, we explored five machine learning models, including Logistic Regression, Naive Bayes Classifier, Random Forest, KNN(K-Nearest Neighbors), and Decision Tree. The accuracy score and classification report are crucial metrics influencing analysis. They offer insights into a model's performance and its ability to correctly classify instances, aiding in real-world applications.

1. Logistic Regression

Logistic Regression is a statistical method used for binary classification tasks, where the outcome variable or target variable is categorical and has only two possible outcomes. It is a type of regression analysis that models the probability of a binary outcome by fitting the data to a logistic function.

2. Naive Bayes Classifier

Naive Bayes Classifier is a probabilistic machine learning model based on Bayes' theorem with an assumption of independence among features. It is commonly used for classification tasks, particularly in text classification and spam filtering. Naive Bayes Classifier remains a popular choice for classification tasks, especially in scenarios where the assumption holds reasonably well and computational efficiency is important.

3. Random Forest Classifier

Random Forest Classifier is a popular ensemble learning algorithm that combines the power of multiple decision trees to make predictions. Random Forest Classifier is widely used in various machine learning applications, including classification, regression, and anomaly detection. It is known for its robustness, accuracy, and ease of use, making it a popular choice among practitioners and researchers. Proper tuning of hyperparameters such as the number of trees and maximum depth of trees is important for optimizing the performance of Random Forest models.

4. K-Nearest Neighbors
 
KNN is a versatile algorithm with various applications, including classification, regression, clustering, and outlier detection. It is particularly useful when the decision boundary is nonlinear or when the underlying data distribution is unknown. However, it may not perform well with high-dimensional data or imbalanced datasets. Proper preprocessing, feature scaling, and tuning of hyperparameters are essential for maximizing the performance of KNN.

5. Decision Tree
 
The Decision Tree Classifier algorithm builds a predictive model in the form of a tree structure. Each internal node in the tree represents a decision based on a feature, and each leaf node represents a class label or a decision. The algorithm partitions the feature space into regions, with each region corresponding to a leaf node in the tree. Decision trees are trained using a recursive partitioning algorithm that selects the best feature and split point at each node based on criteria such as Gini impurity or entropy.

# Evaluation Metrics

The accuracy score and classification report are vital metrics that can greatly influence business decisions and outcomes. By accurately assessing the performance of a classification model, businesses can make informed decisions regarding various aspects of their operations. For instance, a high accuracy score and a detailed classification report provide valuable insights into the model's ability to correctly classify instances, helping businesses gauge the effectiveness of their predictive models in real-world scenarios.

# Conclusion

The primary objective is to leverage machine learning techniques to accurately classify the sentiment conveyed in COVID-19 tweets. We focused our analysis solely on the "OriginalTweet" and "Sentiment" columns, as columns like "UserName" and "ScreenName" do not provide meaningful insights for our analysis. These two columns contain the primary data we need to analyze sentiments expressed in the tweets, thereby streamlining our data processing and analysis pipeline. We used stemming and lemmatizing for text normalization.

In our analysis of COVID-19 tweets, we explored five machine learning models, including Logistic Regression, Naive Bayes Classifier, Random Forest, KNN, and Decision Tree. Despite implementing grid search cross-validation to optimize the models, we did not observe significant improvements in the test accuracy across all models.

However, the Logistic Regression model with Grid Search CV and count vectorization stood out, achieving an accuracy of 79.51%. This model demonstrated robust performance without signs of overfitting, indicating its suitability for deployment.

Our analysis revealed that despite the challenging circumstances of the COVID-19 pandemic, positive sentiments outweighed negative ones in the tweets. Nonetheless, a substantial portion of negative sentiments persists, presenting opportunities for government agencies, NGOs, and other entities to implement initiatives aimed at boosting public morale and addressing concerns.

Looking ahead, repeating the analysis in the future and comparing it with the present sentiment analysis could provide valuable insights into the effectiveness of such initiatives over time. This iterative approach allows for ongoing assessment and adjustment of strategies to better address evolving sentiments and needs during unprecedented situations like the COVID-19 pandemic.
