# module24Capston
Capstone Machine Learning Course Final Project
NLP Classification Model for News Articles

Introduction:
What level of accuracy can we expect from a Natural Language Processing (NLP) model when classifying news articles into different categories? Is this level of accuracy sufficient to replace human classification? In this study, we explore the capabilities of NLP models using a selected dataset from Kaggle, the News Category Dataset. This dataset contains various attributes for each news article, including the category, headline, authors, link, short description, and publication date. The goal is to classify news articles into their respective categories using the headline and short description as features, simulating a real-world scenario where manufacturing events are classified for trending analysis. Due to confidentiality constraints, real manufacturing data cannot be used, making this dataset an ideal representative example.

Dataset Overview:
The News Category Dataset consists of news articles with the following attributes:

Category: The category in which the article was published.
Headline: The headline of the news article.
Authors: A list of authors who contributed to the article.
Link: A link to the original news article.
Short Description: An abstract of the news article.
Date: The publication date of the article.
Modeling Strategies:
This project explores various modeling strategies, including Random Forest, Logistic Regression, Decision Tree, Multinomial Naive Bayes, and Ensemble methods and consists of two Juptiper notebook files.

Conclusion:
The study began by using the headline as the primary input feature and evaluated several models, including Random Forest, Decision Tree, and Neural Network. Unfortunately, the inclusion of the Support Vector 
Classifier (SVC) model was impractical due to its extensive runtime, exceeding 15 hours. Notably, both the Random Forest and Decision Tree models displayed signs of overfitting, characterized by high training 
accuracy but consistently low test accuracy (below 60%). An attempt to enhance performance by incorporating the "short_description" feature did not yield improved results compared to using only the headline as input.
Subsequently, the study proceeded to create a novel feature by combining the text from both the headline and short_description, consolidating them into a single column labeled "all text." This novel feature 
became the focal point for the final modeling phase. Among the diverse modeling approaches explored, logistic regression emerged as the top-performing model for this dataset, achieving an accuracy rate of 0.76.
It consistently demonstrated robust performance in terms of accuracy, precision, and recall, all while maintaining an acceptable runtime. Resource limitations constrained further exploration of new models. 
Therefore, the next step in this study involves an investigation into the SVC model, initially omitted due to its prolonged execution time. Moving forward, the applicability of this technique to real-world scenarios 
appears promising, given that the dataset size is significantly smaller than the 200k records available for this exercise. It is essential to note that an accuracy rate of 0.76, while seemingly modest for replacing 
human judgment in record classification, represents a noteworthy improvement. This is particularly significant when considering that the initial models began with accuracy rates below 60%. Moreover, upon reviewing 
records where the model failed during testing, it became apparent that the model's predictions were often more accurate than human judgments, underscoring the inconsistency in human assessment.Future steps include 
exploring additional modeling strategies, addressing low precision for specific categories, reducing the dataset size for quicker experimentation, and fine-tuning models for improved performance. The ultimate goal
is to build a robust and accurate model for the News Category Dataset, leveraging the insights gained from this initial analysis.
