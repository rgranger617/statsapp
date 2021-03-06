Hypothesis Test Calculator
========================================================
author: Robert Granger
date: Thu Jan 14 2016
<a href="https://github.com/rgranger617/statsapp">GITHUB Code and Slides</a>


========================================================

## What does the App do?

1. The application conducts a hypothesis test on the mean given some inputs.
2. Shows an interactive graph of the sampling distribution with the rejection region in red.
3. Lists important statistics like the critical values, p-values, etc...
4. Gives a conclusion on whether one should reject or not reject.

## Why is this App useful?
1. Hypothesis testing can be complicated and easy to make mistakes.
2. Much quicker than conducting the test from scratch.
3. Excellent tool for new learners of statistics to better understand the concept.

The User Interface
========================================================

<img src="hypothesistest-figure/inputbar.jpg" width="150%">

***

-4 regular text inputs (although they take numbers)

-2 sets of radio buttons

-1 numeric input




Sampling Distribution Graph
========================================================

<img src="hypothesistest-figure/normdist.png">

```r
#Creating the plot#
curve(dnorm(x,mu,SE),xlim=c(boundl,boundu),main=
'Normal Density',ylab="",yaxt="n",xlab="Sample Mean")
```
Note: See code for how to add the colors.

Hypothesis Test
========================================================
The final part of the application is the test itself.

<img src="hypothesistest-figure/output.png">

The application gives all the useful statistics along with a conclusion.
