# NLP

## Sentiment Analysis

- Text_Classification_Pytorch.ipynb: AG News data from pytorch, classified by news type. Use a simple MLP with the raw tokens. Result is quite good > 90% accuracy, probably because this is an easy task
- Sentiment_Analysis_Using_Universal_Sentence_Embedder: Twitter sentiments, labels look rather arbitrary . Using Universal Sentence Embedder and an MLP. Poor result currently 40% accuracy.
- sentiment-analysis-marketing/: using Amazon reviews data, and nltk python library. Rule based method

## Parsing text using Dependency parsing and Entity tagging libraries

- Resume parsing using spaCy, done in this [repo](https://github.com/hangjoni/resume-parsing)

TODO:

- pick one dataset, maybe Twitter dataset and try different methods with it
- Try ULMFit
- play with [this gensim-based movie genre plot project](https://github.com/RaRe-Technologies/movie-plots-by-genre) (comes with slides)
- play with the Annotated Transformers

# Today I learned

doc = nlp(
"In 1990, more than 60% of people in East Asia were in extreme poverty. "
"Now less than 4% are."
)
When two strings are placed together in python inside a function call, they are concatenated together. This is a convenience method to make code easy to read

# Foundations & Resources

## Transformers

- Transformer_walthrough.ipynb: code walk through of Transformers model.
- Building block of Transformers: Attention, Layer Normalization, Residual Connection, Collapsing then Expanding Linear connections
- When creating embedding with torch.Embedding() they has N(0, 1) distribution. Embeddings are scaled by the factor of sqrt(emb_size) before adding with positional embedding. This helps to reduce the impact of positional embedding in proportion to the word embedding. Inside Attention layers, we did a step of rescaling the embedding by 1/sqrt(emb_size) which get the mean and standard deviation to N(0, 1) back again

## spaCy

- a library for NER, dependency parsing, and pattern matching.
- This is [good book](http://spacy.pythonhumanities.com/02_01_entityruler.html) with project example for spaCy. PROGRESS: chapter 5

## gensim

- an optimized library for loading text into different file formats, word2vec and document similarity
