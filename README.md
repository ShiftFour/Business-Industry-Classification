# Business-Industry-Classification
# Project Objectives & Background
Industry code is one of key features of a prospective client and is used for many marketing and upsell models. Prospective client price points, service needs, and products all vary based on their industry sector, but reliable industry classifications can be difficult to come by. 

The goal of this project is to design an ethical web scraper to glean industry related text information off business websites and build an NLP model that can accurately classify a company’s industry based on keywords found on the company’s public website.

The techniques we will need are web crawler and machine learning. We will use web crawlers to get information from public websites and use machine learning, especially the NLP model to do the prediction of classification of company industry.

# Basic Workflow and Algorithms:
Core Algorithms: In order to compare the similarity of two text-based content (candidate profile and job description), we need to clean the original dataset (seperate words and remove useless words), vectorize core features (transfor from text to numerical data) and project the vector to pre-defined recruiting matrix (recruiting maxtrix that contains all features we need to evaluate). Finally, calculate cosine similarity between features and select candidate with high number.
Basic Workflow:
1.	Web crawling to collect data from companys’ public websites as input
2.	Build a data pipeline for data transformation (including feature extraction) and machine learning
3.	Data preprocessing and Data wrangling

4.	Data split - Use train-split / k-fold crsoss validation 
5.	Use OneVsRestClassifier to solve multi-label data by wrapping these algorithms like LinearSVM or Naive Bayes.
    
    •	Tf-Idf vectorizer to convert the string in to numeric value - have appropriate parameters set.

    •	english stop_words from english Corpus
    
    •	Parameter tunning through GridSearchCV
    
6.	Model Evaluation
    
    •	calculate cosine similarity between features and select candidate with high number.


