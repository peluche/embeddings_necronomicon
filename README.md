# nano-word2vec

This is meant as a small experiment to get my hands dirty with word embeddings.


The rough outline is:
- find a small enough dataset of english sentences on huggingface
- train next word prediction using a code very similar to Karpathy's Makemore
- throw away the head of the model and only keep the embeddings layer
- try to do some kNN-ish to find words related to other words
- try to reproduce some word arithmetic: king - man + woman and see if we can get to queen
