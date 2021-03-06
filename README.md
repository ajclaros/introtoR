<!-- TABLE OF CONTENTS -->
## Table of Contents

* [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
  * [Programming Primer](#pragramming-primer)
  * [Parts of the Presentation](#parts-of-the-presentation)

  * [Links](#Links)



<!-- GETTING STARTED -->
## Getting Started

On this page, click the green "clone or download" button and choose the "Download Zip" option, save and extract to your desktop or another folder.

### Prerequisites

Make sure you have the [R](https://cran.r-project.org/) language and 
[RStudio](https://rstudio.com/products/rstudio/) installed


### Programming primer

1. IDE: Integrated development Environment. The reason we use RStudio is because it gives us nice ways to view our data and graphs! Just downloading R would mean we're esesntially programing from a command line
2. Comments: Comments are not read by the language interpreter (what runs your program/script) you can use them to make notes for yourself and others to help understand what is being done
```{r}
#this is a comment. Everything after the "#" will be ignored by R
```
3. Variable: How we name and store data when we program. By invoking x=3, everytime we use the name "x" we will be working with the number 3. Creating variable names is important because we don't want to be creating data from scratch every time we use it. This of it like shoving data into a box and then labeling it.

A good naming convention is to start your variable names with a lowercase letter. It is especially important to name them something useful so that anyone else (especially you) can understand your code
```{R}
thisisavariable
thisIsAVariable
this_is_a_variable
this.is.a.variable
variableName2
ThisIsABadName #starts with a capital letter
$thisisnotavariable #R has a specific use for for "$"
```
4. String: A type of data, Think "text". A series of characters that can be put together between qotation marks.
```{r}
"this is a string" # this group of characters including spaces can all be seen as a single item
sentence = "this is a string." #assign "this is a string" to "sentence" 
print(sentence) 
print("this is a string")
```
5. Function: A sequence of repeated steps that are stored under a name. We also store functions so that we dont need to write them over again each time. A function could be named "sum" which sums up all the numbers given to it
6. Argument: a type of variable/input that dictates how a function works. 
```{r} 
combine(x, how) #is a function named "combine" which takes in two arguments, "x" and "how"
``` 
if I had some data, a = (1, 2, 3) and typed combine(a, "subtract") it combines the list by subtracting
```{r}
combine(a, "subtract")    #would print: -4
combine(a, "add")         #would print: 6
combine(a, "concatenate") #would print: "123", note this prints a string because that is how you "combine" numbers
```
7. Dataframe: Think "excel sheet". It allows us to organize our data where each row is an observervation and each column dictates what type of data will be below it. Most of the data you will be working with may be in formats similar to this

### Parts of the Presentation
1. Quick introduction to R and programming
2. How to hit the ground running

While it is important to understand programming basics including the ins and outs of the R language, that is not the purpose of this presention. It is important for us to learn how to use tools that have been built for us, and with experience perhaps build our own.
We will more often than not be reading other's code, data and documentation of how to use their code/data in order to acomplish a task specific to us (maybe providing unique analysis or graphs to visualize). So the second part is a demonstration of how I would go about digesting and learning code that someone else wrote. For this presentation I will be using the R package [Patternize](https://github.com/StevenVB12/patternize)

What is shown in the tutorial is a very brief overview of what is capable in the R language. There are countless of free resources to really get into the depths of R and programming if one were inclined (the internet is your friend!) at the bottom of this README file are some links and websites that I've found useful in my learning. They are not necessarily exclusive to R, but are good resources to learn how to program.


### Links
* [Introduction to Data Science
Data Analysis and Prediction Algorithms with R](https://rafalab.github.io/dsbook/)
  This free book walks you from beginnings of R and programming and teaches you how to make graphs with data

* [The Coding Train](https://www.youtube.com/user/shiffman)
  * [Processing Tutorial](https://www.youtube.com/playlist?list=PLRqwX-V7Uu6ZYJC7L-r6rX6utt6wwJCyi)
  * [Nature of Code](https://www.youtube.com/playlist?list=PLRqwX-V7Uu6aFlwukCmDf0-1-uSR7mklK)
  The Coding train is a Youtube channel that has tons of introductory programming tutorials (introductory to advanced) that uses the languages Processing and Javascript. Daniel Shiffman is great to watch and learn from! He often streams himself trying to program and walks you through his thought process. Can't recommend him enough!
* You will at some point be getting _very_ familiar with [https://stackoverflow.com/](https://stackoverflow.com/)
* The dataset compensation.csv was taken from [r4all.org](http://r4all.org/books/datasets/) which is used in the book [Getting Started with R: An Introduction for Biologists
](http://r4all.org/books/gswr2/)
