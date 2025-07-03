## Practice
2. A manufacturer claims that its LED light bulbs have an average lifespan of 1,200 hours. A consumer protection agency wants to verify this claim. They randomly select 40 bulbs and find that the sample has an average lifespan of 1,165 hours. The population standard deviation is known to be 100 hours. Construct a 99% confidence interval for the true mean lifespan of the manufacturer’s LED light bulbs.

## Solution
From the problem we get the following information:
* Sample is random
* Sample size is $$n=40$$
* Sample mean is $$\bar{x}=1,165$$
* Population standard deviation is $$\sigma=100$$

#### 1. Central Limit Theorem
1. Is the sample random? __Yes__ (stated in the problem)
2. Is the sample large enough? __Yes__ ($$n = 40 \ge 30$$)

#### 2. Critical Value
With a 99% confidence interval, the remaining 1% is divided between the two tails (0.5% each)
* The z-score dividing the center from the two tails is $$\pm$$2.58

#### 3. Margin of Error
$$E = z_c\frac{\sigma}{\sqrt{n}} = 2.58\frac{100}{\sqrt{40}} = 40.79$$

#### 4. Confidence Interval
$$\bar{x} + E = 1165 + 40.79 = 1205.79$$

$$\bar{x} - E = 1165 - 40.79 = 1124.21$$

__The confidence interval is (1,124.21 , 1,205.79)__.

#### 5. Interpretation of the Confidence Interval
__We are 99% confident that the true average life of LED light bulbs is between 1,124.21 hours and 1,205.79 hours.__

[Return back to Lesson 18.3](../18_3_ConfidenceInterval.md#practice)