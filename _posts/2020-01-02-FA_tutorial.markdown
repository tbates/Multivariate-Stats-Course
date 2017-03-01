---
layout: post
title: "Overview and Factor Analysis"
comments: true
categories: intro
---

## Tutorial 1.

1. Find and load the `bfi` dataset (in the psych package).
2. Find a package in R that does parallel analysis
	* What is it's name?
	* What is the name of the function?
	* *tutor note*: Introduce the package and function we wish to work with now.
3. Read the help
	* What parameters does this parallel analysis function take?
	* What do they do?
4. Use the function to determine how many factors are in the bfi dataset
	* How many?
	* What is a screen plot?
5. Find R's built in factor analysis function
	* What is it?
	* *tutor note* - share the `correct` answer with the class
	* What parameters does this function need?
	* What are its options? Discuss.
6. Run an fa, extracting the predicted number of factors from paran
	* Was what you ran by default oblique or orthogonal?
	* What is the name of an oblique rotation?
	* *tutor-note* share the correct answer before continuing.
7. Use the oblique rotation
	* Is the structure "simple"?
	* What does that mean?
	* What are the factors? ( Name them based on high loadings)
10. Try and alter how the result prints out
	* The factor analysis object has a special print method, which supports sorting and hiding small values!
	* Are the factors independent?
	* What component of the print out tells us this?
12. Create scores for each subject (hint, the factor analysis function has a scores parameter)
13. Add these to the dataset.

**Bravo!**

## Extra credit if you finish early
1. Try doing all of this with IQ data set Holzinger from `psych`
2. Do an FA on some of your own data, or mtcars, or ... anything else: practise creates skill.

### To prepare for next week's tutorials and lectures
1. Install the package `umx`
2. Read the `?umxRAM` help, and run a model in its help examples
3. Try and re-run one of the factor analyses using `umxFactanal`

### Scientific as opposed to statistical Questions:
1. Do you think personality has 5 or 6 major domains?
2. Is the test good?
3. What would happen to the parallel analysis if we sampled facets better?
4. What could go wrong if the data have a hierarchical structure like we know personality does?
