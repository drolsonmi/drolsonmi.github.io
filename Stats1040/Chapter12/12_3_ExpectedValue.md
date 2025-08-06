<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

# Lesson 12.3 Expected Value
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 

## Lesson
With quantitative data, you can find the center by using the mean, the median, and the mode. But how do you calculate the center of categorical data? What is the middle of the categorical set {Exhausted, Tired, Normal, Energized}, taking into account the probabilities of each category?

To calculate the center, we use the __expected value__.

Finding the expected value can only be done if there is an order to the categories. In other words, we are working with an *ordinal* variable.

Calculating the expected value can be done in 4 steps:

1. List the categories in order and assign a value to show that order - we'll call this 
2. Find the probability distribution by calculating the relative frequency (probability) of each category: 
3. Multiply the value $$x$$ by its probability $$P(x)$$
4. Add up all the results

Here's the full equation:

$$\sum x\cdot P(x)$$

This can be applied in cases where you have values for each category. If there are no values, we can assign values. Let me give you two examples, one for each scenario.

### Example 1 - Values provided
First, we have an example where values are already given to each category. 

I am involved in a program where I pay $1000 for a class. If I successfully pass the class, I get half of the payment back. If I fail the class, I lose the entire amount.

Putting those into concrete numbers:

* If I pass the class, I pay $1000 - $500 = $500
* If I fail the class, I pay $1000

If 80% of the students pass the class, what is the average amount paid per student?

Start by creating a table:

| Category               | Pass  | Fail  |
| :--------------------- | :---: | :---: |
| Value ($$x$$)          | $500  | $1000 |
| Probability ($$P(x)$$) | 0.80  | 0.20  |

To find the expected value, multiply the values by their probabilities, then add up those results.

| Category               | Pass  | Fail  |
| :--------------------- | :---: | :---: |
| Value ($$x$$)          | $500  | $1000 |
| Probability ($$P(x)$$) | 0.80  | 0.20  |
| $$x\cdot P(x)$$        | $500*0.80 = $400 | $1000*0.20 = $200 |

$$E[x] = $400 + $200 = $600$$

So, the expected value, or the average amount paid per student, is $600.

Does this make sense? Most of the students pass, so they only pay $500. But some do fail, so that will raise the average a little bit, so $600 does make sense.

### Example 2 - No values provided
Now, we'll address a scenario where we don't have values for the categories.

After exercising, I track if I feel tired or energetic. I get the following data:

* Exhausted: 12 times
* Tired:  19 times
* Normal: 16 times
*  Energized: 9 times

These categories have an order, from exhausted on one extreme and energized on the other. So, I'm going to assign 0 to the lowest extreme (exhausted) and 3 to the highest (energized). Now, I have a numerical way of representing each category.

| Category  | Exhausted | Tired | Normal | Energized |
| :-------- | :-------: | :---: | :----: | :-------: |
| Value (x) | 0         | 1     | 2      | 3         |

Now, I add the relative frequencies of each category, and multiply the $$x$$ values by $$P(x)$$:

| Category               | Exhausted     | Tired           | Normal          | Energized       |
| :--------------------- | :-----------: | :-------------: | :-------------: | :-------------: |
| Value ($$x$$)          | 0             | 1               | 2               | 3               |
| Probability ($$P(x)$$) | 12/56 = 0.214 | 19/56 = 0.339   | 16/56 = 0.286   | 9/56 = 0.161    |
| $$x\cdot P(x)$$        | 0*0.214 = 0   | 1*0.339 = 0.339 | 2*0.286 = 0.572 | 3*0.161 = 0.483 |

Adding up those results gives me my expected value.

$$\begin{align*}
E[x] &= 0*0.214 + 1*0.339 + 2*0.286 + 3*0.161 \\
     &= 0 + 0.339 + 0.572 + 0.483 \\
     &= \mathbf{1.394}
\end{align*}$$

Now, what does this number mean? On average, my energy level is at 1.394. That is part way between 1 and 2. But remember that 1 means "Tired" and 2 means "Normal". So, on average, I am somewhere between Tired and Normal, a little closer to Tired.

And there you have it! We have found the average of a categorical variable.

## Practice
1. ?
    * After solving on your own, check the <button popovertarget="Problem_1">Solution</button>
2. ?
    * After solving on your own, check the <button popovertarget="Problem_2">Solution</button>
3. ?
    * After solving on your own, check the <button popovertarget="Problem_3">Solution</button>

<div popover id="Problem_1">

## Problem 20.1.1
A popover is an element that is placed on top of everything else.
* Item 1
* Item 2

$$\bar{x}=\frac{1}{n}\sum x$$
It can be used when you want to tell something important.

<center><button popovertarget="Problem_1" popovertargetaction="hide">Close</button></center>
</div>

<div popover id="Problem_2">

## Problem 20.1.2
A popover is an element that is placed on top of everything else.
* Item 1
* Item 2

$$\bar{x}=\frac{1}{n}\sum x$$
It can be used when you want to tell something important.

<center><button popovertarget="Problem_2" popovertargetaction="hide">Close</button></center>
</div>
<div popover id="Problem_3">

## Problem 20.1.3
A popover is an element that is placed on top of everything else.
* Item 1
* Item 2

$$\bar{x}=\frac{1}{n}\sum x$$
It can be used when you want to tell something important.

<center><button popovertarget="Problem_3" popovertargetaction="hide">Close</button></center>
</div>


## Technology

### TI-83/84

### Excel

### Desmos