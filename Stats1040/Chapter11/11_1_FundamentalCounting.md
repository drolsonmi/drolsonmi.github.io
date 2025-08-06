# 11.1 Fundamental Counting Rule

## Outlook of Lesson 11
In lessons 9 and 10, we have learned about basic probability calculations. These by themselves will help with doing calculations of Categorical variables. However, __probability theory__ expands what we have learned to get more sophisticated calculations. We'll introduce some of the concepts of probability theory by looking at Probability Distributions (Lesson 12) and Binomial Distributions (Lessons 13 and 14).

In order to understand these, we need to talk about the __rules of counting__. These are just a few probability tools that we will need for lessons 12-14. These tools are:
* Lesson 11.1 Fundamental Counting Rule
* Lesson 11.2 Factorials
* Lesson 11.3 Permutations
* Lesson 11.4 Combinations

## Reading

## Lesson
We have discussed the probabilities of a single event (lessons 9-10). But what if you have multiple events at the same time? For example, we roll not one die but two dice. Or instead of choosing marbles from 5 different bags. Or choosing toppings for a pizza (choosing meats, cheese, and toppings). All of these have multiple events. In this lesson, we will learn how to calculate the probabilities of multiple events.

Consider two dice - one 4-sided white die and one 6-sided black die. If the white die rolls a 3, we'll call that `W3`, and if the black die rolls a 5, we'll call that `B5`. Now, roll the dice. How many possibilities are there?
* If we roll `W1`, there are 6 possibilities for black: (`W1,B1`),(`W1,B2`),(`W1,B3`),(`W1,B4`),(`W1,B5`),(`W1,B6`)
* If we roll `W2`, there are 6 possibilities for black: (`W2,B1`),(`W2,B2`),(`W2,B3`),(`W2,B4`),(`W2,B5`),(`W2,B6`)
* If we roll `W3`, there are 6 possibilities for black: (`W3,B1`),(`W3,B2`),(`W3,B3`),(`W3,B4`),(`W3,B5`),(`W3,B6`)
* If we roll `W4`, there are 6 possibilities for black: (`W4,B1`),(`W4,B2`),(`W4,B3`),(`W4,B4`),(`W4,B5`),(`W4,B6`)
* *Bottom line*: There are 4 possibilities for the white die. For each possibility, there are 6 possibilities for the black die. That is a total of $4\times 6 = 24$ possibilities

That's it! That is the __Fundamental Counting Rule__. 
> If event A has $k$ different possibilities, and event B has $n$ different possibilities, then __the total number of combined possibilities is $k\times n$__.

What about 3 events? Let's take the 4-sided white die and the 6-sided black die, and we'll add a 10-sided red die.
* There are 24 possibilities with the white and black dice
* For each possibility with the white and black dice, there are 10 possibilities for the red die
* That's a total of $24\times 10 = 240$ possible combinations

The complete __Fundamental Counting Rule__.
> For multiple events, let's say that event $i$ has $n_i$ different possible outcomes. __The total possible combinations is, $n_1 \times n_2 \times n_3 \times \dots$__.

## Practice
Here are three example problems using the Fundamental Counting Rule. Answer the questions to the best of your ability then *afterwards* check the answer.

### Practice Problem 1
Papa Miguel's pizza place allows you to choose your sauce, cheese and 1 topping for a flat price. The menu has the following options:
* Sauce: Tomato, BBQ, Alfredo
* Cheese: Mozerella, 5-cheese, Mexican, Parmesan
* Toppings: Pepperoni, Sausage, Chicken, Ham, Bacon, Pineapple, Onion, Taco Beef

How many possible pizza combinations could you create?

#### Answer to Practice Problem 1
There are 3 sauces, 4 cheese options, and 8 toppings. So, there are $3\times 4\times 8 = 96$ different combinations.

### Practice Problem 2
There are 13 people in a race. How many ways can the 13 runners cross the finish line?

#### Answer to Practice Problem 2
* There are 13 different contestants who can place 1st.
* There are 12 different contestants who can place 2nd (all but the 1st place contestant).
* There are 11 different contestants who can place 3rd (all but the 1st and 2nd place contestants).
* There are 10 different contestants who can place 4th (all but the 1st, 2nd, and 3rd place contestants).
* There are 9 different contestants who can place 5th (all but the 1st, 2nd, 3rd, and 4th place contestants).
* There are 8 different contestants who can place 6th (all but the 1st - 5th place contestants).
* There are 7 different contestants who can place 7th (all but the 1st - 6th place contestants).
* There are 6 different contestants who can place 8th (all but the 1st - 7th place contestants).
* There are 5 different contestants who can place 9th (all but the 1st - 8th place contestants).
* There are 4 different contestants who can place 10th (the last 4 runners).
* There are 3 different contestants who can place 11th (the last 3 runners).
* There are 2 different contestants who can place 12th (the last 2 runners).
* There is only 1 contestant who can place 13th (the last runner).

Using the Fundamental Counting Rule, there are $13\times 12\times 10\times 9\times 8\times 7\times 6\times 5\times 4\times 3\times 2\times 1 = \mathbf{6,227,020,800}$ possible ways the 13 contestants can cross the finish line.

### Practice Problem 3
If you have a secure password, then it is very difficult for a hacker to randomly guess your password. Is it safer to have an 8-character password that can contain any character \{a-z, A-Z, 0-9, !@#$%^&*() \} or a 12-character password with only lower-case letters? 

Take a second and make a guess as to which is more secure. Then use the Fundamental Counting Rule to find the number of possible 8-character and 12-character passwords. The option with more possible passwords would be more secure as it is more difficult to randomly guess.

#### Answer to Practice Problem 3
For the 8-character complex password, there are 26 letters (lower- and upper-case), 10 digits, and 10 special characters. That is a total of 72 different characters. Each character of the password can be any of the 72 characters, so there are (72 * 72 * 72 * 72 * 72 * 72 * 72 * 72) = 72^8 = 7.222*10^{14} = 722,200,000,000,000 (722.2 trillion) different possible passwords.

For the 12-character simple password, there are only 26 different possible characters. Each character can be any of the 26 characters, so there are (26 * 26 * 26 * 26 * 26 * 26 * 26 * 26 * 26 * 26 * 26 * 26 = 26^12 = 9.543*10^{16} = 95,430,000,000,000,000 (95.4 quadrillion) different possible passwords.

Since there are more possible passwords for the 12-character simple password, this would be more secure password.

*Note*: Of course, length combined with complexity is a better option, so the more secure option would be a 12-character password with any character \{a-z, A-Z, 0-9, !@#$%^&*() \}. Passphrases that are 15-30 characters long are even more secure. However, these options weren't addressed in the question.
