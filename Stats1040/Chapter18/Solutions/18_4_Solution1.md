<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice
1. A university is interested in estimating the average daily commute time for its students. The population standard deviation is known to be 8 minutes. What sample size is needed to get a margin of error less than 3.0 for a 95% confidence interval?

## Solution
From the problem we get the following information:
* A confidence interval of 95% has a critical value of $$z_c = 1.96$$
* The population standard deviation is $$\sigma=8$$
* The desired margin of error is $$SE = 3.0$$

$$n = \left(\frac{z_c \sigma}{SE}\right)^2 \left(\frac{1.96\cdot 8}{3}\right)^2 = 27.32$$

Rounding up, __the required sample size is at least 28__.

[Return back to Lesson 18.4](../18_4_FindingN.md#practice)