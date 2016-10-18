---
layout: post
title: "Path Analysis: Regression and lm as a subset of SEM"
comments: true
categories: intro
---

<a name="top"></a>
### Introduces
* The idea of causality, testing (and, critically, mxCompare()-ing) ideas. And use real tasks, such as handling a ordinal outcomes as thresholded normals.
* **Tutorial**: Specific SEM models
* *Curb your enthusiasm*: By this week you should understand what boxes, circles, triangles, diamonds, and straight and curved arrows are. 

### Regression and lm as a subset of SEM

This week we will leverage the modelling you already know by building the equivalent of `lm(y ~ x + z)` in `umx` package.

This builds on two ideas you already understand: Factor analysis and linear models/ANOVA.</li>

### Regression and lm as a subset of SEM



| Regression                          | SEM                                    |
|:------------------------------------|:---------------------------------------|
| Only one dependent variable.        | Multiple dependent variables.          |
| Independent variables covaried out. | IVs correlate or influence each other. |
| Assumes measures error free.        | Separates measurement from structure.  |
