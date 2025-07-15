<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

# Lesson 20.2 How Confidence Intervals fit in
## Reading

## Lesson
Recall how the __confidence interval__ is used to find the range of true values. We showed this with this example:

> American mental abilities are often measured by an IQ test.  The IQ distribution is normal with a mean of 100 and a population standard deviation of 15. A random sample of 40 Snow College students is taken and they have an average IQ of 106.3. Can we say with a 5% level of significance that the true average IQ of Snow College students is higher than the nation?

We found, with 90% confidence, that the true average IQ of Snow College students is between 102.4 and 110.2. This confidence interval is shown in the image below.

Now, let's look again at this as a hypothesis test. We want to see if the true average IQ of Snow College students is larger than the national average. The nation has an average of 100, so that is our null value.

$$H_0: \mu = 100 \qquad\qquad H_A: \mu > 100$$

In this image, we can see the confidence interval along with the null value

<img src="images/Fig20_1a_90ConfInt.png?raw=true" width="500" alt="90% Confidence Level">

If the true value is most likely between 102.4 and 110.2, then there is not much chance that the true value can be equal to the null value (100). Because the confidence interval is completely above the null value, we can be pretty confident that the average IQ of Snow College students is higher than the national average.

So, in this case, we can __reject the null hypothesis__ as we have enough evidence to suggest the true average is higher than the null value. Instead, we __adopt the alternate hypothesis__ which claims Snow College students have a higher IQ.

Consider another school:

> A random sample of 50 students from Medford College shows an average IQ of 98.3. Can we say with a 5% level of significance that the true average IQ of Snow College students is higher than the nation?

Doing a 90% confidence interval in this situation, we show that the true average is between 94.8 and 101.8.

<img src="images/Fig20_1b_90ConfInt.png?raw=true" width="500" alt="90% Confidence Level">

In this case, the null value of 100 is inside of the confidence interval. That means that there is a chance that the true IQ of students at Medford College is at or near 100. So, we __fail to reject the null hypothesis__ since we don't have enough evidence to reject it.

When doing hypothesis testing, we don't actually look at confidence intervals. However, the method of hypothesis testing is actually closely related to confidence intervals. So, when I go through the hypothesis testing process in the next pages, I will include the confidence interval so that you can see that this works.

