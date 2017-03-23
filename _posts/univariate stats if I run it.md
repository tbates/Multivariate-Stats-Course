We don't teach operant or pavlovian conditioning: that's a gaping hole in understanding behaviour (I had 2 people in a 4th year class of 45 (which is way too big) who knew what operant conditioning was).

We should have a class where students make suggestions for business, and coaching people, using psychology. Otherwise what are we learning?

# Univariate or Multivariate stats
## Timothy C. Bates
## Edinburgh University

### Course Wiki

### Syllabus
In this course you will learn how to conduct univariate statistics using R. You will learn how to install and configure R, and develop an understanding of statistics via lectures and, importantly, doing statistics in the statistical language R. We will read in data, creating and explore graphics, access additional packages in R, create some basic functions, and conduct mini projects

### Objectives
After taking this course you should be able to

* Read formatted data into R
* Subset, remove missing values from, and clean tabular data
* Write custom functions in R to implement new functionality and making use of control structures such as loops and conditionals
* Use the R code debugger to identify problems in R functions
* Make a scatterplot/boxplot/histogram/image plot and modify a plot with custom annotations
* Define a new data class in R and write methods for that class
* Lecture Materials
* Lecture videos will be released weekly and will be available for the week and thereafter. 

You are welcome to view them at your convenience. Accompanying each video lecture will be a PDF copy of the slides, unless the lecture is a demo, in which case there will be no lecture slides.

#### Quizzes
There will be four weekly quizzes that will test your comprehension of the material covered in the lecture material provided that week. The quizzes will consist of multiple choice, true/false, or short answer questions. Each quiz is worth 10 points. You will be allowed 3 attempts to submit each quiz and your maximum score will be taken as the final score.

#### Quiz Opening/Closing Dates
Quiz 1: 2012-09-24 12:00:00 AM PDT to 2012-09-30 11:59:00 PM PDT
Quiz 2: 2012-10-01 12:00:00 AM PDT to 2012-10-07 11:59:00 PM PDT
Quiz 3: 2012-10-08 12:00:00 AM PDT to 2012-10-14 11:59:00 PM PDT
Quiz 4: 2012-10-15 12:00:00 AM PDT to 2012-10-21 11:59:00 PM PDT
#### Assignments
There will be two programming assignments that will involve writing R code and R functions. These assignments will allow you to work on your R programming skills and practice writing and debugging code. For each programming assignment you will be asked to write R code or functions that produce output given a certain input. Your grade on the assignment will be based on whether the output your function produces matches the correct output. Details can be found in the descriptions of each programming assignment.

Each programming assignment is worth 30 points and is broken down into sub-parts. For each sub-part you will be allowed an unlimited number of submissions and your latest score will be taken as the final score.

Programming Assignment Due Dates
Programming Assignment 1: 2012-10-07 11:59:00 PM PDT
Programming Assignment 2: 2012-10-21 11:59:00 PM PDT


## Grading
Your grade in this course will consist of performance on four weekly quizzes and two programming assignments. The breakdown of the weighting for these elements is

Week 1 Quiz: 10 points
Week 2 Quiz: 10 points
Week 3 Quiz: 10 points
Week 4 Quiz: 10 points
Assignment 1: 30 points
Assignment 2: 30 points

There is a maximum of 100 points to obtain in this course through the four quizzes and the two programming assignments.

The final grade for the course is based on your total score on the four quizzes and two assignments.

## Class Schedule
#### Week 1
* Introduction and overview
* Installing R
* Data types, subsetting
* Reading/writing data
#### Week 2
* Control structures
* Functions
* Loop functions
* Debugging
#### Week 3
* Simulation
* Plotting, visualizing data
* Principles of data graphics 
#### Week 4
* Objected oriented programming
* Data abstraction
* Statistical modeling 


Skip Navigation This page features MathJax technology to render mathematical formulae. If you are using a screen reader, please visit MathPlayer to download the plugin for your browser. Please note that this is an Internet Explorer-only plugin at this time. Computing for Data Analysis
Top Navigation Bar
COURSESABOUT TIMOTHY BATES 
 

Computing for Data Analysis
Roger D. Peng
Johns Hopkins University
Side Navigation Bar
Home

Video Lectures

Discussion Forums

Additional Documents

Quizzes

Programming Assignments

Syllabus

About the Instructors

Join a Meetup

Course Wiki

Week 1 Quiz
This quiz will assess your knowledge of the material covered in Week 1.
1	R was developed by statisticians working at<break>The University of Auckland<break>StatSci<break>Bell Labs<break>Harvard University"
The 'L' suffix creates an integer vector as opposed to a numeric vector.
2	The definition of free software consists of four freedoms (freedoms 0 through 3). Which of the following is NOT one of the freedoms that are part of the definition?<break>The freedom to study how the program works, and adapt it to your needs.<break>The freedom to restrict access to the source code for the software.<break>The freedom to improve the program, and release your improvements to the public, so that the whole community benefits.<break>The freedom to redistribute copies so you can help your neighbor.
This is not part of the free software definition. Freedoms 1 and 3 require access to the source code.
3	In R the following are all atomic data types EXCEPT<break>numeric<break>integer<break>list<break>logical
'list' is not an atomic data type in R.
4	If I execute the expression x <- 4L in R, what is the class of the object `x'?<break>character<break>logical<break>matrix<break>integer
The 'L' suffix creates an integer vector as opposed to a numeric vector.
5	What is the class of the object defined by x <- c(4, TRUE)?<break>integer<break>numeric<break>matrix<break>character
The numeric class is the "lowest common denominator" here and so all elements will be coerced into that class.
6	If I have two vectors x <- c(1,3, 5) and y <- c(3, 2, 10), what is produced by the expression cbind(x, y)?<break>a 2 by 3 matrix<break>a vector of length 3<break>a vector of length 2<break>a numeric matrix with 3 rows and 2 columns
7	A key property of vectors in R is that<break>a vector cannot have have attributes like dimensions<break>elements of a vector can only be character or numeric<break>elements of a vector all must be of the same class<break>elements of a vector can be of different classes
8	Suppose I have a list defined as x <- list(2, "a", "b", TRUE). What does x[[1]] give me?<break>a list containing the number 2<break>a list containing a numeric vector of length 1<break>a character vector containing the element "2"<break>a numeric vector containing the element 2.
9	Suppose I have a vector x <- 1:4 and a vector y <- 2. What is produced by the expression x + y?<break>a numeric vector with elements 3, 4, 5, 6<break>a numeric vector with elements 1, 2, 3, 6.<break>an integer vector with elements 3, 2, 3, 6.<break>a numeric vector with elements 3, 2, 3, 6.
10	Suppose I have a vector x <- c(3, 5, 1, 10, 12, 6) and I want to set all elements of this vector that are less than 6 to be equal to zero. What R code achieves this?<break>x[x < 6] == 0<break>x[x <= 5] <- 0<break>x[x > 6] <- 0<break>x[x == 6] <- 0"
You can create a logical vector with the expression x <= 5 and then use the [ operator to subset the original vector x.

In accordance with the Honor Code, I certify that my answers here are my own work.