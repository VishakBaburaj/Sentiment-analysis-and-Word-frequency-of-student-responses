Sentiment Analysis and Topic Modeling of student responses.

Problem Statement

Given the times of a new normal since the COVID-19 pandemic, we know how most industries and sectors have forcibly transitioned from the traditional workspace to a work-from-home model during the coronavirus global pandemic. One of which endured digital adoption as no exception is the educational domain.
Even though the education sector has been keeping up to speed with the advancements of the latest requirements, the parallel disadvantages are hard to ignore. The examination scenario is a complete game-changer. In India, the intensity and importance are given to class 12 board examinations since they are considered a predetermining factor of a prosperous future, thus an integral part of an Indian student’s education. Therefore, the commencement of the class 12 board exams was initially said to be conducted offline to bring back the efficacy of its traditional pattern; however, this comes with the opportunity cost of guaranteeing and safeguarding the student and public health.

Significance of the project

The harsh reality of the Indian education system eventually curates most decisions where students do not hold much of a role in conclusions drawn for them. Thus, this paper stands as a platform for their voices as it is necessary to research students' perspectives. This also constituent other factors such as their parents' opinions and support. Even supposing the stance is not offline, this could be dissatisfying for some, maybe a relief for others, but what stands of utmost importance is the overall uneasiness and concern that should not be unheard.

Objectives

The first objective is to identify the sentiments of each student based on their responses. The sentiments can be divided into positive, negative, and neutral sentiments. 
The second objective is to identify how many times a certain emotion has been used by the students in positive, negative, and neutral sentiments. 
The third objective is to identify the number of times a student has used a combination of emotions. 
The fourth objective is to find the reasons why the students want the exams to be conducted at a later date or to be canceled.

Project Approach

The first methodology is in deciding the research approach. There are three common types of research approaches Quantitative, Qualitative, and Mixed research approach. The quantitative research approach deals with numeric data, the qualitative research approach deals with textural data, and the mixed research approach deals with both textural and numeric data. 
Based on the project, the most appropriate research approach to conduct is the qualitative research approach, where the data collected will be entirely in a textural format. Qualitative research helps us identify societal phenomena from a participant's point of view.
Several methods are used to conduct qualitative research recommended in five main ways: Case Studies, Grounded theory, Ethnography, Content analysis, and Phenomenological study. The method adopted is the phenomenological study determined to understand the experience of a particular event from the participant's point of view.

Data Collection

Data collection has been done through a primary source of data the survey method. Google Form is the best choice to distribute the survey considering the COVID-19 situation in 2021. Data collection is done through the snowball sampling technique where primary contacts are asked to distribute the google form to their target acquaintances. The survey is stated for academic purposes only, and the personal data of the respondents are not shared with anyone.

Data Understanding

The google form consists of four sections. 
The first section comprises three questions related to which board the students are studying in, how they feel about their board exams and their opinions on whether to cancel or conduct the exams later. All three questions are definite, and the students are given an option to choose within the mentioned choices. 
The second section consists of one question as to why they want the board exams to be canceled. This section will only be redirected only if the student’s opinion is to cancel the exams. 
The third section consists of one question to state why they want their exams to be conducted later. This section will only be redirected only if the student’s opinion is to conduct the exams later. The students can type their reasons in short or long answers for both the second and third sections. 
And finally, the fourth section consists of one question regarding the demographic from which state the respondents are from.

Tools and Programming language adopted.

Python libraries used for data analysis are 
Pandas.
Numpy.
Re used to check whether a string matches a regular expression to remove punctuations in the data frame, 
From the autocorrect library Speller is used to correcting the spelling mistakes in the data frame. 
nltk a Natural Language Processing library, 
From nltk.tokenize, word_tokenize to split the sentences into words.
From nltk.stem.wordnet, WordNetLemmatizer used to Lemmatize the words into one form. 
From nltk.corpus, stopwords to remove stopwords such as ‘the’.
From vaderSentiment.vaderSentiment, SentimentIntensityAnalyzer to identify the sentiments of each response in the data frame. 
Gensim for topic modeling, 
Import gensim.corpora for creating corpora for topic modeling
From gensim.models CoherenceModel to identify the accuracy of the topic modeling
PyLDAvis and pyLDAvis.gensim_models to visualize the topic modeling.
Microsoft Excel is used to export the analyzed data.
Tableau is used to visually present the findings.

