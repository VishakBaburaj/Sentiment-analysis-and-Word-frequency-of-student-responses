# Sentiment Analysis and Topic Modeling Approach of student responses.

# Problem Statement

Given the times of a new normal since the COVID-19 pandemic, we know how most industries and sectors have forcibly transitioned from the traditional workspace to a work-from-home model. One of which endured digital adoption as no exception is the educational domain.
Even though the education sector has been keeping up to speed with the advancements of the latest requirements, the parallel disadvantages are hard to ignore. The examination scenario is a complete game-changer. In India, the intensity and importance are given to class 12 board examinations since they are considered a predetermining factor of a prosperous future, thus an integral part of an Indian student’s education. Therefore, the commencement of the class 12 board exams was initially said to be conducted offline to bring back the efficacy of its traditional pattern; however, this comes with the opportunity cost of guaranteeing and safeguarding the students and public health.

# Significance of the project

The harsh reality of the Indian education system eventually curates most decisions where students do not hold much of a role in conclusions drawn for them. Thus, this project stands as a platform for their voices as it is necessary to research students perspectives. Even supposing the stance is not offline, this could be dissatisfying for some, maybe a relief for others, but what stands of utmost importance is the overall uneasiness and concern that should not be unheard.

# Project Approach

## Research approach

1) The most appropriate research approach to conduct is the qualitative research approach, the data collected will be in a textual format.
2) Qualitative research helps to identify societal phenomena from a participants point of view.
3) To conduct qualitative research recommended there are five main ways: Case Studies, Grounded theory, Ethnography, Content analysis, and Phenomenological study. 
4) The method adopted is the phenomenological study determined to understand the experience of a particular event from the participants point of view.

## Data Collection

1) Data collection has been done through survey method which is the primary source of data collection. 
2) Google Form has been used to distribute the survey considering the COVID-19 situation in 2021. 
3) Data collection is done through the snowball sampling technique where primary contacts are asked to distribute the survey to their target acquaintances.

## Data Understanding

The google form consists of four sections. 

1) The first section comprises three questions related to which board the students are studying in, how they feel about their board exams and their opinions on whether to cancel or conduct the exams later. All three questions are definite, and the students are given an option to choose within the mentioned choices. 
2) The second section consists of one question as to why they want the board exams to be canceled. This section will only be redirected only if the students opinion is to cancel the exams. 
3) The third section consists of one question to state why they want their exams to be conducted later. This section will only be redirected only if the students opinion is to conduct the exams later. The students can type their reasons in short or long answers for both the second and third sections.
4) The fourth section consists of one question which state the respondents are from.

## Techniques Adopted

### Text pre-processing
1) Text preprocessing is a technique used to clean textual data to a form where Natural Language Processing can be analyzed, and the results can be accurate.

### Sentiment analysis
1) Sentiment analysis describes whether a particular text is negative, positive, or neutral sentiment. 
2) To do so Lexicon-based sentiment analysis has been used. A lexicon sentiment is a list of lexicon words labeled according to their semantic orientation, positive, negative or neutral. 

### Word Frequency
1) Word Frequency helps measure how many times a particular emotion has been used in qualitative data. 

# Data Analysis

### Sentiment analysis 
1) The appropriate method based on the data is Vader lexicon sentiment analysis. 
2) VADER stands for Valence Aware Dictionary and sEntiment Reasoned. 
3) It is a rule-based sentiment analysis framework. 
4) For Vader sentiment analysis, specific scores have been associated with words, emoticons, and even slang words in the library, making it easier for analytics.
5) The Vader sentiment analysis can be called out in python with the essential function SentimentIntensityAnalyser. 
6) The function will give an output containing negative, positive, and neutral scores in a text and sum that up in the compound score.
7) Analyzing further, a condition has been given to understand the numeric representation in the textual form, whether a text is negative, positive, or neutral. 
8) If the compound score is greater than 0, then it is a positive sentiment. If the compound score is less than 0, it is a negative sentiment. If both these conditions are not followed, it will lead to a neutral sentiment in which the compound score is 0.

### Word Frequency
1) After finding the sentiment, the following analysis is to identify the word frequency of each emotions. 
2) To develop the frequency, the semicolon punctuation is replaced with a comma to separate the words. 
3) The result of the word frequency is based on how many times a particular keyword or emotion has been used in each sentiment.

# Findings and Insights

## Sentiment Analysis and Word Frequency
https://public.tableau.com/app/profile/vishak.bbauraj/viz/SentimentAnalysisonClass12StudentResponses/Student_Response_Dashboard

