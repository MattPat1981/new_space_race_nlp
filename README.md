# Matt Paterson, Project 3: Web APIs & NLP
#### hello@hiremattpaterson.com

### Abstract

HireMattPaterson.com has been (fictionally) contracted by Virgin Galactic’s marketing team to build a Natural Language Processing Model that will efficiently predict if reddit posts are being made for the SpaceX subreddit or the Boeing subreddit as a proof of concept to segmenting the targeted markets. 

We’ve created a model that predicts the silo of the post with nearly 80% accuracy (with a top score of 79.9%).  To get there we tried over 2,000 different iterations on a total of 5 different classification modeling algorithms including two versions of Multinomial Naïve Bayes, Random Cut Forest, Extra Trees, and a simple Logistic Regression Classifier.  We’d like to use Support Vector Machines as well as Gradient Boosting and a K-Nearest Neighbors model in our follow-up to this presentation.

If you like our proof of concept, the next iteration of our model will take in to account the trend or frequency in the comments of each user; what other subreddits these users can be found to post to (are they commenting on the Rolex and Gulfstream and Maserati or are they part of the Venture Capital and AI crowd?); and if their comments appear to be professional in nature (are they looking to someday work in aerospace or maybe they already do).  These trends will help the marketing team tune their tone, choose words that are trending, and speak directly to each cohort in a narrow-cast fashion thus allowing VG to spend less money on ads and on people over time.

This notebook shows how we got there.


### Problem Statement

<ul><li>Virgin Galactic wants to charge customers $250K per voyage to bring customers into outer space on a pleasure cruise in null G</li>
<li>The potential customers range from more traditional HNWI who have more conservative values, to the Nouveau Riche, and various levels of tech millionaires in between</li>
  <li>Large teams of many Marketing Analysts and Marketing Managers are expensive</li>
<li>If you can keep your current headcount or only add a few you are better off, since as headcount grows, overall ROI tends to shrink (VG HC ~ 200 ppl)</li>
</ul>

---

### Solution

<ul><li>Create a machine learning model to identify what type of interests each user has based on their social media and reddit posts</li>

<li>Narrowcast to each smaller cohort with the language, tone, and vocabulary that will push each to purchase the quarter-million dollar flight</li>

---
**Additional Libraries**
This project utilizes the lebowski.py python library created and managed by Matt Paterson, hello@hiremattpaterson.com
