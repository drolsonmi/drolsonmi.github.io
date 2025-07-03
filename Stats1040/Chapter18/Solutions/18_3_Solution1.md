## Practice
1. A university is interested in estimating the average daily commute time for its students. A random sample of 50 students is selected, and their average commute time is found to be 32 minutes. The population standard deviation is known to be 8 minutes. Construct a 95% confidence interval for the true mean commute time of all students at the university.

## Solution
From the problem we get the following information:
* Sample is random
* Sample size is $$n=50$$
* Sample mean is $$\bar{x}=32$$
* Population standard deviation is $$\sigma=8$$

#### 1. Central Limit Theorem
1. Is the sample random? __Yes__ (stated in the problem)
2. Is the sample large enough? __Yes__ ($$n = 50 \ge 30$$)

#### 2. Critical Value
With a 95% confidence interval, the remaining 5% is divided between the two tails (2.5% each)
* The z-score dividing the center from the two tails is $$\pm$$1.96

#### 3. Margin of Error
$$E = z_c\frac{\sigma}{\sqrt{n}} = 1.96\frac{8}{\sqrt{50}} = 2.22$$

#### 4. Confidence Interval
$$\bar{x} + E = 32 + 2.22 = 34.22$$

$$\bar{x} - E = 32 - 2.22 = 29.78$$

__The confidence interval is (29.78, 34.22)__.

#### 5. Interpretation of the Confidence Interval
__We are 95% confident that the true average daily commute is between 29.78 minutes and 34.22 minutes.__

[Return back to Lesson 18.3](../18_3_ConfidenceInterval.md#practice)