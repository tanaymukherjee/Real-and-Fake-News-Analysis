# Real-and-Fake-News-Analysis

### Introduction & Background:
For our final project, we wanted to analyze a dataset that focuses on a topic that is relevant, applicable and relatable. Having said that, ‘Fake News’ is very prevalent throughout our generation and is a coined term used very often in our society. The amount of untruthful information, rumors and unreliable news that is out there is growing more and more everyday. It is also becoming extremely difficult to distinguish fake news from real news, as imposters get smarter and technology advances, making it very easy to create websites to mimic legitimate news sources.

Fake news articles also have a greater influence and reach, more than ever now, as news can be shared across the world in seconds, exponentially increasing the reach to consumers, regardless of the legitimacy of the news. This means that the impact this has on our society is now more significant than ever as a majority of the time these articles are created with a malicious intent and targeted to a specific audience in order to influence someone's belief, decision making or stir up negative feelings. We saw the fake news and real news dataset as a good opportunity to help us explore and dive deeper into this topic.


### Motivation:
As misinformation, rumors or fake news are becoming abundant, we are motivated by the clash  between real news and fake news. How can we minimize the damage and public insecurity caused by its explosive growth?

Our project is structured around the 2 main research questions:
- Can we automatically classify a news article as real or fake news?
- Can we quickly identify the topic of news through the topwords?


### Text Dataset Description:
We obtained our dataset from Kaggle. There are two separate CSV files, one named fake news and one named real news. Each file has four columns, labeled as follows: article title, article text, article subject, and publication date.

In order to have a better baseline understanding of the data set, we used different methods to locate general patterns that would later help us with our analysis. With named entity recognition, we found the most frequent entities (such as people and places) mentioned in both real and fake news. This included items such as “Trump”, “Mueller”, and “War.” With N-gram analysis, we found unigrams, bigrams and trigrams to help build models for our LDA topic modeling analysis. The top salient results were “Trump”, “Donald Trump”, and “President Donald Trump.”


### Text Preprocessing Description:
Text preprocessing is the first and an important step for NLP tasks. It transforms text into a more digestible form so that machine learning algorithms can perform better. In this project, we will use 3 methods to pre-process our raw datasets. The first one is regular expression. Regular expression can give us a more powerful and flexible method for describing the character patterns we are interested in. Second is tokenization. Tokenization is the task of cutting a string into identifiable linguistic units that constitute a piece of language data. We will also use normalization. Normalization is a process that converts a list of words to a more uniform sequence. By transforming the words to a standard format, other operations are able to work with the data and will not have to deal with issues that might compromise the process.

Before we could begin our analysis, we needed to properly format our dataset. First we joined the “real” and “fake” news datasets. Fake news received the tag “0” and real news was tagged with “1”. We then converted the dates of the publications to a date time format. Next, the data was parsed to exclude the publisher data, i.e. we only wanted the text pertaining to the body of the articles. The data was cleaned to set text to lowercase, remove line breaks and to remove links. And then we finally removed stop words.


### Methods & Model Evaluation:
Part 1: Topic Modeling
Part 2: Text Classification


### Conclusion and Practical Implications:
Logistic regression is one of the most basic and  simplest methods of machine learning. By tuning the hyperparameters for logistic regression, we can improve the model in terms of reducing the problem of overfitting and increase the accuracy score to 99.26%. Our results suggest that text feature in our data set are effective for distinguishing between fake and real news, and that robust classifiers can be constructed that enable the discovery of fake news articles.

As information shapes how we view the world and influences our decision making, no one can deny the abundance of misinformation, rumors, or fake news. By building an effective classification model, we can filter out news articles that are not credible and as a result, relieve the negative impact of fake news. It is important that such solutions are identified as they will prove to be useful to both readers and tech companies involved in the issue


### Team Members:
1. Danny Huang
2. Nicole Ly
3. Nishtha Ram
4. Qinyi Li
5. Tanay Mukherjee
6. Trang Le
7. Xinyi Li

## Submission to:
Prof. Chaoqun Deng