## Practice
For each of the following questions, find the confidence interval and compare it to the null value. (Note that I give you the confidence level. We'll discuss the significance level in the next page.)
1. A coffee shop claims that the average wait time for a customer to receive their order is no more than 4 minutes. A customer advocacy group believes the wait time is longer. A random sample of 35 customers had an average wait time of 4.6 minutes with a standard deviation of 1.2 minutes. At the 5% significance level (90% confidence level), test the claim that the average wait time is greater than 4 minutes.
    * After solving on your own, check the <button popovertarget="Problem_1">Solution</button><br><br>
2. A smartphone manufacturer advertises that their new model has an average battery life of 20 hours. A tech reviewer suspects the battery life is less than advertised. A sample of 55 phones showed an average battery life of 18.7 hours with a standard deviation of 2.5 hours. Conduct a hypothesis test at the 1% significance level (98% confidence level).
    * After solving on your own, check the <button popovertarget="Problem_2">Solution</button><br><br>
3. An educator wants to test whether a new teaching method affects student performance. Historically, the average score on a standardized exam is 75. The educator believes the new method may lead to a different average score. A class of 40 students taught with the new method had an average score of 78.2 with a standard deviation of 6.3. Test the hypothesis at the 5% significance level (95% confidence level).
    * After solving on your own, check the <button popovertarget="Problem_3">Solution</button>

<div popover id="Problem_1">

## Problem 20.2.1
1. A coffee shop claims that the average wait time for a customer to receive their order is no more than __4 minutes__. A customer advocacy group believes the wait time is longer. A __random sample__ of __35 customers__ had an __average wait time of 4.6 minutes__ with a __standard deviation of 1.2 minutes__. At the 5% significance level (90% confidence level), test the claim that the average wait time is greater than 4 minutes.

We are going to do the following:
1. Verify that the CLT is satisfied
2. Define our Hypotheses
3. Determine the correct interval to use
4. Calculate the interval
5. Compare to the null value

The Central Limit Theorem is satisfied
* The sample is random
* The sample is large enough ($$n = 35 > 30$$)

From 20.1, we determined the hypotheses:

$$H_0: \mu = 4 \qquad\qquad $$H_A: \mu > 4$$

Since we don't have a population standard deviation ($$\sigma$$), we will use a t-score with the `TInterval` function on the calculator.

<img src="images/Fig20_1c_TI84.png?raw=true" width="500" alt="Setting for TInterval function"> <img src="images/Fig20_1d_results.png?raw=true" width="500" alt="Results for confidence interval">

With 90% confidence, we see the true average wait time for customers is between 4.257 and 4.943 minutes. The null value ($$\mu_0 = 4$$) is *not* inside the confidence interval. So, we can __reject the null hypothesis__.

Therefore, there is enough evidence to suggest that the average wait time for customers to receive their orders is more than 4 minutes.

<center><button popovertarget="Problem_1" popovertargetaction="hide">Close</button></center>
</div>

<div popover id="Problem_2">

## Problem 20.2.2
2. A smartphone manufacturer advertises that their new model has an average battery life of __20 hours__. A tech reviewer suspects the battery life is less than advertised. A __random sample__ of __55 phones__ showed an __average battery life of 18.7 hours__ with a __standard deviation of 2.5 hours__. Conduct a hypothesis test at the 1% significance level (98% confidence level).

We are going to do the following:
1. Verify that the CLT is satisfied
2. Define our Hypotheses
3. Determine the correct interval to use
4. Calculate the interval
5. Compare to the null value

The Central Limit Theorem is satisfied
* The sample is random
* The sample is large enough ($$n = 55 > 30$$)

From 20.1, we determined the hypotheses:

$$H_0: \mu = 20 \qquad\qquad $$H_A: \mu < 20$$

Since we don't have a population standard deviation ($$\sigma$$), we will use a t-score with the `TInterval` function on the calculator.

<img src="images/Fig20_1e_TI84.png?raw=true" width="500" alt="Setting for TInterval function"> <img src="images/Fig20_1f_results.png?raw=true" width="500" alt="Results for confidence interval">

With 98% confidence, we see the true average wait time for customers is between 17.892 and 19.508 minutes. The null value ($$\mu_0 = 20$$) is *not* inside the confidence interval. So, we can __reject the null hypothesis__.

Therefore, there is enough evidence to suggest that the average battery life is less than 20 hours.

<center><button popovertarget="Problem_2" popovertargetaction="hide">Close</button></center>
</div>
<div popover id="Problem_3">

## Problem 20.2.3
3. An educator wants to test whether a new teaching method affects student performance. Historically, __the average score on a standardized exam is 75__. The educator believes the new method may lead to a different average score. A class of __40 students__ taught with the new method had an __average score of 78.2__ with a __standard deviation of 6.3__. Test the hypothesis at the 5% significance level (95% confidence level).

We are going to do the following:
1. Verify that the CLT is satisfied
2. Define our Hypotheses
3. Determine the correct interval to use
4. Calculate the interval
5. Compare to the null value

The Central Limit Theorem is NOT satisfied
* <font color='red'>The sample is *not* random</font>
* The sample is large enough ($$n = 35 > 30$$)

Technically, we should stop here. However, just for practice, we'll go ahead and solve it even though the CLT is not satisfied.

From 20.1, we determined the hypotheses:

$$H_0: \mu = 75 \qquad\qquad $$H_A: \mu > 75$$

Since we don't have a population standard deviation ($$\sigma$$), we will use a t-score with the `TInterval` function on the calculator.

<img src="images/Fig20_1g_TI84.png?raw=true" width="500" alt="Setting for TInterval function"> <img src="images/Fig20_1h_results.png?raw=true" width="500" alt="Results for confidence interval">

With 98% confidence, we see the true average score is between 76.185 and 80.215 minutes. The null value ($$\mu_0 = 75$$) is *not* inside the confidence interval. So, we can __reject the null hypothesis__.

Therefore, there is enough evidence to suggest that the average score with the new teaching method is different from the average score with the old teaching method.

<center><button popovertarget="Problem_3" popovertargetaction="hide">Close</button></center>
</div>