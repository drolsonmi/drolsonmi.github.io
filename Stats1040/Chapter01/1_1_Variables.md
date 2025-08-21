<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

# Lesson 1.1 Variables
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 1.2.1 Observations, variables, and data matrices (pages 11-12)
* 1.2.2 Types of Variables (pages 12-13)
* 1.2.3 Relationships between variables (pages 13-15)

## Lesson
We begin by looking at populations.
* A __population__ is everyone/everything pertaining to a study
    * A study about favorite flavors of ice cream among college students would have a population of *all college students*
    * A study about the quality of a brand of chocolate bar would have a population of *all chocolate bars of that brand*
* A measurement taken from a population is known as a __parameter__

Populations can be difficult to measure as *every* person or item in the population *must* be included. This is frequently impossible to do. So, we instead take a sample.
* A __sample__ is a subset of the population that represents the population
    * To study the favorite flavors of ice cream among college students, we may ask about 100 students from each college
    * To study the quality of a brand of chocolate bar, we might take 5 bars from each batch of chocolate bars made

Samples are much easier to measure. We then take the results of our sample to __infer__ information about the population. The topic of __inference__ will be discussed after the midterm this semester.

<iframe width="560" height="315" src="https://www.youtube.com/embed/qUTsxREdZfU?si=Ftwb6n4k647Ekh9Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/0SI23BfhVHM?si=0pPAjn9Le3sBLtpe" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

All variables can be identified as one of two types:
* __Quantitative__ (or numerical) variables deal with numbers. We can do mathematical calculations on these.
* __Categorical__ (or qualitative) variables deal with groups. Doing math on these variables will not make sense. Instead, we count the occurrences in each category and deal with percentages and probabilities.

<table style="margin: 1.2em 0px; padding: 0px; border-collapse: collapse; border-spacing: 0px; font: inherit; border: 0px;">
                <thead>
                    <tr style="border-width: 1px 0px 0px; background-color: white; margin: 0px; padding: 0px; border-color: #cccccc initial initial initial; border-style: solid initial initial initial;">
                        <th style="font-size: 1em; border: 1px solid #cccccc; margin: 0px; padding: 0.5em 1em; background-color: #f0f0f0;">Quantitative (or Numerical)</th>
                        <th style="font-size: 1em; border: 1px solid #cccccc; margin: 0px; padding: 0.5em 1em; background-color: #f0f0f0;">Qualitative (or Categorical)</th>
                    </tr>
                </thead>
                <tbody style="margin: 0px; padding: 0px; border: 0px;">
                    <tr class="" style="border-width: 1px 0px 0px; background-color: white; margin: 0px; padding: 0px; border-color: #cccccc initial initial initial; border-style: solid initial initial initial;">
                        <td class="" style="font-size: 1em; border: 1px solid #cccccc; margin: 0px; padding: 0.5em 1em; vertical-align: top;">
                            <p>Deals with numbers</p>
                            <ul>
                                <li>Can take an average, and the average has meaning</li>
                                <li>Can do other mathematics</li>
                            </ul>
                        </td>
                        <td style="font-size: 1em; border: 1px solid #cccccc; margin: 0px; padding: 0.5em 1em; vertical-align: top;">
                            <p>Deals with categories</p>
                            <ul>
                                <li>Words</li>
                                <li>Levels</li>
                                <li>Identification
                                    <ul>
                                        <li>Can be numbers, but an average is meaningless</li>
                                    </ul>
                                </li>
                            </ul>
                        </td>
                    </tr>
                    <tr style="border-width: 1px 0px 0px; background-color: #f8f8f8; margin: 0px; padding: 0px; border-color: #cccccc initial initial initial; border-style: solid initial initial initial;">
                        <td style="font-size: 1em; border: 1px solid #cccccc; margin: 0px; padding: 0.5em 1em;">
                            <p>Examples:</p>
                            <ul>
                                <li>GPA</li>
                                <li>Age</li>
                                <li>Weight</li>
                                <li>Height</li>
                                <li>Number of pets</li>
                                <li>Distances</li>
                                <li>Time (elapsed time: 25 seconds, 5 months, 42 years)</li>
                            </ul>
                        </td>
                        <td style="font-size: 1em; border: 1px solid #cccccc; margin: 0px; padding: 0.5em 1em;">
                            <p>Examples:</p>
                            <ul>
                                <li>Favorite ice cream flavor (Vanilla, Chocolate, Strawberry)</li>
                                <li>Grade Level (Freshman, Sophomore, Junior, Senior)</li>
                                <li>Grade Level (9, 10, 11, 12, 13+)</li>
                                <li>Phone number</li>
                                <li>ZIP Code</li>
                                <li>Student ID</li>
                                <li>Date (referenced time: January, 6th century, 2024)&nbsp;</li>
                            </ul>
                        </td>
                    </tr>
                </tbody>
            </table>

