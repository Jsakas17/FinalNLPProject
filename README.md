**Objective**

The objective was to examine whether the addition of syntactic information (POS Tags) to the Word Embedding improves the performance of sentiment classification in Movie reviews.

**Steps**

Data loading was performed using the SST2 (Stanford Sentiment Treebank) dataset, which contains short texts with binary sentiment tagging (positive/negative).

**Preprocessing** involved tokenization, lemmatization, and the removal of stopwords. Additionally, each word was assigned a POS tag.

For word embedding, two versions were used. The regular version calculated the average of embeddings based on words only. The second version merged the words and POS tag for each word (example for what we did is: "love_VERB"), and then used the embedding based on the new words.

**Two types of models were employed**. A basic model,Simple MLP. And a more advanced model, LSTM (Long Short-Term Memory), operated on a sequence of words, with or without the addition of POS tags.
