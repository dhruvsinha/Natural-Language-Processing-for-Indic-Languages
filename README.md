# Natural Language Processing for Indic Languages

## Abstract

This paper aims to replicate some common NLP tasks on 5 Indic languages- Hindi, Bengali, Tamil,
Malayalam, and Kannada. We will be performing language detection, text classification, part of speech
tagging, sentence generation on these languages. We have trained several datasets using BoW, LSTMs,
and GRUs to perform the mentioned tasks. Our model was able to perform exceptionally well in language
detection. The model performed well on classification of Kannada and Malayalam texts but failed for
Hindi, plausibly due to data constraints. For Part of Speech tagging in Hindi, the model was performing
well but suffers from severe overfitting. Finally, for sentence generation, we saw that the model was able
to learn some very interesting nuances of Hindi which took us by surprise!

## Files Attached
1. Classification_clean.ipynb: This notebook performs language detection and text classification task on indic languages
2. PoS_Tagger_final.ipynb: This notebook performs part of speech tagging task
3. RNN_based_sentence_generation.ipynb: This notebook generates paragraph in Hindi
4. indic_languages_report.pdf: Final project report
5. final_presentation.pdf: This is a summary of the project report that we presented to our class. **Please navigate to this pdf file to get a more concise summary of the project report**

## Tasks Performed
### Language Detection

The language detection task was performed on Hindi, Kannada, Malayalam, Tamil, and Bengali. We used BoW to train the model and achieved high accuracy. This is because the script of each of these languages is different and therefore it should not be difficult for the model to distinguish just by looking at the script. 

### Text Classification

In this part, we classify text clippings into some broad categories- Sports, Business, Entertainment, etc. The methodology for this exercise is same as that of the language detection task. We have used linear operations on embedding layer and in the end we get probabilities of each of the classes. The image below is the snapshot of the classification dataset for Hindi. 

| ![classification_data.jpg](/indic_languages/classification_data.jpg) | 
|:--:| 
|Hindi Classification Dataset|

The results of performing classification task on Hindi were very poor. This is because the dataset was very small. Moreover, it is very
difficult to differentiate between some of the classes. For example, sentence belonging to class 'India and sentence belonging to class 'Sports' might have intersection of words.

| ![classification_hindi.jpg](/indic_languages/classification_hindi.jpg) | 
|:--:| 
|Hindi Classification Result|

The classification task performed on Kannada showed good results because the dataset was large and classes were distinct. 

| ![classification_Kannada.jpg](/indic_languages/classification_Kannada.jpg) | 
|:--:| 
|Kannada Classification Result|

### Part of Speech Tagging

We trained a model to tag each word in Hindi sentence with their respective Part of speech.

### Paragraph Generation

For this task, we generated sequences/sub-sequence in hindi language based on a given prompt. We trained a multi-layer long short-term memory (LSTM) and (GRU) RNN. 
The LSTM model produced some excellent results. 

| ![lstm_sentence.jpg](/indic_languages/lstm_sentence.jpg) | 
|:--:| 
|Sentence Generation by LSTM|

For those who can't read Hindi, the model is able to pick up finer nuances of the language. For example, the gender identification of a word in
Hindi is unique. This aspect is displayed in some sentences. The singular/plural words are also used in almost perfect ways. 
