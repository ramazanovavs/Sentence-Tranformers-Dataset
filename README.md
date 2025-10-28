Experimental settings for fine-tuning Sentence Transformers. 
Training dataset: 
To fine-tune the model, a multilingual skills training dataset was created containing 9,336 paraphrase pairs in Russian, English, and Kazakh, as well as an additional set of 3,095 pairs in Russian.
Testing datasets: 
Validation and testing were performed on publicly available datasets such as STSB for English and RuSTSBenchmarkSTS for Russian.
Loss function: 
The model was tuned using the MultipleNegativesRankingLoss loss function, which is effective for dealing with pairs of similar texts such as paraphrases or repeated questions.
Evaluation of embedding model training: 
EmbeddingSimialityEvaluator - evaluates the model by computing the Pearson correlation and Spearman rank correlation between the computed embedding similarity and the gold standard labels of the test datasets.
Similarity Metrics: 
Semantic similarity of phrases was assessed using cosine similarity, Manhattan distance, Euclidean distance, and dot product similarity.


