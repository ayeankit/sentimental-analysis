# Sentimental-analysis
![image](https://user-images.githubusercontent.com/72691866/190260250-6747b5fc-03c1-4952-a5f1-3efc14ac0dba.png)



Sentiment analysis or opinion mining is a simple task of understanding the emotions of the writer of a particular text. What was the intent of the writer when writing a certain thing?

We use various natural language processing (NLP) and text analysis tools to figure out what could be subjective information. We need to identify, extract and quantify such details from the text for easier classification and working with the data.

# But why do we need sentiment analysis?

Sentiment analysis serves as a fundamental aspect of dealing with customers on online portals and websites for the companies. They do this all the time to classify a comment as a query, complaint, suggestion, opinion, or just love for a product. This way they can easily sort through the comments or questions and prioritize what they need to handle first and even order them in a way that looks better. Companies sometimes even try to delete content that has a negative sentiment attached to it.

sentiment

It is an easy way to understand and analyze public reception and perception of different ideas and concepts, or a newly launched product, maybe an event or a government policy.

Emotion understanding and sentiment analysis play a huge role in collaborative filtering based recommendation systems. Grouping together people who have similar reactions to a certain product and showing them related products. Like recommending movies to people by grouping them with others that have similar perceptions for a certain show or movie.

Lastly, they are also used for spam filtering and removing unwanted content.

# How does sentiment analysis work?
NLP or natural language processing is the basic concept on which sentiment analysis is built upon. Natural language processing is a superclass of sentiment analysis that deals with understanding all kinds of things from a piece of text.

NLP is the branch of AI dealing with texts, giving machines the ability to understand and derive from the text. For tasks such as virtual assistant, query solving, creating and maintaining human-like conversations, summarizing texts, spam detection, sentiment analysis, etc. it includes everything from counting the number of words to a machine writing a story, indistinguishable from human texts.

Sentiment analysis can be classified into various categories based on various criteria. Depending upon the scope it can be classified into document-level sentiment analysis, sentence level sentiment analysis, and sub sentence level or phrase level sentiment analysis.

Also, a very common classification is based on what needs to be done with the data or the reason for sentiment analysis. Examples of which are

Simple classification of text into positive, negative or neutral. It may also advance into fine grained answers like very positive or moderately positive.
Aspect-based sentiment analysis- where we figure out the sentiment along with a specific aspect it is related to. Like identifying sentiments regarding various aspects or parts of a car in user reviews, identifying what feature or aspect was appreciated or disliked.
The sentiment along with an action associated with it. Like mails written to customer support. Understanding if it is a query or complaint or suggestion etc
Based on what needs to be done and what kind of data we need to work with there are two major methods of tackling this problem.

Matching rules based sentiment analysis: There is a predefined list of words for each type of sentiment needed and then the text or document is matched with the lists. The algorithm then determines which type of words or which sentiment is more prevalent in it.
This type of rule based sentiment analysis is easy to implement, but lacks flexibility and does not account for context.
Automatic sentiment analysis: They are mostly based on supervised machine learning algorithms and are actually very useful in understanding complicated texts. Algorithms in this category include support vector machine, linear regression, rnn, and its types. This is what we are gonna explore and learn more about.
In this machine learning project, we will use recurrent neural network for sentiment analysis in python.

# Understanding the sentiment analysis system
Recurrent neural networks or RNNs are the go-to method for sequential data. Recurrent neural networks have a memory of their own and remember the input that was given to each node. In a normal feed forward neural network data or information given in the form of input moves forward and never moves backward in any nodes, from the input layer to the hidden layer and out from the output layer. Because these kinds of networks have no memory they do not remember the last input or predict the next input.

When giving out an output an rnn considers what input it is given and also the input that it had received previously, because the information moves in a cycle in an rnn.

#rnn vs fnn
![image](https://user-images.githubusercontent.com/72691866/190260140-679b25ef-335e-41c7-9ec9-f9a6195e300e.png)


What a recurrent neural network does is creates a copy of the output and loops it back through the network. For example when a sentence is passed through a feedforward network and it takes it word by word, till it reaches the last word. It has no memory of what was fed to it before that. But rnns know the previous inputs as well and can thus also predict what can come next. They are widely used in sequential data.

Recurrent neural networks are not new, were first introduced in the 1980s, but have become a lot popular with the growth of deep learning and its use in sequential data. Still, rnn have their own set of problems, one of the major ones being the vanishing gradient problem. The answer to that being the lstm model.

LSTM or long short term memory models are used to solve these problems. Lstms are a special kind of rnn model that has the capability of learning long term dependencies. They are made to remember long term data. What makes lstm models special is the addition of a memory cell, which is an extra recurrent state and each cell has multiple gates that control the flow of information in and out of the memory cell.

lstm for sentiment analysis

There are three types of gates in an lstm: an input gate, an output gate and a forget gate. The input gate is used to update the cell status, the forget state decides which information is to be stored and which needs to be discarded. The output gate determines the values for the next hidden gates.

# Building Sentiment Analysis System
Now that we have a basic understanding of what we need to build we will try implementing it in an easy way.

We will be building a simple sentiment analysis classifier on top of movie reviews, that will classify if the user review of the movie was positive, negative or neutral. For this sentiment analysis python project, we are going to use the imdb movie review dataset.

#What is Sentiment Analysis
Sentiment analysis is the process of finding users’ opinions towards a brand, company, or product. It defines the subject behind the social data, after launching a product we can find whether people are liking the product or not. There are many use-cases for sentiment analysis apart from opinion mining.
# Summary
![image](https://user-images.githubusercontent.com/72691866/190261792-88857307-bd9b-4a2a-9444-29b2bfd26fb6.png)

We have successfully developed python sentiment analysis model based on lstm techniques that is pretty robust and highly accurate. As discussed earlier, sentiment analysis has many use-cases based on requirements we can use it. We can similarly train it on any other kind of data just by changing the dataset according to our needs. We can use this sentiment analysis model in all different ways possible.
