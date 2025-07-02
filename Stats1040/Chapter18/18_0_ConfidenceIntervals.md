<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

# Lesson 18: Confidence Intervals with 1 Sample Means
Knowing the __Central Limit Theorem__, we are ready to make our first inference. By __inference__, we mean that we are using our sample to infer information about the population. 

This is really what we wanted from the beginning of the course. We can't actually find the average weight of all Americans, but if we find a sample average, we can find an approximation of the true average.

The first inference we will make is known as the __Confidence Interval__. Using the sample average, we can formulate a range of values in which we can say the true value is (at least with some certainty).

For example, if we take the weights from a sample of 250 Americans and find a sample mean of 175 pounds with a standard deviation of 25 pounds, let's quickly find a confidence interval with a 90% certainty (also known as a confidence level).
* We calculate a __margin of error__: 2.61 pounds
* We create the boundaries of our __confidence interval__:
    * Upper boundary: 175 pounds + 2.61 pounds = 177.61 pounds
    * Lower boundary: 175 pounds - 2.61 pounds = 172.39 pounds
    * The confidence interval:
      * $175 \pm 2.61 pounds
      * (172.39, 177.61)
* We __interpret__ the confidence interval
    * We can say with 90% certainty that the true average weight of Americans is between 172.39 pounds and 177.61 pounds

This doesn't give an exact number, but it gives us a good approximation.

Over the next few pages, we'll look at how to find the confidence interval. In this lesson, we will focus on a single sample of quantitative data

## Topics in this lecture
* 18.1 Critical Values
* 18.2 Margin of Error
* 18.3 Confidence Interval with 1 Sample Means