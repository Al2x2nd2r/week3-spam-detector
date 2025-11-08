# Spam Detection Analysis Report
## How My Model Learns
### Features I Used

1. **Word Count**: 
Spam messages usually have shorter or overly long word counts. Short messages like "CONGRATS YOU WON!" or "WIN CASH NOW!" try to grab attention as quickly as possible.
While longer spam messages may include more keywords or filler to try and bypass any filters.

2. **Exclamation Marks**:
Spammers often use exclamation marks to create urgency or excitement. Even if you dont actually click it, a title like "CLICK HERE NOW!!!!!" is going to get your attention more than any regular message.

3. **Money Words**: 
Words such as "free," "win," "cash," "prize," "earn," "money," or any form of "congratulations" are typically strong indicators of spam because they promise rewards to lure the reader in.

4. **ALL CAPS**: 
Spam messages also often use all caps to generate a sense of urgency or excitement. As previously mentioned, even if you arent actually clicking anything similar to "CONGRATULATIONS!" or "ACT NOW!" messages like those are more likely to at least grab your attention.

## Training Results
- Training Accuracy: 100%
- Testing Accuracy: 100%

### What This Means
The spam detector predicts all of the messages correctly, but that doesn’t mean it’s actually accurate in real situations. It probably just memorized those exact patterns instead of truly learning what spam looks like.

## Preventing Overfitting
Since my data was very small, it’s easy for the model to “memorize” it. To prevent that, I could use a much larger and more varied dataset, shuffle the examples, or add new unseen test messages.

## Real-World Application
If this was used by Gmail:
- Strengths: Works on simple or very obvious spam emails. Easy and fast to run. Demonstrates how spam detection works.

- Weaknesses: Unreliable for real emails as it was only trained on very limited examples. Might mark normal messages as spam or miss any new spam types. Doesnt actually understand language/context/sentiments, it is based off of variables such as Exclamation points, all caps, and keywords.

- Improvements needed: Train with an abundance of real emails. Add natural language processing or deep learning. Regularly update the model to detect any new types of spam emails.

## What I Learned
I learned how models use patterns in data instead of hard-coded rules to make predictions. I also learned that 100% accuracy might not actually always be a good thing, It could mean that the model is simply memorizing the examples and not actually learning. Finally, I learned about Overfitting, which happens when a model preforms perfectly on what its already seen, but fails on new data. This project helped me understand why real spam filters need vast, constantly updated datasets to work as intended.