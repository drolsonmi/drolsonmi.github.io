<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

# Lesson 18.2 Margin of Error
## Reading
* 7.1.1 Using the z-distribution for inference when $$\mu$$ is unknown and $$\sigma$$ is known (pages 277 of the [Introduction to Statistics Textbook](../Resources/OpenIntroTextbook.pdf))

## Lesson
In lesson 18.1, we found the critical values of a specified critical level.

<img src="https://github.com/drolsonmi/SnowCollegeClasses/blob/main/math1040online/images/Fig18_1a_90ConfInt.png?raw=true" width="350" alt="90% Confidence Level">

We take these critical values and convert them back to our regular scale to find the boundaries of our confidence interval.

Recall that the equation for finding a z-score is,

$$z = \frac{x-\mu}{\sigma}$$

We need to make two changes. Since we are applying the Central Limit Theorem, we are going to use our mean and standard deviation from our sampling distribution:

$$z = \frac{\bar{x} - \mu_{\bar{x}}}{\sigma_{\bar{x}}} = \frac{\bar{x}-\mu}{\tfrac{\sigma}{\sqrt{n}}}$$

Since we are after the population mean, we solve for $$\mu$$.

$$\pm z\frac{\sigma}{\sqrt{n}} = \bar{x}-\mu$$

$$-\bar{x} \pm z\frac{\sigma}{\sqrt{n}} = -\mu$$

$$\mu = \bar{x} \pm z\frac{\sigma}{\sqrt{n}}$$

This is our confidence interval! The population mean (the true value) is most likely between $$\bar{x} - z(\sigma / \sqrt{n})$$ and $$\bar{x} + z(\sigma / \sqrt{n})$$. In the next page, we'll see a full example of this calculation along with how to interpret it.

The last term of this formula is known as the __margin of error__ ($$E$$), or more commonly as the __standard error__ ($$SE$$).

$$SE = z\frac{\sigma}{\sqrt{n}}$$


## Practice
1. The average height of a particular species of flower is 5.5 inches with a standard deviation of 0.4 inches. You sample a subspecies and find 49 flowers with a sample mean height of 5.8 inches. What is the margin of error with a 95% confidence level?
    * [After solving on your own, see solution here](./Solutions/18_2_Solution1.md)
2. The average length of a particular set of books written by authors around the world is 425 pages with a standard devation of 32 pages. Looking at authors specifically from South Africa, a sample of 36 of these books has an average length of 410 pages. What is the margin of error with a 90% confidence level?
    * [After solving on your own, see solution here](https://github.com/drolsonmi/SnowCollegeClasses/blob/main/math1040online/Lectures/Solutions/18_2_Solution2.md)
3. Bottles of soda are to be filled with 2.00 liters, allowing some room for error giving a standard deviation of 0.15 liters. Calculate the margin of error for a sample of 54 of these bottles with an average volume of 1.95 liters at a 99% confidence level.
    * [After solving on your own, see solution here](https://github.com/drolsonmi/SnowCollegeClasses/blob/main/math1040online/Lectures/Solutions/18_2_Solution3.md)