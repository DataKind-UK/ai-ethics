# [Google Explainable AI](https://cloud.google.com/explainable-ai)

**Overall evaluation**

_User-friendliness (system usability scale)_

Answer with strongly agree (5), agree (4), neutral (3), disagree (2), strongly disagree (1)

Feel free to add comments and justifications!

1. I think that I would like to use this system frequently: 3
2. I found the system unnecessarily complex: 2
3. I thought the system was easy to use: 4
4. I think that I would need the support of a technical person to be able to use this system: 1
5. I found the various functions in this system were well integrated: 3
6. I thought there was too much inconsistency in this system: 2
7. I would imagine that most people would learn to use this system very quickly: 4
8. I found the system very cumbersome to use: 2
9. I felt very confident using the system: 3
10. I needed to learn a lot of things before I could get going with this system: 2

**Description of the tool**

What is its purpose?

Google is aiming to make explaining models a natural endpoint of any model deployment. So when a prediction is inferred, the explanation is automatically returned. This includes state of the art XAI frameworks such as SHAP and Integrated Gradient methods. In addition, Google’s There are two options for how a model can be created with the platform:

  *   AutoML - you give Google tabular data and it will choose the machine learning model and hyperparameters based on a performance metric
  *   Explainable AI Platform - create your own tensorflow model

For both of these methods, Google will choose the appropriate XAI framework that is used, so the user is abstracted from which XAI to use and which parameters to apply. The purpose of the platform is therefore not just for XAI, but to create a scalable and production-ready end-to-end machine learning pipeline from tagging, to model building, deployment, inference, and evaluation.

Who is the intended user?

- Data Scientists and Data Engineers
- Technical expertise is required in order to use this. Although there are some user interfaces, they have to be produced by code then can be used by a non-technical user.

What is its scope (algorithms, data, types of challenges)?

- Tabular and image data applied to tensorflow models
- Data has to be structured in some way, either tabular or image
- Algorithms are limited to AutoML and tensorflow v1.X. Any XAI algorithms are abstracted from the user.

**Best for**

What should practitioners use this tool for?

- Productionising explanations as part of a MLOps deployment pipeline
- Easy explanations for structured data models where no XAI knowledge is known

Are there any scenarios / use cases in which this tool is particularly helpful vs. useless?

- If GCP is already used, it is a very easy addition to pipelines
- Can link to other GCP services such as AutoML easily
- For technical people who have no idea about XAI, this can give some valuable insight

**Pros & cons**

What are the benefits of this tool? ì

- Pro: Automated deployment means infrastructure management is easy
- Pro: GCP advises on the XAI based on the datatype
- Con: Flexibility limited compared to use source packages directly
- Con: Cloud-based lock-in
- Con: Data will need to be uploaded to the cloud

What are the challenges in using this tool?

- Some GCP knowledge is required
- Abstraction means easy use, but more limited flexibility

**Case study demo with screenshots**

Guessing the duration of London bike hire

![alt_text](../_media/image27.png "image_tooltip")

Create tensorflow model, deploy on a GCP instance, and expose API

![alt_text](../_media/image28.png "image_tooltip")

Query the model by creating an API request on a test datapoint

![alt_text](../_media/image29.png "image_tooltip")

The response contains feature attribute information. This is automatically selected based on the model given: here it is an integrated gradients XAI method. The attribution value is the outcome from the XAI, where it shows the impact the feature has had on the regression output. For example, the most significant feature is ‘euclidean’, which has a positive effect on the regression.

![alt_text](../_media/image30.png "image_tooltip")

Google’s What-If service can be easily used. Here a datapoint can be selected then the feature inputs changed. The model is queried with the new datapoint and the delta from the original is recorded.

![alt_text](../_media/image31.png "image_tooltip")

\_media can also be used. This overlays the feature attribution onto the image so the areas of the image that were of importance to deciding the classification are displayed. Below, we can see a good model as the important pixels of the animals are the animals themselves. If the important pixels were the background, the model would be basing its decision on features not to do with the animal and would therefore be poor.

![alt_text](../_media/image32.png "image_tooltip")
