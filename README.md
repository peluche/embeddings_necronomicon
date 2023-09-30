# Embeddings Necronomicon

This is meant as a small experiment to get my hands dirty with word embeddings.

The original idea was to try to reproduce the word arithmetic examples from Google's Word2Vec demo: `King - Man + Woman = Queen` and `Paris - France + Italy = Rome`.

(Spoiler alert) but it turned out to be more of an experiment on how to create/handle/visualize word embeddings. Even using `Gensim.word2vec` with the google-news pre-trained weights or `Bert` embeddings from huggingface I couldn't get to the same results as the original demo.


## Word2Vec hatchling
For the manual attempt in `embeddings_necronomicon.ipynb` the rough outline is:
- find a small enough dataset of english sentences on huggingface
- train next word prediction using a code very similar to Karpathy's Makemore
- throw away the head of the model and only keep the embeddings layer
- try to reproduce some word arithmetic: king - man + woman and see if we can get to queen

## PCA (Principal Component Analysis)
I also did a bit of a deepdive into PCA and re-implemented a fair bit of it by hand with cool visualizations in `pca.ipynb`.
