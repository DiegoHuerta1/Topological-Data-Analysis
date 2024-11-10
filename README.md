# Topological-Data-Analysis
Implementation of topological data analysis algorithms. Specifically, applying Mapper, Vietoris-Rips filtration, homology, and persistent homology with various datasets.

The code is implemented in Spanish.

## MAPPER


BERT models (Bidirectional Encoder Representations from Transformers) are neural networks widely used in natural language processing (NLP) and represent the state-of-the-art for various linguistic tasks. Generally, these models take a sequence of words (a sentence) as input and generate a series of vectors, one for each word in the sequence, along with a special vector associated with a token called "CLS."
BERT models undergo a pre-training process that addresses two primary tasks: language modeling and next sentence prediction. This pre-training enables them to capture a deep understanding of the structure and use of natural language. After this phase, these models can undergo fine-tuning, where specific adjustments are made to adapt them to particular tasks. This typically involves training an additional layer, such as a classification layer, on top of the original model.

A key feature of BERT models is their ability to generate sentence embeddings. This is achieved through a pooling process, where the representation vector for the sentence is obtained from the "CLS" token in the last layer of the BERT model. The "CLS" token contains condensed information about the sentence in its context and is used as the representation of the entire sentence.

The vectors generated by a BERT model typically reside in a 768-dimensional space, corresponding to the model's last layer. Thus, the process of generating sentence embeddings with BERT can be conceptualized as a function 
$f : O \rightarrow \mathbb{R}^{768}$,
where $O$ is the space of sentences. In other words, the resulting embedding from a BERT model transforms a sentence into a 768-dimensional vector.

This part of the project focuses on analyzing the topological structure of embeddings generated by a BERT model that has been fine-tuned specifically for sentiment classification. The main objective is to explore and understand the structure of this space; that is, to study $f(O)$ as a topological space. To achieve this, a dataset of sentences expressing emotions is collected, and the corresponding embeddings are computed using the CLS pooling process on the last layer of the fine-tuned BERT model. Subsequently, the Mapper algorithm is applied to visualize the topological structure of these vectors in high-dimensional space. This exploration allows a deeper understanding of how sentiment representations are organized in the embedding space and help identify significant patterns or clusters within the data.














