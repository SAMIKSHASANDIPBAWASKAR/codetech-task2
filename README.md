# codetech-task2
<h1>INPUT</h1>
from textblob import TextBlob

# Sample sentences for sentiment analysis
sentences = [
    "I love programming!",
    "Python is an amazing language.",
    "I'm not a fan of bugs in the code.",
    "The weather today is gloomy.",
    "This project is going to be a success!"
]

# Function to analyze sentiment
def analyze_sentiment(sentences):
    for sentence in sentences:
        blob = TextBlob(sentence)
        sentiment = blob.sentiment
        print(f"Sentence: {sentence}")
        print(f"Sentiment: {sentiment}\n")

# Perform sentiment analysis
analyze_sentiment(sentences)
<h1>OUTPUT</h1>

Sentence: I love programming!
Sentiment: Sentiment(polarity=0.6000000000000001, subjectivity=0.6000000000000001)

Sentence: Python is an amazing language.
Sentiment: Sentiment(polarity=0.7000000000000001, subjectivity=0.6000000000000001)

Sentence: I'm not a fan of bugs in the code.
Sentiment: Sentiment(polarity=-0.1, subjectivity=0.5)

Sentence: The weather today is gloomy.
Sentiment: Sentiment(polarity=-0.3, subjectivity=0.5)

Sentence: This project is going to be a success!
Sentiment: Sentiment(polarity=0.5, subjectivity=0.5)














