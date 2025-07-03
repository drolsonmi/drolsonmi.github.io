<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice
1. A nutritionist wants to estimate the average number of cups of coffee consumed per week by graduate students. A random sample of 16 students __is taken from a normally-distributed population__. The sample shows a mean of 9.3 cups with a sample standard deviation of 2.1 cups. Construct a 90% confidence interval for the true mean weekly coffee consumption of graduate students.

## Solution
From the problem we get the following information:
* A confidence level of 90%
* Sample Size is $$n=16$$
* The sample mean is $$\bar{x} = 9.3$$
* The sample standard deviation is $$s=2.1$$

First, we verify the central limit theorem.
* Is the sample random? __Yes__ (stated in the problem)
* Is the sample large enough? __No__ (sample size is smaller than 30)
  * If it's not large enough, is the population normally distributed? __Yes__ (stated in the problem)

Now, we need to find the critical value. Since we only have a *sample standard deviation*, we need to find a critical *t-score*. With a 90% confidence interval and $$n-1 = 15$$ degrees of freedom, we find a critical value of $$t_c = 1.753$$.

<img src="../images/Fig18_5e_Practice1.png?raw=true" width="500" alt="Finding Critical Value for Practice Problem 1">

$$E = t_c\frac{s}{\sqrt{n}} = 1.753\frac{2.1}{\sqrt{16}} = 0.92$$

$$\bar{x} + E = 9.3 + 0.92 = 10.22$$

$$\bar{x} - E = 9.3 - 0.92 = 8.38$$

Solution:

__We are 90% confident that the average number of cups of coffee consumed by graduate students per week is between 8.38 and 10.22.__

[Return back to Lesson 18.5](../18_5_StudentT.md#practice)