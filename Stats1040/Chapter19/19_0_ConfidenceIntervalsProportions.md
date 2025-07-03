<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

# Lesson 19: Confidence Intervals with 1 Sample Proportions
Let's turn our attention to Categorical Data. That means we will shift our attention from means and standard deviations, and we will use proportions.

A few things to note while using proportions:

Since we aren't working with standard deviations, we don't have to worry about whether we have it or not. So, we will ALWAYS be using the z-score. The t-score will not appear at all whenever we are using proportions.

Remember that a proportions always have a value between 0 and 1. That means that the boundaries for our confidence intervals will also be between 0 and 1.

For interpreting, we can add a level of understanding. If both of the boundaries of our confidence interval are above 0.50, then we are quite confident that we have a majority. 

## Quick example
Presidential elections are a great example of this. Election committees often put out surveys to see if citizens in a state will vote for a given candidate. Let's say that in Utah, a survey to determine whether citizens vote republican or not shows a 99% confidence interval of (0.65, 0.8).

Since we are 99% confident that the overall proportion of Utah citizens that vote republican is between 0.65 and 0.80 (between 65% and 80%), then we are very confident that the state will vote republican.

Next presidential election, watch the news when polls close. You'll see that they will declare Utah as republican before they count a single vote. This is because the confidence interval is so clearly in the majority.

## Topics in this lecture
So, in this lesson, we'll learn how to find the confidence interval for categorical data using proportions.
* 19.1 Critical Values
* 19.2 Confidence Intervals with 1 Sample Proportions