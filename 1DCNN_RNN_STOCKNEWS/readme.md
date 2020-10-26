# Problem Statement & Reference Architecture

* **Aim**: Use Reddit News Headlines to predict the movement of Dow Jones Industrial Average.   


* **Data Source**: https://www.kaggle.com/aaron7sun/stocknews 


* **Data Description**: Dow Jones details on Open, High, Low and Close for each day from 2008-08-08 to 2016-07-01 and headlines for those dates from Reddit News. 


* **Methodology**: For this project, we will use GloVe to create our word embeddings and CNNs followed by LSTMs to build our model. This model is based off the work done in this paper https://www.aclweb.org/anthology/C/C16/C16-1229.pdf.


### Brief:

Predicting Stock market behavior is a hot topic among the NLP researchers. RNNs, LSTMs, GRUs have proven greatly efficient when dealing with Sequential data. But it turns out that other than RNNs, CNNs too are really effective in extracting features from the text. Although, we can directly feed text to an RNN but there are cases when the sequences are really long which makes it harder to use RNN since they're computationally expensive. <br><br>
**In this project, we have used 1D CNN-RNN architecture. The original work behind using 1D CNNs with RNNs was proposed in this paper titled "Combination of Convolutional and Recurrent Neural Network for Sentiment Analysis of Short Texts".**
