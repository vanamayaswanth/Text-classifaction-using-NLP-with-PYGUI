# Introduction:
In this project, I developed a question-answering application using natural language processing (NLP) techniques. The aim of the application is to provide users with relevant answers to their questions by comparing their input to a dataset of pre-existing questions and answers.

## Architecture:
I began by importing the necessary Python libraries, including pandas, numpy, and nltk, and then read in the question-answer data from three different files. I merged the data into a single DataFrame and performed some basic preprocessing steps, including dropping duplicate questions and removing stop words and punctuation from the questions. Next, I used the WordNetLemmatizer to lemmatize the remaining words and generate tokens from the questions.

To generate a similarity score between the user's input and the pre-existing questions, I used the TfidfVectorizer to generate a sparse matrix of term frequency-inverse document frequency (TF-IDF) values. I then calculated the cosine similarity between the user's input and each question in the dataset and returned the most similar question and its corresponding answer to the user.

To make the application user-friendly, I used the PySimpleGUI library to create a basic graphical user interface (GUI) with a text input field and a button for the user to submit their question.
