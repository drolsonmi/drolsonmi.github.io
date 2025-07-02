#### Answer to Practice Problem 2
A factory produces light bulbs with a mean lifetime of 1,200 hours and a standard deviation of 100 hours. A quality control engineer selects a random sample of 36 bulbs.

2. What is the probability that the sample mean lifetime of the 36 bulbs is greater than 1,225 hours?
    * The mean and standard deviation are:
        * $\mu_{\bar{x}}$ = $\mu$ = 1200
        * $\sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}} = \frac{100}{\sqrt{36}} = \frac{100}{6} = 16.667$
    * The probability is found by finding the area of the right tail of the sampling distribution using a Z-Table or a calculator
        * On a Z-Table,
            * The z-score is $z = \frac{1225 - 1200}{16.667} = \frac{25}{16.667} = 1.5$
            * Look at the area left of z = 1.5
                * $P(z < 1.5) = 0.933$
            * Take the compliment to get the area to the right of z = 0.25
                * $P(z > 1.5) = 1 - P(z < 1.5) = 1 - 0.933 = 0.067$
        * On a TI-83/84, DISTR --> 2:normalcdf(
            * 2:normalcdf(1225,99999,1200,16.667) if using the values from the problem
            * 2:normalcdf(1.5,9999,0,1) if using the z-score (gives the same answer)
    * __Probability = 0.067 = 6.7\%__

[Click here](https://github.com/drolsonmi/SnowCollegeClasses/blob/main/math1040online/Lectures/17_2_StatsOfSamplingDists.md#practice) to return to the lecture notes.