# **[IBM Fairness 360](https://github.com/IBM/AIF360)**

**Overall evaluation**

_Technical Implementation_

Useful: 2/5

Comprehensive: 4/5

Technical scalability: 4/5

Easy to customize (data): 4/5

Easy to customize (visualizations / analyses): 2/5

Easy to integrate: 2/5

Robustness: 3/5

_User-friendliness (system usability scale)_

Answer with strongly agree (5), agree (4), neutral (3), disagree (2), strongly disagree (1)

Feel free to add comments and justifications!

I think that I would like to use this system frequently: 3

I found the system unnecessarily complex: 3

I thought the system was easy to use: 2

I think that I would need the support of a technical person to be able to use this system: 5

I found the various functions in this system were well integrated: 4

I thought there was too much inconsistency in this system: 3

I would imagine that most people would learn to use this system very quickly: 1

I found the system very cumbersome to use: 4

I felt very confident using the system: 2

I needed to learn a lot of things before I could get going with this system: 5

**Description of the tool**

A repository of 9 different debiasing algorithms covering pre,. during, and post modelling phases. Not only a python package but also an interactive demonstration that provides an introduction to fairness concepts in AI, as well as examples of 3 different datasets.

Pre-Processing:

- Reweighing: Weights the examples in each (group, label) combination differently to ensure fairness before classification.

- Optimised Preprocessing: Learns a probabilistic transformation that can modify the features and the labels in the training data.
  In-Processing:

- Adversarial Debiasing: Learns a classifier that maximizes prediction accuracy and simultaneously reduces an adversary's ability to determine the protected attribute from the predictions. This approach leads to a fair classifier as the predictions cannot carry any group discrimination information that the adversary can exploit.
  Post-Processing:

- Reject Option Based Classification: Changes predictions from a classifier to make them fairer. Provides favorable outcomes to unprivileged groups and unfavorable outcomes to privileged groups in a confidence band around the decision boundary with the highest uncertainty.

**Best for: **

Data Scientists + Model builders looking for quick and easy ways to “de-bias” their system, at all stages of the pipeline.

**Pros & cons**

Pros:

1. Fairly comprehensive selection of tutorial notebooks to learn from:[ https://github.com/IBM/AIF360/tree/master/examples](https://github.com/IBM/AIF360/tree/master/examples)

2. Can Integrate easily in sklearn[ https://github.com/IBM/AIF360/blob/master/examples/sklearn/demo_new_features.ipynb](https://github.com/IBM/AIF360/blob/master/examples/sklearn/demo_new_features.ipynb)

3. Well defined API with lots of functionality.

**Limitations, especially any technical issues**

There is a general consensus that “De-Bias”ing algorithms do not actually lead to fairer systems in general, so whilst this package is a good starting point to thinking about how a dataset can be altered, or a model’s behavior changed with fairness in mind it might not be that effective in practice.

The tool is not very effective at identifying who might be being treated unfairly within a system and where that bias might be originating from.

Perhaps a steep learning curve in terms of integrating into an existing model building pipeline

**Case study demo with screenshots**

![alt_text](../_media/image10.png "image_tooltip")

![alt_text](../_media/image11.png "image_tooltip")
