---
layout: post
title: "1. Overview and Factor Analysis"
date: 2020-01-01 00:01
comments: true
categories: intro
---

<a name="top"></a>
### Overview and factor analysis

[This block](http://tbates.github.io/Multivariate-Stats-Course) of the [MV course](http://www.drps.ed.ac.uk/current/dpt/cxpsyl11054.htm) introduces the idea of latent variables, the concept of a path diagram, on to general Structural Equation Modeling or SEM.

An [overview of the next 5 weeks is here](http://tbates.github.io/Multivariate-Stats-Course/intro/2020/12/01/outline.html)

1. Factor analysis
2. CFA & concepts of fit
3. Path Analysis: Regression and lm as a subset of SEM
4. Structural Equation Modelling
5. Latent variable modeling
6. Causality?


We begin this week by learning how to do a factor analysis in R.

Show how the EFA needs to fix latent variances at 1 and covariances at 0, and fix the upper right triangle of whatever matrix contains the latent loadings.

Show what rotation does (R is great for that - just pull the loadings matrix and throw in at promax() or varimax().

Introduce indeterminacy by talking about how the rotations do not differ in fit.

### How many factors?
#### Horn's Parallel analysis

http://stats.stackexchange.com/questions/97802/how-to-correctly-interpret-a-parallel-analysis-in-exploratory-factor-analysis

### Rotation

We now know about loadings

### Scores: Why scores are not just data %*% loadings

http://stackoverflow.com/questions/4145400/how-to-create-factors-from-factanal

Can we construct scores on our factors?

An intuition might be: Factors = data matrix * Loadings matrix.

1. Thomson Regression method restriction that the scores are uncorrelated, centered around 0 and with variance = 1.
 * 'scale(m1) %*% solve(cor(m1)) %*% loadings(fa)'
2. Bartlett's method
3. ML


```splus
v1 <- c(1,1,1,1,1,1,1,1,1,1,3,3,3,3,3,4,5,6)
v2 <- c(1,2,1,1,1,1,2,1,2,1,3,4,3,3,3,4,6,5)
v3 <- c(3,3,3,3,3,1,1,1,1,1,1,1,1,1,1,5,4,6)
v4 <- c(3,3,4,3,3,1,1,2,1,1,1,1,2,1,1,5,6,4)
v5 <- c(1,1,1,1,1,3,3,3,3,3,1,1,1,1,1,6,4,5)
v6 <- c(1,1,1,2,1,3,3,3,4,3,1,1,1,2,1,6,5,4)
m1 <- cbind(v1,v2,v3,v4,v5,v6)

fa <- factanal(m1, factors=3,scores="regression")

fa$scores # the correct solution

fac <- m1 %*% loadings(fa) # the answer on your question
```

```splus
> round(cor(fac),2)
        Factor1 Factor2 Factor3
Factor1    1.00    0.79    0.81
Factor2    0.79    1.00    0.82
Factor3    0.81    0.82    1.00

> round(cor(fac2),2)
        Factor1 Factor2 Factor3
Factor1       1       0       0
Factor2       0       1       0
Factor3       0       0       1
```

#### What happens with missing data

**Next week**: We will convert this model to CFA. Use a real data set so it has a purpose.


## Refs
1. http://www.psy.ed.ac.uk/people/iand/Bartholomew%20%282009%29%20Br%20J%20Math%20Stat%20Psychol%20factor%20scores%20Thomson%20Spearman%20Bartlett.pdf