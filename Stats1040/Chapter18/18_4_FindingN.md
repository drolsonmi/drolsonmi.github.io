
# Lesson 18.4 Finding the best sample size
## Reading
* 7.1.6 Choosing a sample size when estimating a mean (pages 285-286 of the [Introductory Statistics Textbook](OpenIntroTextbook.pdf))

## Lesson
How do you know what the sample size $$n$$ should be? This is actually not hard. Take the Margin of Error and solve for $$n$$:

$$SE = z_c \frac{\sigma}{\sqrt{n}} \qquad \to \qquad n = \left(\frac{z_c \sigma}{SE}\right)^2$$

So what we need is a critical value (a confidence level), a population standard deviation, and a desired Margin of Error. Then just plug them into the equation to get the desired sample size.

Recall the example problem from 18.3. We'll modify the question a bit to show what we mean.

> American mental abilities are often measured by an IQ test.  The IQ distribution is normal with a mean of 100 and a population standard deviation of 15.  
> 
> What sample size is needed if you want the margin of error to be 1.5 with a 90% confidence level?

* Confidence level is 90%, so $$z_c = 1.645$$
* The population standard deviation is $$\sigma = 15$$
* The desired Margin of Error is $$SE = 1.5$$

$$n = \left(\frac{z_c\sigma}{SE}\right)^2 = \left(\frac{1.645\cdot 15}{1.5}\right)^2 = \left(\frac{24.675}{1.5}\right)^2 = 16.45^2 = 270.60$$

The answer is that you need to sample 270.6 people to get a margin of error of 1.5. However, you can't sample 0.6 people, so we need to *round the answer up*.
* If you round down, the margin of error goes up, which we don't want
* So, we always round *up*

Thus, the sample size needs to be at least 271 people in order to get a margin of error at or below 1.5.

## Practice
1. A university is interested in estimating the average daily commute time for its students. The population standard deviation is known to be 8 minutes. What sample size is needed to get a margin of error less than 3.0 for a 95% confidence interval?
    * [After solving on your own, see solution here](Solutions/18_4_Solution1.md)

2. A manufacturer claims that its LED light bulbs have an average lifespan of 1,200 hours. A consumer protection agency wants to verify this claim. The population standard deviation is known to be 100 hours. What sample size is needed to get a margin of error less than 35 for a 99% confidence interval?
    * [After solving on your own, see solution here](Solutions/18_4_Solution2.md)

3. A national education researcher wants to estimate the average SAT Math score for high school seniors in a particular state. The population standard deviation is known to be 100 points. What sample size is needed to get a margin of error less than 25 for a 92% confidence interval?
    * [After solving on your own, see solution here](Solutions/18_4_Solution3.md)