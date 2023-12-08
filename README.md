# module24Capston

NLP Classification Model for News Articles

By William Valentin 

Executive Summary
This study delves into the realm of Natural Language Processing (NLP) models, aiming to gauge their accuracy in classifying news articles into distinct categories. The central question is whether these models can attain a level of accuracy that renders them capable of replacing human classification. To explore this inquiry, we employ the News Category Dataset from Kaggle, encompassing various attributes for each news article, including category, headline, authors, link, short description, and publication date. The ultimate objective is to leverage the headline and short description as features to classify news articles, emulating real-world scenarios where manufacturing events require classification for trend analysis. This dataset serves as an ideal representative example due to confidentiality constraints preventing the use of actual manufacturing data.

Rationale
Understanding the potential accuracy of NLP models in classifying news articles into categories holds substantial significance. This knowledge can inform decisions regarding the feasibility of automating the classification process, potentially saving time and resources. Furthermore, it offers insights into the consistency of NLP models compared to human judgments, addressing concerns related to human assessment variability.

Research Question
The primary research question addressed in this study is: "What level of accuracy can we expect from a Natural Language Processing (NLP) model when classifying news articles into different categories, and is this level of accuracy sufficient to replace human classification?

Data Sources
The primary data source for this study is the News Category Dataset, accessible through Kaggle. This dataset encompasses a diverse range of news articles, each associated with attributes such as category, headline, authors, link, short description, and publication date.

Methodology
The methodology employed in this study revolves around utilizing NLP techniques to preprocess and analyze the text data. Initially, the headline and short description of each article are tokenized, with subsequent steps including the removal of stop words, punctuation, and capitalization, along with lemmatization. The LabelEncoder is applied to categorical labels, and TF-IDF vectorization is utilized to transform the text data into numerical features. Various machine learning models, including Random Forest, Logistic Regression, Decision Tree, Multinomial Naive Bayes, and Ensemble methods, are explored to classify news articles into categories. Model performance is assessed using metrics such as accuracy, precision, recall, and F1-score.

Results
The study commenced by utilizing the headline as the primary input feature and evaluating several models, including Random Forest, Decision Tree, and Neural Network. Unfortunately, the inclusion of the Support Vector Classifier (SVC) model was impractical due to its extensive runtime, exceeding 15 hours. Notably, both the Random Forest and Decision Tree models displayed signs of overfitting, characterized by high training accuracy but consistently low test accuracy (below 60%). An attempt to enhance performance by incorporating the "short_description" feature did not yield improved results compared to using only the headline as input. Subsequently, the study proceeded to create a novel feature by combining the text from both the headline and short_description, consolidating them into a single column labeled "all text." This novel feature became the focal point for the final modeling phase. Among the diverse modeling approaches explored, logistic regression emerged as the top-performing model for this dataset, achieving an accuracy rate of 0.76. It consistently demonstrated robust performance in terms of accuracy, precision, and recall, all while maintaining an acceptable runtime.

Next Steps
The future steps in this study involve exploring additional modeling strategies beyond those initially considered, addressing the issue of low precision for specific categories, reducing the dataset size to facilitate quicker experimentation, and fine-tuning models to enhance their performance. Moreover, the study aims to investigate the feasibility of applying the Support Vector Classifier (SVC) model, which was excluded due to its extended runtime. Scaling up the study to larger datasets and further refining feature engineering techniques are also on the agenda. The ultimate goal is to develop a robust and accurate model for the News Category Dataset, building on the insights gained during this preliminary analysis. Achieving an accuracy rate of 0.76 represents a promising starting point, given the dataset's complexity and the initial models' performance below 60%. Additionally, the study will continue to assess cases where the model outperforms human judgments, highlighting potential inconsistencies in human assessment practices.

Outline of Project
Introduction
Rationale
Research Question
Data Sources
Methodology
Results
Next Steps
Conclusion
Notebook Experiments:
Notebook Final: William Valentin Capstone Experiments.ipynb

Contact Information 
William Valentin
william_valentin@hotmail.com
