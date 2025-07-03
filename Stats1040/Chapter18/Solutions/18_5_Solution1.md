<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice
1. A nutritionist wants to estimate the average number of cups of coffee consumed per week by graduate students. A random sample of 16 students shows a mean of 9.3 cups with a sample standard deviation of 2.1 cups. Construct a 90% confidence interval for the true mean weekly coffee consumption of graduate students.

## Solution
From the problem we get the following information:
* A confidence level of 90%
* Sample Size is $$n=16$$
* The sample mean is $$\bar{x} = 9.3$$
* The sample standard deviation is $$s=2.1$$

First, we verify the central limit theorem.
* Is the sample random? __Yes__ (stated in the problem)
* Is the sample large enough? __No__ (sample size is smaller than 30)
  * If it's not large enough, is the population normally distributed? __No__ (not stated in the problem)

At this point, __we can't solve the problem because the Central Limit Thereom does not hold.__

[See the solution if the problem is modified so the CLT holds](18_5_Solution1b.md)

[Return back to Lesson 18.5](../18_5_StudentT.md#practice)