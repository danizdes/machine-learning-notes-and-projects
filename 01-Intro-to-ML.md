# Introduction
This was the first "course" I took, it was [Googles Intro to Machine Learning Foundational Course](https://developers.google.com/machine-learning/intro-to-ml). I completed the entire thing in about ~15 minutes.

## Supervised Learning

Supervised learning is when a model looks at a bunch of data with the **correct answers** and tries to find patterns to predict the correct answer.

Use cases include:

- Regression model: It predicts a numerical value, for example the price of a home, or time in minutes and seconds to arrive at a destination.
- Binary Classification: This predicts whether something is in a specific category, unlike regression which predicts a numerical value. In binary classification there are only 2 classes that the model can predict, for example a model following binary classification can predict `rain` or `no rain` *only*.
- Multiclass Classification: This is similar to binary classification but now can predict more than 2 classes. Using a similar example from above, instead of only `rain` or `no rain` it can predict `rain`, `hail`, `snow`, or `sleet`

## Unsupervised learning

The major difference between this and supervised learning, is that this model does not have any of the answers. The models aim is to look at supporting data and find meanigful patterns and come up with the answer. A common technique models like these use is called **clustering** where the model will find groups of data points that create natural groupings.

## Reinforcement Learning

This model makes predictions by getting rewards and/or penalties based on the actions it performs in an environment (for example, in a game ). A model like this generates a **policy** that defines the best actions to get the most rewards.

## Generative AI

This model can create unique content from user input. This includes:

- Text-to-Text: ex: Chatgpt
- Text-to-Image: ex: Midjourney
- Text-to-Video: ex: Sora
- Image-to-Text: ex: Chatgpt

Generative AI first is trained through unsupervised learning, to give it the ability to produce unique content. It can then be trained using supervised learning or reinforcement learning on specific data that the model might be asked of.

# A deeper dive into supervised learning

## Introduction

Data is the main thing that drives Machine Learning, it is commonly arranged in a datasheet where related data are stored. A datasheet includes:

- Features: Supporting data the model can use to sense patterns
- Label: The "answer", what we want the model to predict

A datasheet with the features and labels are called "labeled examples"

A datasheet is characterized by it's **diversity** and it's **size**. Size is the number of examples we have. Diversity is the range that those examples cover. Both a high diversity and large size'd datasheet make a good datasheet to train a ML model.

## Training

This is how a model is trained:

1. The model takes a single labelled example in the datasheet, and then predicts the label or answer.
2. It then compares it's predicted value with the actual value found in the datasheet.
3. It then updates it's methods to more closely match the actual value.
4. The model repeats this for the entire datasheet

## Evaluate

To evaluate the model- meaning simply to see how closely it's predictions match the actual value, this is how it's done:

1. We use the **trained** ML model and feed it the datasheet, this time however we do not provide it with the label
2. The model then predicts it's possible values for the label
3. We can then compare it's predicted value to the actual value and this evaluate the model