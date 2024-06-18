TEAM NAME: COEUS

TEAM MEMBERS
Wanjiru Kinyara 
Ezra Mageto
Daniel Musili
Ann Mberi - TL

PROBLEM STATEMENT.
Swahili is spoken by 100-150 million people across East Africa. In Tanzania, it is one of two national languages (the other is English) and it is the official language of instruction in all schools. News in Swahili is an important part of the media sphere in Tanzania.
News contributes to education, technology, and the economic growth of a country, and news in local languages plays an important cultural role in many Africa countries. In the modern age, African languages in news and other spheres are at risk of being lost as English becomes the dominant language in online spaces.
The Swahili news dataset was created to reduce the gap of using the Swahili language to create NLP technologies and help AI practitioners in Tanzania and across Africa continent to practice their NLP skills to solve different problems in organizations or societies related to Swahili language. Swahili News were collected from different websites that provide news in the Swahili language. I was able to find some websites that provide news in Swahili only and others in different languages including Swahili.
MAIN OBJECTIVE
To develop a multi-class classification model to classify news content according to their specific categories specified.
SPECIFIC OBJECTIVES.
To classify national news as national news
To classify international news as international news
To classify business news as business news
To classify sports news as sports news
To classify entertainment news as entertainment news

DATA UNDERSTANDING.
The dataset was created for a specific task of text classification, this means each news content can be categorized into six different topics (Local news, International news , Finance news, Health news, Sports news, and Entertainment news). The dataset comes with a specified train/test split. The train set contains - 80% of the dataset and test set contains 20 - % of the dataset.

DATASET DESCRIPTION.
The dataset describes 5151 rows and 3 columns of news from different sources in Tanzania.These news are in 5 different news categories from national news to entertainment news.
Your goal is to accurately classify each swahili news content into five specified categories below:
Kitaifa (National)
Kimataifa (International)
Biashara (Business)
Michezo (Sports)
Burudani (Entertainment)
Data Fields
id: id of the sample
content: the news articles
label: the label of the news article

DATA PREPARATION
These are the steps followed in preparing the data;
Loading Data 
This includes both the train and test datasets to be used in our project
Cleaning Data
We checked for null and duplicate values. Our datasets didn’t have any 
Changed our text to lower case for ease in manipulation and maneuvering. We also went ahead and removed any punctuations and white spaces within our text so as to prepare for tokenization.
Tokenization.
Removing stopwords. These are those common words within our text that hold no value/meaning 
Lemmatization and stemming
Dropping Columns


DATA ANALYSIS
Findings from EDA

We mainly used univariate analysis 
The most common news within our dataset is the ‘kitaifa’ news, followed by ‘michezo’, ‘biashara’, ‘kimataifa’ and lastly, ‘burudani’.
Our data was a text file. We approached our analysis using NLP - Natural Language Process. 
1. Categorical Variables we visualised our columns using the steps below. 
We viewed our categories in a countplot, later we converted our Content column to News Length using frequency tables. This enabled us to plot our News length which is positively skewed. 
We also visualised our content column using word cloud, to be able to see the words that were mostly used. 
2. Numerical variables 
We got a mean of 1608.7 from our new column News Length . 
We visualised the content column using histogram, this was useful to determine the number of characters present in each sentence. 


Modelling 
The models we used for our project with their  accuracy score were as follows:
Multinomial Naive Bayes - 90%
Support Vector Machine(SVM) - 86%
K Means  - We got 5 clusters 
We used Smote to balance our data. (Random over_sampling imbalanced datasets(smote)
It is most commonly used to solve the imbalance problem. It aims to balance class distribution by randomly increasing minority class examples by replicating them)

Challenging the Solution 
We used the Xgboost Model.  Which had a percentage of  95%. 



