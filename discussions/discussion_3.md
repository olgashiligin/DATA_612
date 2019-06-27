---
title: "discussion 3"
author: "Olga Shiligin"
date: "27/06/2019"
output: html_document
---


Recommender systems can be a powerful tool for increasing reader engagement, and encouraging contribution, and filling knowledge gaps. However, recommender systems, like all machine-learning applications, have the potential to reflect and reinforce harmful biases. Sources of bias in machine learning applications can stem from a wide variety of sources, such as:

- limitations in training data
- social and analytical assumptions of system developers
- technical limitations of software infrastructure, and
- evolving social norms [3]

 Recommender Systems can reinforce human bias because the largest subgroup of users will dominate overall statistics; if other subgroups
have different needs, their satisfaction will carry less weight in the final analysis. This can result in an incomplete picture of the performance of the system and and obscure the need to identify how to better serve specific demographic groups.

I have found the following types of recommender system bias:

- popularity bias (where the evaluation protocol gives higher accuracy scores to algorithms that favor popular items irrespective of their ability to meet user information needs)
- misclassified decoys (where a good recommendation is erroneously penalized because data on user preferences is incomplete.)
- demographic bias ( the patterns of the largest group of users will dominate the list of most-popular items, so favoring popular recommendations will also favor recommendations that are more likely to match the taste of the dominant group of users at the expense of other groups with different favorite items). 

I think there are a lot of examples of recommender systems bias, I would consider the following ones:

- Racial Bias: software COMPAS has being used to forecast which criminals are most likely to reoffend. The software estimates how likely a defendant is to re-offend based on his or her response to 137 survey questions. It was discovered that the COMPAS algorithm was able to predict the particular tendency of a convicted criminal to reoffend. However, when the algorithm was wrong in its predicting, the results was displayed differently for black and white offenders. (ProPublica non-profit news organisation). [7]

- The youtube recommender system designed is a such way that YouTube pushes an anonymous user toward more popular, not more fringe, content leaving the space for manipulation of users preferences. Youtube recommender system algorithm seems to have concluded that people are drawn to content that is more extreme than what they started with — or to incendiary content in general. [6]

- In the MovieLens 1M and LastFM 1K data sets, men receive better recommendations than women.

- In the LastFM 360K data set, old (50+) and young (under 18) receive better recommendations than other age groups.[2]


 What is even more important is the long-term effect of recommender system bias: for large values of bias the recommender has a reinforcing effect, which in the long term will lead to polarized groups of users (research was done on synthetically generated data).[1]


Sources:

1. https://arxiv.org/pdf/1811.01461.pdf
2. https://md.ekstrandom.net/pubs/demographics-of-cool-summary.pdf 
3. https://meta.wikimedia.org/wiki/Research:Ethical_and_human-centered_AI/Bias_in_recommender_systems
4. http://proceedings.mlr.press/v81/ekstrand18b/ekstrand18b.pdf
5. https://pdfs.semanticscholar.org/7bdb/7a97b448b9b3a7fd242de777dcb3bc6ea019.pdf
6. https://www.theatlantic.com/technology/archive/2018/11/how-youtubes-algorithm-really-works/575212/
7. https://medium.com/thoughts-and-reflections/racial-bias-and-gender-bias-examples-in-ai-systems-7211e4c166a1