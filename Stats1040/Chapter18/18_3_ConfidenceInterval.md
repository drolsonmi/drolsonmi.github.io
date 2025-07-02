<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

# Lesson 18.3 Confidence Interval
## Reading
* 7.1.1 Using the z-distribution for inference when $$\mu$$ is unknown and $$\sigma$$ is known (pages 277 of the [Introduction to Statistics Textbook](../Resources/OpenIntroTextbook.pdf))

## Lesson
We are going to apply what we have learned in a specific scenario. This is the problem we will work on:

> American mental abilities are often measured by an IQ test.  The IQ distribution is normal with a mean of 100 and a population standard deviation of 15.  
> 
> A random sample of 40 Snow College students is taken and they have an average IQ of 106.3. What is the true average IQ of Snow College students?

We'll find a 90% confidence interval to find this true average. As we discussed, we need to do the following to find the confidence interval:
1. Find the Critical Values
2. Find the Margin of Error
3. Find the Confidence Interval
4. Interpret the Confidence Interval

#### Find the Critical Values
We are given a confidence level( of 90%.
* The remaining 10% is in the two tails, 5% in each tail
* The z-scores that separate the two tails are $$\pm$$1.645.

#### Find the Margin of Error
The equation for the margin of error is $$SE = z_c\tfrac{\sigma}{\sqrt{n}}$$.
* $$z_c = \pm 1.645$$ is the critical value
* $$\sigma = 15$$ is the population standard deviation
* $$n = 40$$ is the sample size

Plugging these in,
$$\begin{align*}
SE &= z_c\frac{\sigma}{\sqrt{n}} \\
   &= \pm 1.645 \frac{15}{\sqrt{n}} \\
   &= \frac{\pm 24.675}{6.3246} \\
   &= \mathbf{3.90}
\end{align*}$$

#### Find the Confidence Interval
The boundaries to our confidence interval are the sample mean ($$\bar{x}$$) plus or minus the margin of error ($$SE$$).
* $$\bar{x} = 106.3$$
* $$SE = 3.90$$

$$\bar{x} + SE = 106.3 + 3.901 = 110.20  \qquad  \bar{x} - SE = 106.3 - 3.901 = 102.4$$

The confidence interval is,

$$\mathbf{(102.4, 110.2)}$$

#### Interpret the Confidence Interval
The goal was to find the true average IQ of Snow College students. Although we couldn't find an exact value, we can find the confidence interval, which is a range of values the true average could be in. So, we take this goal and apply it to the confidence interval we just found.

Here is a proper interpretation of the confidence interval:

> __We are 90% confident that the true average of Snow College student IQ scores is between the values of 102.4 and 110.2.__

## Practice