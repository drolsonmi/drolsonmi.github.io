<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice
2. A tech company tests a new phone battery. A sample of 30 phones, coming from a normally-distributed population, shows an average battery life of 22.4 hours with a sample standard deviation of 3.5 hours. Construct a 99% confidence interval for the true mean battery life of the new phone model.

## Solution
From the problem we get the following information:
* A confidence level of 99%
* Sample Size is $$n=30$$
* The sample mean is $$\bar{x} = 22.4$$
* The sample standard deviation is $$s=3.5$$

First, __verify the central limit theorem__
* Is the sample random? __Yes__ (stated in the problem)
* Is the sample large enough? __Yes__ (sample size is at least 30)

The Central Limit Theorem holds.

Now, we find the critical value. Since we only have a sample standard deviation, we need to use the t-score with $$DF = n-1 = 29$$ degrees of freedom. Doing this, we get $$t_c = 2.756$$.

$$E = t_c\frac{s}{\sqrt{n}} = 2.756\frac{3.5}{\sqrt{30}} = 1.76$$

$$\bar{x} + E = 22.4 + 1.76 = 24.16$$

$$\bar{x} - E = 22.4 - 1.76 = 20.64$$

Solution:

__We are 99% confident that the true mean for battery life is between 20.64 and 24.16 hours.__

[Return back to Lesson 18.5](../18_5_StudentT.md#practice)