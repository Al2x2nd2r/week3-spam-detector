# Email spam detector

## Features
- Detects whether an email is spam or not
- Uses measurable features like word count, exclamation marks, money-related terms and use of "ALL CAPS"
- Displays training and testing accuracy, along with confidence
- Creates an image of graphs depicting the spam assessments

## How the model works
This spam detector uses simple text-based features to classify example emails as spam or not spam. It looks for common spam indicators, such as excessive use of exclamation marks or words like “FREE” and “WIN.” The model learns from a small set of example emails and uses those patterns to make predictions. 

## How to Run
1. Clone the repository
2. Run: `python spam_detector.py'
3. The program will print out the feature table, training accuracy, test accuracy, and generate a png with graphs of the assessed information
4. You can enter your own custom email by entering the number of exclamation marks, the total word count, and the count of ALL CAPS words

## Sample Emails to Test
- WIN MONEY NOW!!!
- URGENT: Claim your prize!!!
- FREE OFFER LIMITED TIME

## What I Learned About Search
I learned how models use patterns in data instead of hard-coded rules to make predictions. I also learned that 100% accuracy might not actually always be a good thing, It could mean that the model is simply memorizing the examples and not actually learning. Finally, I learned about Overfitting, which happens when a model preforms perfectly on what its already seen, but fails on new data. This project helped me understand why real spam filters need vast, constantly updated datasets to work as intended.