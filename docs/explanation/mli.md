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

**Best for:**

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
