## EthicalML XAI

Disclaimer: this library is in alpha (0.0.4) and does not seem to be maintained very often (last commit from 10 months ago). The documentation is also partly broken/ obsolete, please use README.md as (not entirely complete) reference

**Github:[ https://github.com/EthicalML/XAI](https://github.com/EthicalML/XAI)**

**Manifesto:[ https://ethical.institute/principles.html#commitment-3](https://ethical.institute/principles.html#commitment-3)**

**Documentation :[ https://ethicalml.github.io/xai/index.html](https://ethicalml.github.io/xai/index.html)**

**Example: [https://github.com/EthicalML/xai/blob/master/examples/XAI%20Tabular%20Data%20Example%20Usage.ipynb](https://github.com/EthicalML/xai/blob/master/examples/XAI%20Tabular%20Data%20Example%20Usage.ipynb)**

**Overall evaluation**

_Technical Implementation_

Useful: 3/5
Comprehensive: 3/5
Technical scalability: 2/5
Easy to customize (data): 3/5
Easy to customize (visualizations / analyses): 3/5
Easy to integrate: 3/5
Robustness: 1/5

**_User-friendliness (system usability scale)_**

1. I think that I would like to use this system frequently: 2 - it does not add much to the usual stack
2. I found the system unnecessarily complex: 1 - it is very simple to use
3. I thought the system was easy to use: 5 - it is extremely easy because it makes it simple to check for unbalance as part of the usual model development cycle
4. I think that I would need the support of a technical person to be able to use this system: 4 - it is targeted as ML engineers or DS
5. I found the various functions in this system were well integrated: 4 - agree
6. I thought there was too much inconsistency in this system: 2- it seems to be quite consistent in how it is to be used
7. I would imagine that most people would learn to use this system very quickly: 3 - they would be able to learn it quickly, provided that they are familiar with the standard model development workflow
8. I found the system very cumbersome to use: 2 - it is fairly simple
9. I felt very confident using the system: 4 - it looks something I could use straight out of the box
10. I needed to learn a lot of things before I could get going with this system: 1 - Reading the quick walkthrough was enough.

**Description of the tool**

**What is its purpose?**

XAI is a Machine Learning library designed to enable explainability at different steps of the ML workflow:

1. data analysis
2. model evaluation
3. production monitoring.

The aim is identifying discrepancies that may result in sub-optimal performance relative to the objectives required.

**Who is the intended user?**

Machine learning engineers and relevant domain experts

**What is its scope (algorithms, data, types of challenges)?**

1. Identifying unbalances in the data during EDA
2. Re-balance the data by downsampling / upsampling (including in train/test split)
3. Improving model evaluation:
   - Features importance (permutation importance)
   - Metric importance against all test data
   - Identify metric imbalances grouped by protected features
   - Visualise the ROC/ precision-recall curves grouped by protected features (and their deviation re the global curves)
   - Visualise performance metrics grouped by probability buckets

**Best for: **

_What should practitioners use this tool for? Are there any scenarios / use cases in which this tool is particularly helpful vs. useless?_

This tool is automating and making easier some analysis that are already possible using the standard industry packages (e.g. scikit-learn and matplotlib), without adding any new algorithms or techniques.

It can be useful to junior engineers/scientists as it makes it easier for them to spot and address unbalance in data or model predictions, but it seems very basic compared to other libraries in the same space.

**Pros & cons**

What are the benefits of this tool?

- Easy to use
- Easy to read and use the outputs

What are the challenges in using this tool?

- Not very sophisticated
- It does not add much to what is already available in the space

**Limitations, especially any technical issues**

It only works for structured (tabular) data.

**Case study demo with screenshots**

The examples in the documentation work only partially, see e.g.:

![alt_text](../_media/image21.png "image_tooltip")

## [MLI Resources](https://github.com/h2oai/mli-resources)

**Overall evaluation**

_Technical Implementation_

Useful: 3/5

Comprehensive: 2/5

Technical scalability: 2/5

Easy to customize (data): 4/5

Easy to customize (visualizations / analyses): 4/5

Easy to integrate: 2/5

Robustness: ?/5

**_User-friendliness (system usability scale)_**

1. I think that I would like to use this system frequently: 3
2. I found the system unnecessarily complex: 2
3. I thought the system was easy to use: 4
4. I think that I would need the support of a technical person to be able to use this system: 5 ( you would need a technical person if not a developer, as it requires understanding of setting up Docker, along with Python)
5. I found the various functions in this system were well integrated: 3 (this tool consists of a series of notebooks and Python library to use in your own work. They have easily integrate-able models. However would replace your existing ML tools such as SciKit learn)
6. I thought there was too much inconsistency in this system:
7. I would imagine that most people would learn to use this system very quickly: 3 - A technical person would learn quickly; if not technical it would be struggle.
8. I found the system very cumbersome to use: 1 - Uses Docker \_media and no requirements for a GPU.
9. I felt very confident using the system: 2 - Can use out of the box with the Jupyter notebooks. Explain-abilities are worded in a confusing manner - a lot of negation, such as `not quite good`
10. I needed to learn a lot of things before I could get going with this system: 1 (If you’re familiar with Machine Learning models, there are some key models here to use)

**Description of the tool**

This is a series of Jupyter notebooks, that illustrate the use of the h2o library for Python.[ h2o](https://www.h2o.ai/) is a company which provides a series of tools and platforms as both OS and Commercialized software for enterprise adoption, in order to Democratize AI.

This particular repository is an example of h2o’s OS offering, that focuses on AI and Explainability.

**What is its purpose?**

- To show adaptations of existing Machine Learning methods allow for explainability
- Directs usage of it’s Python h2o library in Explainable AI.

**Who is the intended user?**

- Developer audience: familiarity with Python
- Interest in Ethical Machine Leaning and to show it’s positioning as a company and community within this area.

**What is its scope (algorithms, data, types of challenges)?**

- Decision Trees, Lime, Loco, XGBoost, PDP Ice, Sensitivity Analysis

**Best for: **

**What should practitioners use this tool for? **

- Trialling out datasets on the available machine learning models

**Are there any scenarios / use cases in which this tool is particularly helpful vs. useless?**

- Machine learnings models that are not included. This cannot be used as a replacement for other more thorough ML libraries such as Tensorflow, SciKit Learn.
- The set appears to not be able to use it in productioni-zed machine learning. It gives no direction on the data set volume and velocity, links to deployment cases or otherwise.

**Pros & cons**

**What are the benefits of this tool?**

- Can be used as a preliminary tool to explain a model. Shows explanations in a natural language format and indicates way to to improve the model

**What are the challenges in using this tool? **

- Need to investigate fully scalability
- Need to see use on real data sets - examples feel out of the box

**Limitations, especially any technical issues**

E.g. difficult to integrate or customize

**Case study demo with screenshots**

Image 1. Shows Jupyter notebook for Sensitivity Analysis

Image 2. Shows Jupyter notebook for Partial Dependency and ICE plot

Image 3. Shows h2o site and mission statement.

![alt_text](../_media/image22.png "image_tooltip")

![alt_text](../_media/image23.png "image_tooltip")

![alt_text](../_media/image24.png "image_tooltip")
