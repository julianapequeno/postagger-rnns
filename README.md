# Part Of Speech Tagging - Recurrent Neural Networks

In this project, I implemented and compared several RNN-based models as POS taggers.This project was an activity to 'Natural Language Processing' classes in my grad.
I truly enjoy NLP and during the semester it was a pleasure to study and practice NLP.

### 🗺️ First, what's is **POS TAGGING**? 

POS Tagging (Part-of-Speech Tagging) is the task of assigning each word in a sentence its grammatical category (noun, verb, adjective, etc.). This process involves a deeply understanding of what the sentence is trying to represent. That is, not always a word means what it would mean if it was alone in the sentence. 

It's possible to do a POS TAGGING with n-grams, though it is kind of complex if the sentence grow longer (O(n^2)). Then, we can try another way, with Recurrent Neural Networks.

In this context, I used the following N.Ns
- Recurrent Neural Network
- Long Short Term Memory (LSTM)
- Bidirectional Long Short Term Memory (BiLSTM) with two stacked layers

As well as methods that can improve the results.
- GLOVE
- FastText including subword information for better handling of out-of-vocabulary words
- Contraction expansion using NLTK

GLOVE is a unsupervised NLP model for global word vectors representations from Standford University. It has a more consistant form that allow us to focus on the development of a model.

FastText, developed by Facebook AI Research, also provides word embeddings but works differently:
it breaks words into subword units (character n-grams). FastText recognizes subwords differently from Glove, and may be better to recognize unknown words.

## The Dataset - Peen Tree Bank 🌳
 Peen Tree Bank is a dataset created for POS TAGGING tasks. It has lots of text alread annotated with its part-of-speech per word. Which is what we need to train the model to predict.