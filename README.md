# Word Completion

### Motivation
The Word Completion is similar to Google Smart Compose, where a user types a message and systems suggests possible next word(s) in sequence which it has learnt from the train data.

This repository demonstrates the auto-complete(Next Word Prediction) in two ways,
1. Probabilistic Approach (Smoothing Technique's)
2. Model Based Approach

### 1. Smoothing Techniques. 
There are statistical models to perform tasks like auto-completion of sentences, where we use a probabilistic model.

Naturally we have many combinations of possible words, it becomes impossible to add all the data in training set so that our model can predict accurately on unseen data. This can be overcome by smoothing technique.

Smoothing Techniques are  simpler to implement and computationally efficient. However, they can struggle with complex language or unseen patterns.

Some of Smoothing Techniques are.
1. Add-1 Smoothing Technique (also known as Laplace Smoothing Technique).
2. Add-k Smoothing Technique(Improvement of Add-1).
3. Kneser Ney Smoothing Technique.
4. Good Turing Smoothing Techniue. 

### Model Based Approach
In this case Machine Learning models are used to learn the relation between the previous words and predict next word.

Model Based Approach can be implemented using `RNN(Recurrent Neural Network)`, the idea of `seq2seq` model with help of `Teacher FOrcing` techniques is implemented using LSTM/GRU cells.


Model based can achieve higher accuracy, especially with large datasets. However, they require more computational resources and training data.