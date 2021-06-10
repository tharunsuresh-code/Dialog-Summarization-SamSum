# Dialog-Summarization-SamSum
Dialog Summarization modelling using Topic modelling and similar sentence reduction

## Project
This project has been carried as part of a course project which will be extended to further research down the line. The primary objective of this summarization project is to augment information available in each utterance with additional modules that extract relevant features from the dialogue set. With the advent of transformer models, several augmentation steps can help improve the generation task in hand.

## Contributions of this project
We have made of use of two modules mainly:
* BerTopic - https://towardsdatascience.com/interactive-topic-modeling-with-bertopic-1ea55e7d73d8
* Sentence Similarity - https://nlp.town/blog/sentence-similarity/

We have noticed that certain sentences in dialogue set contribute more to the dialogue summary than others. Hence topic classification is one of the important steps that helps to segregate utterances such as greetings, fillers, affirmations, acknowledgements from questions, explanations, responses. This marked difference classified at utterance level helps to augment the dataset.  
Also, in many dialogue sets, there can be back and forth explanations around intent/topic that makes it redundant to be included in a summary. Hence, identifying similar sentences across the dataset which ensures inclusion of topics that are looped back at a later point in conversation, helps to avoid them being included in the summary.

## How to run
The python notebook in experiments folder is self explanatory. Different experiments are marked with sub-headings which can be run directly in colab. Even the dataset is attached only for reference purpose and they can also be directly imported in the python environment. 

## Baselines and model
T5 is the baseline chosen on which the above mentioned modules have been implemented to augment the dataset. These are available in the python notebook. 

## Members of the project
* Tharun Suresh
* Aseem Srivastava
