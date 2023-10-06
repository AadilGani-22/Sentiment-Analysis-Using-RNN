# Sentiment-Analysis-using-RRN

Sentiment Analysis: Analyze the sentiment of text data, such as customer reviews or social media posts, using LSTM to determine positive, negative sentiments. 

Sentiment analysis, also known as opinion mining, is a natural language processing (NLP) 
technique used to analyze the sentiment or emotional tone expressed in a piece of text data. One 
popular approach to sentiment analysis is using Long Short-Term Memory (LSTM), which is a 
type of recurrent neural network (RNN) architecture. LSTM models are well-suited for analyzing 
sequential data, such as sentences or paragraphs, because they can capture long-range 
dependencies and contextual information effectively.

The process of sentiment analysis typically involves several steps. We have imported pandas and 
read the csv data sheet, we created x and y variables where x is independent variable i.e 
sentences and y is dependent variable i.e label. We also made train and test set and defiened the 
shape for it. Then we took the index of 1st sentence and put in x and y train. 
We used Tokenizer which will convert string into values and this models only accepts numerical 
data for algorithm, num_words is used to get the most frequent words in the data sheet, as we 
print the x and y train now it has been converted into numbers. We imported pad_sequences and 
set the maximum length to 100 and every sentence has equal length now and it can be easily 
compared and identified. 

There are 3 layers in this model: SimpleRRN, Dense and Activation layer. In SimpleRRN we 
have set the neurals as 50 and in activation the softmax is used to find out the probability of the 
most frequent word in the sentence. We classify the model and fit the model. We find the 
accuracy of the model by importing the accuracy score. The input sentence is conerted into array 
and the result is shown as 0 for negative and 1 for positive sentence. 
