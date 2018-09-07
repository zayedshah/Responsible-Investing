# A New Bottom Line

### Introduction

In this section, rather than annotate in each notebook, we will have a description of the approach taken in using neural networks and pretrained word embeddings to predict company's sector name using business description.

### 1. Neural Network

After the benchmark set by Naive Bayes and Logistic Regression with accuracy of 76% and 80% respectively, we might have thought we should check out neural networks; with all the RNNs and LSTMs we must surely get better results. Well..

Google Colab has been used for these exercises to make use of its GPU. A very simple neural network has been used to see if it shows any improvement in results. What was observed was that very soon it would start to overfit with accuracy hovering at around 80%. We will see similar behaviour when we try with LSTM or with pretrained word embeddings.

### 2. LSTM and CNN

Initial observation with using LSTM was that it was quite slow. Accuracy progressively improved till about 80%! It was noticed that adding a convolution layer helps to speed up. In this one, using Dropout layer was avoided as accuracy was converging slowly.

### 3. GloVe

Pretrained word embeddings from GloVe with 100 dimensions was given a try. Embeddings was retrieved in local machine and uploaded to Google Drive to be used for Training. Part 1 is where the embeddings get pickled in local machine. Part 2 is where training takes place in Google Cloud with Colab. Did the accuracy improved? No. 

### 4. Gensim

Last hope was to use Google's word2vec - it has 300 dimensions for the word embeddings. GloVe has embeddings with 300 dimensions too but always good to venture to a different place. The last test evaluation gave accuracy of 82%.
