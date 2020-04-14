# RECOMMENDER SYSTEMS WITH RECURRENT NEURAL NETWORKS (A feature-rich session-based RecSys) #

This work has been completed in cooperation with prudsys AG in Berlin, where I currently work as a researcher (working student) in department of Consulting & Data science.

Recommender systems are beneficial to both users and companies that provide services. Proper recommendations can support users to find what they are looking for more easily and faster. Additionally, recommender systems can help users discover new content and improve user experience and engagement. Over the last years, many works have been done on the use of Recurrent Neural Networks (RNNs) in the case of recommender systems. Results were positive and promising, especially in the session-based setting where RNNs were shown to outperform state-of-the-art models. In many of these experiments, the RNN could potentially improve its recommendations by utilizing information about past sessions of a user, in addition to his interactions in the current session. An issue for session-based recommenders, is how to generate more accurate recommendations using more information about the session, specifically items.

We propose an approach that extends the existing session-based RNN-based recommender system, making it able to process the information about the item to improve recommendations. This is done by using item features and adding an RNN layer for each item feature to learn from various information that items provide and predict the user’s interest for the next click. By feeding this information to the RNN layer, the proposed solution is able to improve its recommendations.

Our experiments on our dataset, show that the proposed approach can significantly improve recommendations throughout the sessions, compared to using a single RNN working only on the sequence of IDs. The proposed model especially improves recommendations when applying the embedded representation of both IDs and features of items.


## Poster ##

![Poster](https://github.com/Vahidsj/ModelingSeminar/blob/master/RecSys%20with%20RNN%20-%20Poster.png)


## Goals and Research Questions ##

Real-life recommender systems often face the daunting task of providing recommendations based only on the clicks of a user session. However, the items typically have rich feature representations such as text descriptions that can be used to model the sessions. We want to find out how contextual information can be incorporated into an RNN based session-based recommender system. The goal of this research is therefore to implement an RNN-based session-based recommender system, that also considers the information about items. We want to find out how the model performs as a recommender system.
Intuitively, RNNs improve their sequence predictions throughout a sequence, after having learned from the earlier items. Since our proposed model supply the RNN with additional information about the session, it should be able to make stronger recommendations.

**•	Research question 1:** 
Can an RNN be used to learn from previous sessions, and thus produce information about the next click?

**•	Research question 2:** 
How can the features of items be represented and exploited in Recurrent Neural Network session-based models using deep learning, which can help improve recommendations from the straightforward session based RNN recommendation system implementation?
