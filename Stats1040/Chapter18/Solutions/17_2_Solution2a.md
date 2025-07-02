#### Answer to Practice Problem 2
A factory produces light bulbs with a mean lifetime of 1,200 hours and a standard deviation of 100 hours. A quality control engineer selects a random sample of 36 bulbs.

1. What is the probability that the lifetime of a single bulb is greater than 1,225 hours?
    * The probability is found by finding the area of the right tail of a standardized normal distribution using a Z-Table or a calculator
        * On a Z-Table,
            * The z-score is $z = \frac{1225 - 1200}{100} = \frac{25}{100} = 0.25
            * Look at the area left of z = 0.25
                * $P(z < 0.25) = 0.599$
            * Take the compliment to get the area to the right of z = 0.25
                * $P(z > 0.25) = 1 - P(z < 0.25) = 1 - 0.599 = 0.401$
        * On a TI-83/84, DISTR --> 2:normalcdf(
            * 2:normalcdf(1225,9999,1200,100) if using the values from the problem
            * 2:normalcdf(0.25,9999,0,1) if using the z-score (gives the same answer)
    * __Probability = 0.401 = 40.1\%__

[Click here](https://github.com/drolsonmi/SnowCollegeClasses/blob/main/math1040online/Lectures/17_2_StatsOfSamplingDists.md#practice) to return to the lecture notes.