## Introduction

This work has 2 sections. 

The first part is `Responsible Investing.ipynb` notebook which uses Naive Bayes and Logistic Regression to predict company's sector name from business description.

The second part is `A New Bottom Line` folder which has 6 notebooks, and explores different flavours of Neural Networks and pretrained word embeddings from GloVe and Google's word2vec (using Gensim), to predict the same task as above.

## Results

Naive Bayes gave accuracy of 76% while Logistic Regression gave 80% accuracy.

Neural Networks - from a simple one to using LSTM and CNN didn't seem to have improved accuracy. Using pretrained word embeddings from GloVe and Google's word2vec with Gensim didn't seem to have improved accuracy either. The accuracy from these excercises hovered at around 80%.

## Conclusion

Using traditional methods of machine learning with Naive Bayes and Logistic Regression seemed to have done a good job. 

With neural networks, the lacklustre accuracy may be because neural network models are too complex, and not needed, for a small dataset such as ours - we have only around 23k samples. Or it's possible that we are missing something and we may have to dig a little more deeper.
