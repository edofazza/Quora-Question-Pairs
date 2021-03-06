# Quora Question Pairs
Quora is a question-and-answer platform where users can post questions and answers on any topic. Quora groups questions and answers by topics and allows users to vote or add comments. Also, users can collaborate by editing questions or suggesting changes to answers provided by other users.

Since new questions are posted every day, there is a high probability that some of them are literally the same or have similar intent, which creates unnecessary duplicates in both questions and answers. This can be data-heavy and can result in a degradation of the user experience. Indeed, multiple questions with the same intent can cause seekers to spend more time finding the best answer to their question and make writers feel they need to answer multiple versions of the same question. As a result, the answers get fragmented across different versions of the same question. For example, the questions “What’s the fastest way to get from Los Angeles to New York?” and “How do I get from Los Angeles to New York in the least amount of time?” are the same question but asked differently. 

In order to identify duplicate questions and perhaps merge them into a single post, it is crucial to be able to understand their semantics and compute their similarity. Natural Language Processing (NLP) technologies can help solve this challenging task.

In this project, after a brief analysis of the available data, we attempted to solve the task of assessing the similarity of question pairs using three different approaches. First, we tried to build an LSTM architecture on an embedding layer trained from scratch. Next, we built a Siamese neural network inspired by the literature, leveraging pre-trained word embeddings. Later, we took a transfer learning approach by using features extracted from pre-trained models to train a deep neural network. 

At the end, we analyzed the errors made by our best models to evaluate whether or not to resort to an ensemble model. 
The results obtained with the ensemble are encouraging and show that it is possible to correctly classify almost all questions pairs, with a macro-F1 score of 88.13%.

You can find more information in the documentation [here](Documentation.pdf).