<iframe width="560" height="315" src="https://www.youtube.com/embed/sNPDOEc3a6w?si=39XQuSYhtot8ZWZh" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Examples
You want to collect data on the cell phone networks most commonly used among Snow College students. You collect *the network names* from 100 students. What type of variable is this?
  * Possible answers include {"Verizon Wireless", "AT&T", "T-Mobile", "Boost Mobile", "Cricket", ...}
  * These are just words, so math cannot be done on them
  * The students are categorized (or grouped together) based on their answer to this question
  * So, __this is a categorical variable__.

You want to study our dependence on computers. You ask Snow College students *how many computers are used in their houses*. What type of variable is this?
  * Possible answers are a number {1, 2, 3, 4, ...}
  * Although you could use the number of computers to categorize the students (such as "0-2 computer", "3-5 computers", "More than 5"), we want to focus on the numbers
    * Taking an average makes sense
  * So, __this is a quantitative variable__.

What regions of Utah are most represented by Snow College students? You ask students for their *ZIP codes*. What type of variable is this?
  * Possible answers are 5-digit numbers, such as {84102, 84109, 84627, 84642, 84698, ...}
  * Even though they are numbers, we aren't focusing on the number. They are only used to group students into regions
    * The average ZIP code doesn't make sense
  * So, even though the answers are numbers, __this is a categorical variable__.

## Practice
Here are a few variables. Determine if they are Quantitative or Categorical.
1. Age
    * After answering on your own, check the <button popovertarget="Problem_1">Solution</button>
2. Eye color
    * After answering on your own, check the <button popovertarget="Problem_2">Solution</button>
3. Value of a house
    * After answering on your own, check the <button popovertarget="Problem_3">Solution</button>
4. GPA
    * After answering on your own, check the <button popovertarget="Problem_4">Solution</button>
5. Pain Level (No pain, Little pain, Moderate pain, Strong pain, Intense pain)
    * After answering on your own, check the <button popovertarget="Problem_5">Solution</button>
6. Phone number
    * After answering on your own, check the <button popovertarget="Problem_6">Solution</button>


<div popover id="Problem_1">


## Problem 1.1.1
1. What type of variable is the "Age" variable? 

This is a number, and finding the average age makes sense, so this is a __Quantitative__ variable.

*Note*: It is often possible to take a Quantitative variable and use it to categorize your sample. For example, we can use the age to group people by age range: (Babies are ages 0-1, Toddlers ages 2-3, Children ages 4-8, ...). In this case, the age is used as a __Categorical__ variable.

<center><button popovertarget="Problem_1" popovertargetaction="hide">Close</button></center>
</div>

<div popover id="Problem_2">

## Problem 1.1.2
2. What type of variable is the "Eye Color" variable? 

It is not a number. Instead, people are grouped by the color of their eyes {Blue, Brown, Green, Hazel, ...}. So, this is a __Categorical__ variable.

<center><button popovertarget="Problem_2" popovertargetaction="hide">Close</button></center>
</div>
<div popover id="Problem_3">

## Problem 1.1.3
3. What type of variable is the "Value of a house"?

This is a number, and finding an average value of a house makes sense. So, this is a __Quantitative__ variable.

<center><button popovertarget="Problem_3" popovertargetaction="hide">Close</button></center>
</div>

<div popover id="Problem_4">

## Problem 1.1.4
4. What type of variable is a student's "GPA"?

This is a number, and finding the average GPA makes sense. So, this is a __Quantitative__ variable.

*Note*: The GPA is often used to group students as {"A-student", "B-student", ...} and to determine if students are in a certain group (such as the honor role).
* In this case, the GPA is still a Quantitative variable
* The GPA is used to create another variable that is Categorical

<center><button popovertarget="Problem_4" popovertargetaction="hide">Close</button></center>
</div>

<div popover id="Problem_5">

## Problem 1.1.5
5. What type of variable is a patient's "pain level"?

The pain level groups the patients into groups based on the amount of pain they report (no pain, low pain, etc.). So, this is a __Categorical__ variable.

<center><button popovertarget="Problem_5" popovertargetaction="hide">Close</button></center>
</div>

<div popover id="Problem_6">

## Problem 1.1.6
6. What type of variable is a person's "phone number"?

A phone number is a number, but taking the average makes no sense. A phone number is really an identification number as you want to identify the person you are calling. 
  * Loosely speaking, you can also use the phone number to group people by area code

So, the phone number is a __Categorical__ variable.

<center><button popovertarget="Problem_6" popovertargetaction="hide">Close</button></center>
</div>
