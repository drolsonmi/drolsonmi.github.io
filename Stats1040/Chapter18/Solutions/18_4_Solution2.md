<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice
2. A manufacturer claims that its LED light bulbs have an average lifespan of 1,200 hours. A consumer protection agency wants to verify this claim. The population standard deviation is known to be 100 hours. What sample size is needed to get a margin of error less than 35 for a 99% confidence interval?

## Solution
From the problem we get the following information:
* A confidence interval of 99% has a critical value of $$z_c = 2.58$$
* The population standard deviation is $$\sigma=100$$
* The desired margin of error is $$E = 35$$

$$n = \left(\frac{z_c \sigma}{E}\right)^2 \left(\frac{2.58\cdot 100}{35}\right)^2 = 54.34$$

Rounding up, __the required sample size is at least 55__.

[Return back to Lesson 18.4](../18_4_FindingN.md#practice)