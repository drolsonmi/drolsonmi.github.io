<head>
<title>18.5 Confidence Intervals when you don't know the population standard deviation</title>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

# Lesson 18.5 Confidence Interval when you don't know $$\sigma$$
## Reading
* 7.1.2 Introducing the t-distribution (pages 278-281 of the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf))
* 7.1.3 The t-distribution and the standard error of a mean (page 281 of the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf))
* 7.1.5 One sample t-intervals (pages 282-285 of the [Introductory Statistics Textbook](OpenIntroTextbook.pdf))

## Lesson
Consider this problem:
> A health researcher wants to estimate the average number of hours of sleep that college students get on weeknights. A random sample of 25 students is taken, and the sample yields a mean of 6.8 hours with a sample standard deviation of 1.2 hours.
> 
> Construct a 95% confidence interval for the true mean number of hours of sleep college students get on weeknights.

Notice that in this case, we do not have a population standard deviation ($$\sigma$$). So, our Margin of Error calculation won't work.

Fortunately, we have a solution. The normal distribution depends on the population. Another distribution that we call the __t-distribution__ depends instead on the sample. This is a good approximation of the normal distribution.

With the t-distribution, we find a critical value from t-scores and use the sample standard deviation to find the margin of error.

$$E = t_c\frac{s}{\sqrt{n}}$$

However, since the t-distribution relies on the sample, we also have to consider one more variable:
* The __Degrees of Freedom__ is calculated as $$DF = n-1$$
* As $$n$$ increases, the t-distribution becomes a better approximation of the normal distribution.

<img src="images/Fig18_5a_tDistributions.png?raw=true" width="500" alt="T-Distributions with varying degrees of freedom">

To find the critical t-score, use a [T-Table](../Resources/T-Table.pdf) or a calculator (Note that the TI-83 will not work for this step, so be familiar with the table). In the problem above, 
* The Sample Size is $$n=25$$
* There are $$DF = n-1 = 24$$ degrees of freedom
* The confidence level is 95%

Using these on the T-Table, we get a critical t-score of $$t_c = 2.064$$

<img src="images/Fig18_5b_tTable.png?raw=true" width="500" alt="T-Distributions with varying degrees of freedom">

Other than that, the calculations for the Margin of Error and the Confidence Interval are exactly the same.
$$E = t_c\frac{s}{\sqrt{n}} \qquad \mu = \bar{x} \pm SE$$

#### Example
Here is the problem from earlier:
> A health researcher wants to estimate the average number of hours of sleep that college students get on weeknights. A random sample of 25 students is taken from a normally-distributed population, and the sample yields a mean of 6.8 hours with a sample standard deviation of 1.2 hours.
> 
> Construct a 95% confidence interval for the true mean number of hours of sleep college students get on weeknights.

Here is the information given from the problem.
* Confidence Level is 95%
* Sample Size is $$n = 25$$
* Degrees of Freedom is $$DF = n-1 = 24$$
* Sample mean is $$\bar{x} = 6.8$$
* Sample standard deviation is $$s = 1.2$$

__Before we do anything, we must verify that the Central Limit Theorem holds.__
* Is the sample random? __Yes__ (stated in the problem)
* Is the sample large enough? __No__ (sample size is smaller than 30)
  * If it's not large enough, is the population normally distributed? __Yes__ (stated in the problem)

So, the Central Limit Theorem holds.

Using the T-Table or the TI-84, we get a critical value of $$t_c = 2.064$$.

$$SE = t_c\frac{s}{\sqrt{n}} = 2.064\frac{1.2}{\sqrt{25}} = 0.495$$

$$\bar{x} + E = 6.8 + 0.495 = 7.295 \approx \mathbf{7.3}$$

$$\bar{x} - E = 6.8 - 0.495 = 6.305 \approx \mathbf{6.3}$$

Solution: __We are 95% confident that the true mean for the number of hours of sleep college students get on weeknights is between 6.3 and 7.3 hours__.

## Practice
1. A nutritionist wants to estimate the average number of cups of coffee consumed per week by graduate students. A random sample of 16 students shows a mean of 9.3 cups with a sample standard deviation of 2.1 cups. Construct a 90% confidence interval for the true mean weekly coffee consumption of graduate students.
    * [After solving on your own, see solution here](Solutions/18_5_Solution1.md)

2. A tech company tests a new phone battery. A sample of 30 phones, coming from a normally-distributed population, shows an average battery life of 22.4 hours with a sample standard deviation of 3.5 hours. Construct a 99% confidence interval for the true mean battery life of the new phone model.
    * [After solving on your own, see solution here](Solutions/18_5_Solution2.md)

3. A professor surveys 41 students about how many hours they studied for the last exam. The sample mean is 14.2 hours, and the sample standard deviation is 4.6 hours. Construct a 95% confidence interval for the true mean number of hours students studied for the exam.
    * [After solving on your own, see solution here](Solutions/18_5_Solution3.md)

## Technology
### TI-84
Note that this method will not work on the TI-83. Use the [T-Table](../Resources/T-Table.pdf) instead.

To find the t-score: