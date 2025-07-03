<head>
<title>18.5 Confidence Intervals when you don't know the population standard deviation</title>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

# Lesson 18.5 Confidence Interval when you don't know $$\sigma$$
## Reading
* 7.1.2 Introducing the t-distribution (pages 278-281 of the [Introductory Statistics Textbook](OpenIntroTextbook.pdf))
* 7.1.3 The t-distribution and the standard error of a mean (page 281 of the [Introductory Statistics Textbook](OpenIntroTextbook.pdf))
* 7.1.5 One sample t-intervals (pages 282-285 of the [Introductory Statistics Textbook](OpenIntroTextbook.pdf))

## Lesson
Consider this problem:
> A health researcher wants to estimate the average number of hours of sleep that college students get on weeknights. A random sample of 25 students is taken, and the sample yields a mean of 6.8 hours with a sample standard deviation of 1.2 hours.
> 
> Construct a 95% confidence interval for the true mean number of hours of sleep college students get on weeknights.

Notice that in this case, we do not have a population standard deviation ($$\sigma$$). So, our Margin of Error calculation won't work.

Fortunately, we have a solution. The normal distribution depends on the population. Another distribution that we call the __t-distribution__ depends instead on the sample. This is a good approximation of the normal distribution.

With the t-distribution, we find a critical value from t-scores and use the sample standard deviation to find the margin of error.

$$SE = t_c\frac{s}{\sqrt{n}}$$

However, since the t-distribution relies on the sample, we also have to consider one more variable:
* The __Degrees of Freedom__ is calculated as $$DF = n-1$$
* As $$n$$ increases, the t-distribution becomes a better approximation of the normal distribution.

<img src="images/Fig18_5_tDistributions.png?raw=true" width="500" alt="T-Distributions with varying degrees of freedom">

## Practice
1. ?
    * [After solving on your own, see solution here](Solutions/18_5_Solution1.md)
2. ?
    * [After solving on your own, see solution here](Solutions/18_5_Solution2.md)
3. ?
    * [After solving on your own, see solution here](Solutions/18_5_Solution3.md)

## Technology
### TI-83/84
### Excel
### Desmos