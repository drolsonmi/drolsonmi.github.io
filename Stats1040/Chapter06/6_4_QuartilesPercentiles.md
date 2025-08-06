# 6.4 Quartiles and Percentiles

## Reading

## Lesson
### Quartiles

### Percentiles

## Practice

## Technology
There are a few different ways to calculate quartiles. Different software calculates the quartiles differently. The method we learned here is the method used by the TI-83/TI-84. However, it is useful to see how it is done with other technologies.

For homework and exams, we will stick with the TI-84 method as we learned. So if you have a different calculator, then be sure you know how to do this method by hand.

### TI-83/84

### Excel
Excel does not calculate quartiles like we did in class. It interpolates between values, then finds the 25th percentile. For example, if your dataset is {0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10}, then
* Excel will add values between these values to give us 100 points:
  * {0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1, 1.1, 1.2, 1.3, 1.4, 1.5, 1.6, 1.7, 1.8, 1.9, 2, 2.1, 2.2, ..., 9.8, 9.9, 10}
* Excel will then find the 25th percentile, which in this case would be 2.5

It is important to be aware of this as the results be differ from the results of a TI-84.

There are 3 different functions
* `=quartile.inc([array],[quartile])`
    * Includes the minimum and the median to find Q1
    * Includes the median and the maximum to find Q3
* `=quartile.exc([array],[quartile])`
    * Excludes the minimum and the median to find Q1
    * Excludes the median and the maximum to find Q3
* `=quartile([array],[quartile])`
    * Follows the `quartile.exc` calculation

### Desmos
