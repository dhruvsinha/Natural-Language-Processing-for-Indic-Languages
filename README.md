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
1. Classification_clean.ipynb: This notebook performs classification task on indic languages
2. PoS_Tagger_final.ipynb: This notebook performs part of speech tagging task
3. RNN_based_sentence_generation.ipynb: This notebook generates paragraph in Hindi
4. indic_languages_report.pdf: Final project report
5. final_presentation.pdf: This is a summary of the project report that we presented to our class. **Please navigate to this pdf file to get a more concise summary of the project report**

## Tasks Performed
### Classification Task

The language detection and classification task was performed on Hindi, Kannada, Malayalam, Tamil, and Bengali. We used BoW to train the model and achieved high accuracy. 
