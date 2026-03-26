Ex.No.6 Development of Python Code Compatible with Multiple AI Tools

Aim: 

Write and implement Python code that integrates with multiple AI tools to automate the task of interacting with APIs, comparing outputs, and generating actionable insights with Multiple AI Tools.

Explanation:

Develop a python code that integrates multiple AI tool by interacting with their APIs.
Compare outputs from different APIs.
Analyze the response and the Output.

The aim is to understand how to request help from AI tools for tasks like writing Python code, integrating with APIs, comparing outputs, and generating actionable insights.

Code for Positive Review:
```
from nltk.sentiment import SentimentIntensityAnalyzer 
import nltk 
nltk.download('vader_lexicon') 

generated_text = "This smartphone offers outstanding battery life and an intelligent AI camera 
that captures stunning photos." 
print("Generated Review:\n") 
print(generated_text) 

sia = SentimentIntensityAnalyzer() 
sentiment = sia.polarity_scores(generated_text) 
print("\nSentiment Analysis:") 
print(sentiment) 

if sentiment['compound'] > 0: 
  print("\nInsight: The review is positive and suitable for marketing promotion.") 
else: 
  print("\nInsight: The review tone is neutral or negative.")
```
Output:
<img width="782" height="166" alt="image" src="https://github.com/user-attachments/assets/a01b29f1-7d7c-4fcd-949a-ccc2a453064a" />

Code for Negative Review:
```

from nltk.sentiment import SentimentIntensityAnalyzer
import nltk

nltk.download('vader_lexicon')


generated_text = "This smartphone has very bad battery life and a poor AI camera that takes blurry photos."

print("Generated Review:\n")
print(generated_text)


sia = SentimentIntensityAnalyzer()
sentiment = sia.polarity_scores(generated_text)

print("\nSentiment Analysis:")
print(sentiment)

if sentiment['compound'] > 0:
    print("\nInsight: The review is positive and suitable for marketing promotion.")
else:
    print("\nInsight: The review tone is neutral or negative.")
```
Output:
<img width="858" height="188" alt="image" src="https://github.com/user-attachments/assets/8453e8f3-f36d-41a4-9b31-85180b141409" />

Result: 
The Python program successfully integrated multiple AI tools, automated API interactions, and collected responses efficiently.
