Ex.No.6 Development of Python Code Compatible with Multiple AI Tools

Aim: 

Write and implement Python code that integrates with multiple AI tools to automate the task of interacting with APIs, comparing outputs, and generating actionable insights with Multiple AI Tools.

Explanation:

Develop a python code that integrates multiple AI tool by interacting with their APIs.
Compare outputs from different APIs.
Analyze the response and the Output.

The aim is to understand how to request help from AI tools for tasks like writing Python code, integrating with APIs, comparing outputs, and generating actionable insights.
program:

positive statement:

```
from nltk.sentiment import SentimentIntensityAnalyzer
import nltk

nltk.download('vader_lexicon')

# Simulated AI-generated text
generated_text = "This laptop delivers lightning-fast performance with a sleek design and long-lasting battery for all-day productivity."

print("Generated Review:\n")
print(generated_text)

# Sentiment analysis
sia = SentimentIntensityAnalyzer()
sentiment = sia.polarity_scores(generated_text)

print("\nSentiment Analysis:")
print(sentiment)

# Insight generation
if sentiment['compound'] > 0:
    print("\nInsight: The review is positive and suitable for marketing promotion.")
else:
    print("\nInsight: The review tone is neutral or negative.")
```

output:
```
Generated Review:

This laptop delivers lightning-fast performance with a sleek design and long-lasting battery for all-day productivity.

Sentiment Analysis:
{'neg': 0.0, 'neu': 1.0, 'pos': 0.0, 'compound': 0.0}

Insight: The review tone is neutral or negative.
[nltk_data] Downloading package vader_lexicon to /root/nltk_data...
```

negative statement:
```
from nltk.sentiment import SentimentIntensityAnalyzer
import nltk

nltk.download('vader_lexicon')

# Simulated AI-generated text
generated_text = "This laptop suffers from slow performance, a bulky design, and poor battery life that struggles to last through the day."

print("Generated Review:\n")
print(generated_text)

# Sentiment analysis
sia = SentimentIntensityAnalyzer()
sentiment = sia.polarity_scores(generated_text)

print("\nSentiment Analysis:")
print(sentiment)

# Insight generation
if sentiment['compound'] > 0:
    print("\nInsight: The review is positive and suitable for marketing promotion.")
else:
    print("\nInsight: The review tone is neutral or negative.")
```

output:
```
Generated Review:

This laptop suffers from slow performance, a bulky design, and poor battery life that struggles to last through the day.

Sentiment Analysis:
{'neg': 0.352, 'neu': 0.648, 'pos': 0.0, 'compound': -0.8271}

Insight: The review tone is neutral or negative.
[nltk_data] Downloading package vader_lexicon to /root/nltk_data...
[nltk_data]   Package vader_lexicon is already up-to-date!
```






Result: 
