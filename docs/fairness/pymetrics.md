## **[PyMetrics Audit AI](https://github.com/pymetrics/audit-ai)**

**Overall evaluation**

_Technical Implementation_

Useful: 2/5
Comprehensive: 2/5
Technical scalability: 2/5
Easy to customize (data): 2/5
Easy to customize (visualizations / analyses): 5/5
Easy to integrate: 5/5
Robustness: ?/5

_User-friendliness (system usability scale)_

Answer with strongly agree (5), agree (4), neutral (3), disagree (2), strongly disagree (1)

1. I think that I would like to use this system frequently: 3
2. I found the system unnecessarily complex: 1
3. I thought the system was easy to use: 5
4. I think that I would need the support of a technical person to be able to use this system: 1 (assuming user is a DS/DA)
5. I found the various functions in this system were well integrated: 5
6. I thought there was too much inconsistency in this system: 1
7. I would imagine that most people would learn to use this system very quickly: 5
8. I found the system very cumbersome to use: 1
9. I felt very confident using the system: 4
10. I needed to learn a lot of things before I could get going with this system: 1

## Description of the tool

What is its purpose?

_Measure the effects of discriminatory patterns in training data and the predictions_

Who is the intended user?

_Data Scientist evaluating socially sensitive decision processes in ML_

What is its scope (algorithms, data, types of challenges)?

_Measure disparate impact in data and predictions_

**Best for: **

What should practitioners use this tool for? Are there any scenarios / use cases in which this tool is particularly helpful vs. useless?

This tool is great at looking at one form of fairness: disparate impact. This concept is often used in the law for standards of selection procedures. If an algorithm leads to a disparity between protected groups (gender, race, age 40+), then it may not be used as part of the selection procedure.

However, we know that there are several definitions of fairness that are more appropriate for cases as credit modelling.

I’d only use this tool if my only goal is to measure disparate impact.

## Pros & cons

What are the benefits of this tool?

- Very easy to install and follow the instructions on its examples

- Includes adverse impact over time

What are the challenges in using this tool?

- This tool includes only one form of fairness. That is if groups are different according to a standard of statistical significance (e.g.: 4/5th, fisher, z-test, bayes factor, chi squared)

- It does not include more bias metrics as Equalised Odds that may be more appropriate for many classification models

- Examples do not explain how to interpret the results in the context of bias. Whoever uses the tool could not draw relevant conclusions from the examples.\_

- Assumes you’re very familiar with all statistical test, some extra information on them would have been useful

## Limitations, especially any technical issues

Limited to only one form of fairness definition

## Case study demo with screenshots

[Student Performance dataset](https://github.com/pymetrics/audit-ai/blob/master/examples/StudentPerformanceData_BiasCheck.ipynb)

- The example shows how easy it is to install, import and use the package

![alt_text](../_media/image15.png "image_tooltip")

![alt_text](../_media/image16.png "image_tooltip")
