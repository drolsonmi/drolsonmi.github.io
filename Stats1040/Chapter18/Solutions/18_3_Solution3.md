## Practice
3. A national education researcher wants to estimate the average SAT Math score for high school seniors in a particular state. A random sample of 60 students yields a sample mean score of 540. The population standard deviation is known to be 100 points. Construct a 92% confidence interval for the true mean SAT Math score of all high school seniors in the state.

## Solution
From the problem we get the following information:
* Sample is random
* Sample size is $$n=60$$
* Sample mean is $$\bar{x}=540$$
* Population standard deviation is $$\sigma=100$$

#### 1. Central Limit Theorem
1. Is the sample random? __Yes__ (stated in the problem)
2. Is the sample large enough? __Yes__ ($$n = 50 \ge 30$$)

#### 2. Critical Value
With a 92% confidence interval, the remaining 8% is divided between the two tails (4% each)
* Using a Z-Table or a calculator, we find that the z-score dividing the center from the two tails is $$\pm$$1.75

#### 3. Margin of Error
$$SE = z_c\frac{\sigma}{\sqrt{n}} = 1.75\frac{100}{\sqrt{60}} = 22.59$$

#### 4. Confidence Interval
$$\bar{x} + SE = 540 + 22.59 = 562.59$$

$$\bar{x} - SE = 540 - 22.59 = 517.41$$

__The confidence interval is (517.41, 562.59)__.

#### 5. Interpretation of the Confidence Interval
__We are 92% confident that the average daily commute is between 517.41 minutes and 562.59 minutes.__

[Return back to Lesson 18.3](../18_3_ConfidenceInterval.md#practice)