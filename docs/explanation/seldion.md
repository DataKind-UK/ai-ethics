# [Seldon.io Alibi]

**Description of the tool**

**What is its purpose?**

All purpose framework for handling a range of explanations [local/global]

But also model monitoring via outliers - metrics to test model: drift [when to retrain], outliers/adversarial usage (e.g. is something an outlier, what feature make it an outlier, etc)

Open source

**_Who is the intended user?_**

Developers

Operators (i.e. those who have deployed models - being used in practice)

**_What is its scope (algorithms, data, types of challenges)?_**

Supports a large number of approaches, different data types

e.g . show most important features, counterfactuals, explain the reason why a model gave a given label.

![alt_text](../_media/image25.png "image_tooltip")

The tool is designed to work well with libraries with an API similar to scikit-learn (and its own API is close to that standard, see image below).

![alt_text](../_media/image26.png "image_tooltip")

**Best for:**

All purpose framework for handling explanations, and model monitoring. It works well with both unstructured data (NLP, computer vision) and tabular data; it covers different tasks (both regression and classification) and contains different state-of-the-art algorithms.

The documentation is very comprehensive, including code for many many practical examples:

  *   different approaches
  *   different tasks
  *   in different contexts (different datasets)
