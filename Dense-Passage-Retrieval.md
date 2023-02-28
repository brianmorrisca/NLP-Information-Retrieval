# Dense Passage Retrieval
Dense Passage Retrieval (DPR) is a technique used in natural language processing (NLP) for information retrieval, specifically for question-answering tasks. DPR is a hybrid method that combines the strengths of dense vector-based retrieval and sparse BM25 retrieval.

In traditional sparse retrieval methods, the text is indexed based on sparse representations of individual words or n-grams. However, this approach does not capture the full semantic meaning of the text, leading to suboptimal retrieval results. On the other hand, dense vector-based retrieval methods like BERT (Bidirectional Encoder Representations from Transformers) can capture more of the contextual information and meaning of the text.

DPR works by encoding both the question and the context (or document) into dense vectors using a neural network, such as BERT. These vectors are then used to compute a similarity score between the question and the context. The similarity score indicates the relevance of the context to the question, and the top-ranking contexts are returned as candidate answers.

To improve efficiency, DPR uses a two-stage approach: first, a candidate set of contexts is retrieved using BM25, a sparse retrieval method. Then, the dense vector similarity score is computed only for the candidate contexts, reducing the computational cost of encoding all the contexts.

DPR has shown state-of-the-art performance on several benchmark question-answering datasets, such as Natural Questions and TriviaQA. It has also been shown to be effective in multi-task learning scenarios, where a single DPR model can be trained for both retrieval and question answering tasks.



# The Illustrated Dense Passage retriever 
https://ankur3107.github.io/blogs/dense-passage-retriever/
