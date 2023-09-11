# BREAST-CANCER-DETECTION

# Breast Cancer Detection Using DEEP LEARNING AND MACHINE LEARNING

# About Dataset:
Breast Cancer Wisconsin (Diagnostic) Data Set Used Here
Features are computed from a digitized image of a fine needle aspirate (FNA) of a breast mass. They describe characteristics of the cell nuclei present in the image. 
n the 3-dimensional space is that described in: [K. P. Bennett and O. L. Mangasarian: "Robust Linear Programming Discrimination of Two Linearly Inseparable Sets", Optimization Methods and Software 1, 1992, 23-34].

This database is also available through the UW CS ftp server: 
ftp ftp.cs.wisc.edu 
cd math-prog/cpo-dataset/machine-learn/WDBC/

Also can be found on UCI Machine Learning Repository: https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29

# Attribute Information:

1) ID number 
2) Diagnosis (M = malignant, B = benign) 
3-32)

# Ten real-valued features are computed for each cell nucleus:

a) radius (mean of distances from center to points on the perimeter) 
b) texture (standard deviation of gray-scale values) 
c) perimeter 
d) area 
e) smoothness (local variation in radius lengths) 
f) compactness (perimeter^2 / area - 1.0) 
g) concavity (severity of concave portions of the contour) 
h) concave points (number of concave portions of the contour) 
i) symmetry 
j) fractal dimension ("coastline approximation" - 1)

The mean, standard error and "worst" or largest (mean of the three
largest values) of these features were computed for each image,
resulting in 30 features. For instance, field 3 is Mean Radius, field
13 is Radius SE, field 23 is Worst Radius.

All feature values are recoded with four significant digits.

Missing attribute values: none

# Class distribution: 357 benign, 212 malignant


# ABOUT LSTM:

LSTM stands for Long Short-Term Memory, which is a type of recurrent neural network (RNN) that is commonly used in deep learning for processing sequential data, such as text, speech, and time series data.

LSTMs are designed to overcome the limitations of traditional RNNs, which suffer from the vanishing gradient problem when training on long sequences of data. The vanishing gradient problem occurs when the gradients propagated through the network become very small as they are multiplied by many small weights in the recurrent connections, which makes it difficult to learn long-term dependencies in the data.

LSTMs solve this problem by introducing a memory cell that can store information for long periods of time, and three gates (input, forget, and output) that control the flow of information into and out of the cell. The input gate controls which information to let into the memory cell, the forget gate controls which information to discard from the memory cell, and the output gate controls which information to output from the memory cell.

The architecture of an LSTM cell allows it to selectively remember or forget information over time, which makes it well-suited for processing sequential data with long-term dependencies. LSTMs have been used successfully in a wide range of applications, such as natural language processing, speech recognition, and stock price prediction.

# ABOUT BiDirectional LSTM:

BiLSTM stands for Bidirectional Long Short-Term Memory, which is an extension of the traditional LSTM architecture. BiLSTMs are designed to capture both past and future context of a sequence by processing the sequence in both forward and backward directions simultaneously.

In a traditional LSTM, the input sequence is processed from left to right, and the output sequence is produced one token at a time, with each token being generated based on the preceding tokens in the sequence. This means that the output at a given time step only has access to the past context of the sequence.

In a BiLSTM, the input sequence is processed both from left to right and from right to left using two separate LSTMs. This allows the network to capture both past and future context of the sequence, which can be useful in tasks such as natural language processing, where the meaning of a word can depend on the words that come both before and after it in a sentence.

The output of a BiLSTM is typically computed by concatenating the forward and backward hidden states of the LSTMs at each time step. This combined hidden state can be fed into a downstream task, such as a classification or regression model.

BiLSTMs have been shown to be effective in a variety of tasks, such as named entity recognition, sentiment analysis, and machine translation. They are widely used in deep learning for natural language processing and speech recognition applications, where capturing both past and future context is critical for achieving high accuracy.

Conclusion:
Using LSTM algorithm we can conclude that this works very well for the prediction of the Breast Cancer with Provided Datasets.


![PredictionBC](https://user-images.githubusercontent.com/103871423/236560291-cdc108d0-128f-4143-bf7d-84316bde009e.png)
