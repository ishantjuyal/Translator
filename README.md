# Machine Translator Model
A Machine Translation model which converts English to German. 

## Dataset
I used the Deutsch to English parallel sentence data from [here](http://www.manythings.org/anki/). You can get dataset related to many languages here.

## Approach
I started with the problem being very confused about what to do with the data and then took some help from online resources. 
I preprocessed the data first, removed all the special characters and converted whole data to lowercase. 

I used tokenizer from keras.preprocessing to make two different tokenizers, one for English and one for Deutsch. Then I used these tokenizers to encode all the sentences into sequences with padding. I took the maximum length as 8 because most of the sentences had 8 as the length, both in English and Deutsch. 

## Training
I used Neural Networks, LSTM to be specific. I used 2 layers of LSTM in my model and trained the model on all the data present. 

## Performance
The performance was much better than I expected as Deutsch is a really tough language with complex grammar. 
Here are some photos which show the performance of the model in translating some basic English sentence to Deutsch. 

![Image 1](https://github.com/ishantjuyal/Translator/blob/master/English%20to%20German%20Translator/Image%201.png)

![Image 2](https://github.com/ishantjuyal/Translator/blob/master/English%20to%20German%20Translator/Image%202.png)

References:
[Analytics Vidhya](https://www.analyticsvidhya.com/blog/2019/01/neural-machine-translation-keras/)
