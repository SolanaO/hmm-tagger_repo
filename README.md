## Part of Speech Tagging

Part of speech tagging is the process of determining the syntactic category of a word from the words in its surrounding context. It is often used to help disambiguate natural language phrases because it can be done quickly with high accuracy. Tagging can be used for many NLP tasks such as for information retrieval or for word sense disambiguation.

The project is built on a template provided by Udacity. The approach uses the _Pomegranate library_ to build a _Hidden Markov Model (HMM)_ for part of speech tagging using an 'universal' tag set. Hidden Markov models have been able to achieve more than 96% tag accuracy with larger tag sets on realistic text corpora. These models have also been used for speech recognition and speech generation, machine translation, and human gesture recognition for computer vision, and more.

There are two taggers constructed in this project. First a Most Frequent Class tagger to use as a baseline is built. A good baseline for tagger performance is to simply choose the tag most frequently assigned to each word. This 'most frequent class' tagger inspects each observed word in the sequence and assigns it the label that was most often assigned to that word in the corpus.

The HMM tagger has one hidden state for each possible tag, and is parameterized by two distributions: the emission probabilities giving the conditional probability of observing a given word from each hidden state, and the transition probabilities giving the conditional probability of moving between tags during the sequence.




