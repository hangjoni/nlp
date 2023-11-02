# NLP 

## Sentiment Analysis
- Text_Classification_Pytorch.ipynb: AG News data from pytorch, classified by news type. Use a simple MLP with the raw tokens. Result is quite good > 90% accuracy, probably because this is an easy task
- Sentiment_Analysis_Using_Universal_Sentence_Embedder: Twitter sentiments, labels look rather arbitrary . Using Universal Sentence Embedder and an MLP. Poor result currently 40% accuracy.
- sentiment-analysis-marketing/: using Amazon reviews data, and nltk python library. Rule based method

TODO:
- pick one dataset, maybe Twitter dataset and try different methods with it
- Try ULMFit
- Try SpaCy - is an NLP package and framework, like NLTK?, but seems more popular and well documented


# Today I learned
doc = nlp(
    "In 1990, more than 60% of people in East Asia were in extreme poverty. "
    "Now less than 4% are."
)
When two strings are placed together in python inside a function call, they are concatenated together. This is a convenience method to make code easy to read