Techniques Adopted

Text preprocessing is a technique used to clean textual data to a form where Natural Language Processing can be analyzed, and the results can be accurate. 
The following are the significant text preprocessing techniques Stop Words removal, Word tokenization, Parts of speech tagging lemmatization, and stemming, Term frequency Inverse document frequency (TFIDF).

Sentiment analysis describes whether a particular text is negative, positive, or neutral sentiment. It helps in classifying the opinions of students into negative, positive, or neutral sentiment. To do so Lexicon-based sentiment analysis has been used. A lexicon sentiment is a list of lexicon words labeled according to their semantic orientation, positive, negative or neutral. 

Word Frequency helps measure how many times a particular word has been used in qualitative data. This can help in identifying the most expressed emotions from the student’s responses.

Word combination helps to identify what type of combinations are used most while a student describes their emotions.

Topic modeling helps in organizing and clustering the qualitative data by subject or theme. A text mining technique will identify the patterns of word co-occurrence across a corpus of documents. This technique is used to determine the mental health of why the students want the exams to be canceled or conducted on a later date.

Model

Sentiment Analysis	

To identify the sentiments of students. There are different methods in Lexicon-based sentiment analysis. The appropriate way based on the data is Vader lexicon sentiment analysis. VADER stands for Valence Aware Dictionary and sEntiment Reasoned. It is a rule-based sentiment analysis framework. For Vader sentiment analysis, specific scores have been associated with words, emoticons, and even slang words in the library, making it easier for analytics (Sarkar, 2019). Furthermore, the Vader sentiment analysis can be called out in python with the essential function SentimentIntensityAnalyser. The function will give an output containing negative, positive, and neutral scores in a text and sum that up in the compound score, determining whether the entire text is in positive, negative, or neutral sentiment.
Analyzing further, a condition has been given to understand the numeric representation in the textural form, whether a text is negative, positive, or neutral. If the compound score is greater than 0, then it is a positive sentiment. If the compound score is less than 0, it is a negative sentiment. If both these conditions are not followed, it will lead to a neutral sentiment in which the compound score is 0.

Word Frequencies

After finding the sentiment, the following analysis is to identify the word frequency of each feeling. To develop the frequency, the semicolon punctuation is replaced with a comma to separate the words. Here we cannot use the phrase tokenization as there are two sentences in the feelings category, which are “Inability to concentrate” and “More time for preparation” So, to divide the words, coding was used. The result of the word frequency is based on how many times a particular term has been used in each sentiment.

Word Combinations

Analysis to find out the combination of words used to describe the feelings of students. First, feelings such as the Inability to concentrate have been replaced for its short-form ITC, and More time for preparation has also been replaced with its short-form MTFP. It is then assigning a new variable to calculate the total number of words used in a response containing the feelings described by each student.
A condition is given to extract the mixed feelings combinations. A condition is given, to the compound score between -0.4 and 0.4 can be considered mixed sentiments. Extracting these data and grouping is based on the number of words.

Topic Modeling

The topic modeling has been done individually to both the response's reasons for canceling and conducting late. 
After cleaning the textural data, the first step in achieving the results of Topic Modelling is to input a training LDA model. Converting the cleaned data into corpus and dictionary. The main objective of the corpus is to map the word id (unique id) and word frequency of words from each document in a dictionary.
TFIDF object, which gives an output of how relevant a term is in the document and then applies this transformation into the existing corpus, is the unique words from the documents. This helps in achieving much more accuracy for the topic modeling results.
The next step is in adopting the LDA training and testing model. To run a topic model, the assumption of the topic is needed to be assigned to the corpus sensibly. Another parameter is the hyperparameters alpha and beta that affect the sparsity of topics. Chunk size is the number of topics to be used in the training model. Here the chunk size is the total sample size because the data has been collected through google form as unstructured data. Passed is the total number of training passes to the model.

Testing and Validation

The perplexity score helps in deciding how well the topic modeling model is. It is used for the language evaluation model. The lesser the perplexity score, the better the LDA model. Perplexity is not correlated with human judgment. Here the perplexity is -5.79, which is very good as the perplexity is in the negatives.
The coherence score helps in identifying how well a word is placed in a topic. Here the coherence score is 60% which is good comparatively.

Findings

![image](https://user-images.githubusercontent.com/86551004/187086579-a3f78802-3a3b-4039-b1ca-2e47ec4c14e1.png)

