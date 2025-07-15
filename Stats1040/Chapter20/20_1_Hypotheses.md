<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

# Lesson 20.1 Hypotheses
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 5.3.1 Introducing Hypotheis Testing (page 195)
* 5.3.2 Setting up the null and alternate hypotheses (pages 196-198)

## Lesson
Imagine you are in a courtroom as a member of the jury. The defendant comes in. As a member of the jury,
* Your default assumption is that the defendant is `innocent`
* You then gether evidence through witnesses
* From the evidence, we decide whether there is enough evidence to change the `innocent` verdict to `guilty`
  * If there is enough evidence, then we reject the innocent assumption and declare the defendant `guilty`
  * If there is not enough evidence, then we cannot reject the `innocent` assumption, so it remains.

This is actually a good picture of what we are doing with __hypothesis testing__. We have some pre-detemined value which we call the __null value__. 
* For quantitative data, the null value will be a mean ($$\mu_0$$)
* For categorical data, the null value will be a proportion ($$p_0$$)

We then gather data and use statistics to determine if the null value fits with the data or not.

#### The Null Hypothesis
Our default assumption in statistics is that the true value (the population mean for quantitative data) has not changed. It is the same as the null value. This is known as a __Null Hypothesis__.

$$H_0: \mu = \mu_0\text{ for Quantitative variables} \qquad\qquad H_0: p = p_0\text{ for Categorical variables}$$

For problems within this course, the null value will often be given to you. In the real world, this may take some research. It may be published in a research paper, it may be a calculation from last year, or it may be something you need to find on your own. For this class, we'll make it easy for you and give it to you.

Consider this problem we saw back in Lesson 18 (I'll adapt the question to fit what we are looking for in hypothesis testing):

> American mental abilities are often measured by an IQ test.  The IQ distribution is normal with a mean of 100 and a population standard deviation of 15. A random sample of 40 Snow College students is taken and they have an average IQ of 106.3. Can we say with a 5% level of significance that the true average IQ of Snow College students is higher than the nation?

(For now, don't worry about the 5% level of significance. We'll address that in the next section).

In this case, we have a sample that represents all Snow College students ($$\bar{x} = 106.3$$). We don't know what the population mean is ($$\mu$$). We can find a Confidence Interval to find this. But the question is how this population mean compares to the mean for the entire United States. Since we want to compare Snow College IQ scores to the national scores, the national average is our null value.

$$\mu_0 = 100$$

So, our __Null Hypothesis__, or our default assumption, is that the average IQ of Snow College students is the same as for the nation. Specifically, we assume that the average IQ of Snow College students is 100.

$$H_0: \mu = 100$$

#### The Alternate Hypothesis
What if the null hypothesis isn't true? We need to establish a second hypothesis, known as an __Alternate Hypothesis__, which will be our assumption if the null hypothesis fails. The alternate hypothesis is based on what we want to show in our question. There are 3 different possible alternate hypothesis:
* The true value is greater than the null value

$$H_A: \mu > \mu_0$$

* The true value is less than the null value

$$H_A: \mu < \mu_0$$

* The true value is different from the null value

$$H_A: \mu \ne \mu_0$$

In the IQ question, we want to see whether the IQ of Snow College students is *"higher than"* the national average. So, we take the first option for our alternate hypothesis.

$$H_0: \mu = 100 \qquad\qquad H_A: \mu > 100$$

The rest of the lesson will look at how to determine which hypothesis we accept.

## Practice
For each of the following questions, establish both the Null Hypothesis and the Alternate Hypothesis
1. A coffee shop claims that the average wait time for a customer to receive their order is no more than 4 minutes. A customer advocacy group believes the wait time is longer. A random sample of 35 customers had an average wait time of 4.6 minutes with a standard deviation of 1.2 minutes. At the 5% significance level, test the claim that the average wait time is greater than 4 minutes.
    * After solving on your own, check the <button popovertarget="Problem_1">Solution</button><br><br>
2. A smartphone manufacturer advertises that their new model has an average battery life of 20 hours. A tech reviewer suspects the battery life is less than advertised. A sample of 55 phones showed an average battery life of 18.7 hours with a standard deviation of 2.5 hours. Conduct a hypothesis test at the 1% significance level.
    * After solving on your own, check the <button popovertarget="Problem_2">Solution</button><br><br>
3. An educator wants to test whether a new teaching method affects student performance. Historically, the average score on a standardized exam is 75. The educator believes the new method may lead to a different average score. A class of 40 students taught with the new method had an average score of 78.2 with a standard deviation of 6.3. Test the hypothesis at the 5% significance level.
    * After solving on your own, check the <button popovertarget="Problem_3">Solution</button>

<div popover id="Problem_1">

<h1>Problem 20.1.1</h1>
<p>1. A coffee shop claims that the average wait time for a customer to receive their order is no more than <b>4 minutes</b>. A customer advocacy group believes <b>the wait time is longer</b>. A random sample of 35 customers had an average wait time of 4.6 minutes with a standard deviation of 1.2 minutes. At the 5% significance level, test the claim that the average wait time is greater than 4 minutes.</p>

<p>Our study is comparing the average wait time to <b>4 minutes</b>. This is our null value.</p>

$$\mu_0 = 4$$

<p>The default assumption is that the true mean is 4 minutes. We are testing to see if the wait time at the coffee shop is <b>longer</b> than 4 minutes. So, our hypotheses are:</p>

$$H_0: \mu = 4 \qquad \qquad H_A: \mu > 4$$

<center><button popovertarget="Problem_1" popovertargetaction="hide">Close</button></center>
</div>

<div popover id="Problem_2">

<h1>Problem 20.1.2</h1>
<p>2. A smartphone manufacturer advertises that their new model has an average battery life of <b>20 hours</b>. A tech reviewer suspects the battery life is <b>less than advertised</b>. A sample of 55 phones showed an average battery life of 18.7 hours with a standard deviation of 2.5 hours. Conduct a hypothesis test at the 1% significance level.</p>

<p>The advertisement says the average is 20 hours, and we are comparing our phone batteries to this number, so this is our null value.</p>

$$\mu_0 = 20$$

<p>The default assumption is that this is correct. The test is to see if the time is <b>less</b> than advertised. So, our hypotheses are:</p>

$$H_0: \mu = 20 \qquad\qquad H_A: \mu < 20$$

<center><button popovertarget="Problem_2" popovertargetaction="hide">Close</button></center>
</div>
<div popover id="Problem_3">

<h1>Problem 20.1.3</h1>
<p>3. An educator wants to test whether a new teaching method affects student performance. <b>Historically, the average score on a standardized exam is 75</b>. The educator believes the <b>new method may lead to a different average score</b>. A class of 40 students taught with the new method had an average score of 78.2 with a standard deviation of 6.3. Test the hypothesis at the 5% significance level.</p>

<p>The standardized exam shows an average score of 75 using the previous teaching method. This is what we are comparing the new teaching method to, so we use 75 as our null value.</p>

$$\mu_0 = 75$$

<p>We want to see if the new teaching method leads to <b>different</b> average scores. In this case, we don't care if the score is greater or smaller - just different. So, our hypotheses are:</p>

$$H_0: \mu = 75 \qquad\qquad H_A: \mu \ne 75$$

<center><button popovertarget="Problem_3" popovertargetaction="hide">Close</button></center>
</div>