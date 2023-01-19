# Voting-Classifier---Combine-Your-ML-Models-for-Better-Results

The voting classifier is an ensemble learning method that combines several base models to produce the final optimum solution. We create a single model which trains by these models and predicts output based on their combined majority of voting for each output class.

The algorithm aggregates the results of each classifier passed into Voting Classifier and predicts the output class based on the highest majority of voting.

Since voting relies on the performance of many models, they will not be affected by large errors or misclassifications from one model. In other words poor performance from one model can be offset by a strong performance from other models.

## Hard voting

Hard voting (also known as majority voting). The models predict the output class independent of each other. The output class is a class with the highest majority of votes.

Suppose three classifiers predicted the output class(A, A, B), so the majority predicted A as an output. Therefore A will be the final prediction.

## Weighted Majority Voting

In addition to the simple majority vote (hard voting) as described in the previous section, we can compute a weighted majority vote by associating a weight w with classifier C.

## Soft Voting

In soft voting, the output class is the prediction based on the average of probability given to that class. Soft voting entails combining the probabilities of each prediction in each model and picking the prediction with the highest total probability.

Each base model classifier independently assigns the probability of occurrence of each type. In the end, the average of the possibilities of each class is calculated, and the final output is the class having the highest probability.

Suppose given some input to three models, the prediction probability for class A = (0.30, 0.47, 0.53) and B = (0.20, 0.32, 0.40). So the average for class A is 0.4333 and B is 0.3067, the winner is clearly class A because it had the highest probability averaged by each classifier.
