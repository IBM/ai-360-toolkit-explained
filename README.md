# AI 360 Toolkit Series- AI Models Explained

### Introduction:
The capabilities of AI are not hidden. Intelligence of machines is undergoing major transformation by continuous self-learning improvements. However, these AI models are still a black-box and are often questioned for their decisions by the clients. Research is faster than ever on improving and optimisation of the algorithms, but this alone won’t suffice. The conversations around building trust on AI is often a point of interest with the client for developers advocates, Sales and Marketing team which stand at the frontline with them. Hence, it becomes the important aspect to look into. Imagine owning a Computer Vision Company that deals with building AI Classification Models for Healthcare Industry to diagnose cancer using MRIs, CT scans, X-rays, etc which aids doctor in taking decisions. It is difficult for a doctor to rely on the diagnosis suggested by an AI model-a black box when a person’s life is involved.  Therefore, building Trusted AI Pipelines has become increasingly important with the sudden shoot of AI Applications. 

#### Building Trustworthy AI Pipelines stands on three Pillars:

* Fairness: Unfair biases can exist in the data used to train the model as well as in the model’s own decision-making algorithm. Fairness emphasis on Identification and tackling of such biases introduced in the data. This will ensure that a model’s predictions are fair and do not unethically discriminate. 

* Explainability: Explainability raises the curtain from behind the scenes of how an ML model makes its predictions. It gives an improved understanding of the model by clarifying the inner working of the model. It is essential to Data Scientists for detecting, avoiding, and removing its failure modes; to SMEs and Customers for earning public trust in the algorithm; and for introducing effective policies to regulate the technology.

* Robustness: Robustness measures the stability of the algorithm performance when model. deployed in real world is attacked and noise in introduced in the training data. It characterizes how effective your algorithm is while being tested on the new independent (but similar) dataset. This will ensure that the algorithm of the model is able to handle the unseen, perturbed data. It addresses the questions of estimating uncertainties in its predictions and whether or not the model is robust to. 


To build Trusted AI, IBM Research AI is developing [diverse approaches]( https://research.ibm.com/artificial-intelligence/trusted-ai/?_ga=2.53814376.134814594.1606471878-1093864575.1604559368) for how to achieve fairness, robustness, explainability, accountability, value alignment, and how to integrate them throughout the entire lifecycle of an AI application.

### Three-Open source Toolkits by IBM Research : 

1.	[AI Fairness 360]( http://aif360.mybluemix.net/) - This extensible open-source toolkit can help you examine, report, and mitigate discrimination and bias in machine learning models throughout the AI application lifecycle. Containing over 70 fairness metrics and 10 state-of-the-art bias mitigation algorithms developed by the research community, it is designed to translate algorithmic research from the lab into the actual practice of domains as wide-ranging as finance, human capital management, healthcare, and education.
2.	[AI Explainability 360](http://aix360.mybluemix.net) - This extensible open source toolkit can help you comprehend how machine learning models predict labels by various means throughout the AI application lifecycle. Containing eight state-of-the-art algorithms for interpretable machine learning as well as metrics for explainability, it is designed to translate algorithmic research from the lab into the actual practice of domains as wide-ranging as finance, human capital management, healthcare, and education.
3.	[Adversarial Robustness 360 Toolbox](https://developer.ibm.com/open/projects/adversarial-robustness-toolbox/) — The Adversarial Robustness Toolbox is designed to support researchers and developers in creating novel defense techniques, as well as in deploying practical defense of real-world AI systems. Researchers can use the Adversarial Robustness Toolbox to benchmark novel defense against the state-of-the-art. For developers, the library provides interfaces which support the composition of comprehensive defense systems using individual methods as building blocks.


### Architecture 


![](https://github.com/IBM/ai-360-toolkit-explained/blob/main/doc/src/images/AI-Article.png)
 

Flow:
1.	Log in to Watson Studio powered by spark, initiate Cloud Object Storage, and create a project.
2.	Upload the .csv data file to Object Storage.
3.	Load the Data File in Watson Studio Notebook.
4.	Install AI Explainability 360 Toolkit, Adversarial Robustness Toolbox, AI Fairness 360 in the Watson Studio Notebook.
5.	Visualization for explainability and interpretability of AI Model for the three different types of Users.

### About this Series:

The Series demonstrates the AI 360 toolkit in detail and how do we use this IBM toolkit to solve AI use-cases. How to build end to end AI model pipeline and make them transparent. How can we make the AI models explainable for the outcome and how do we ensure that AI models are not biased in their decision making. How do we build robust models which can predict with good accuracy on new datasets without retraining. This series will be for everyone who wants to understand the working of AI models and also make it explainable to the layman. This series will have wider applicability across multiple domains.

- [AI 360 toolkit - How do we identify & remove bias from AI models
](https://github.ibm.com/IBMCode/IBMCodeContent/issues/5283): The First Code Pattern in the series demonstrates how to use AI Fairness 360 toolkit from IBM to identify & mitigate bias in the AI models. This approach will help the business to take fair decisions on different aspects. We will be using the Fraud Prediction dataset to demonstrate how the accuracy of AI models are impacted with the bias in the dataset and how this toolkit helps in removing the bias on the fly to ensure the decision making is not impacted. This approach of building AI models without bias has wider applicability for the developers and can be used to solve multitude of use cases under different domains.


 - [Unveiling Machine's Fraud Prediction Decision with AI Explainability 360](https://github.ibm.com/IBMCode/IBMCodeContent/issues/5285): The Second Code Pattern highlights the use of the AI explainability 360 toolkits to demystify the decisions taken by the machine learning model to gain better insights and explainability which not only help the policy-makers, data scientists to develop trusted explainable AI applications but also the general public for transparency. To demonstrate the use of the AI Explainability 360 Toolkit, we are using the existing Fraud Detection Code Pattern showcasing, explaining the AIX360 Algorithms, and also guide the practitioner on choosing an appropriate explanation method or algorithm depending upon the type of customer(Data Scientist, General Public, SME, Policy Maker) that needs an explanation of the model.  This Code Pattern will also demonstrate the use of ART(Adversarial Robustness 360 Toolkit) to defend and evaluate Machine Learning models and applications against the adversarial threats of Evasion, Poisoning, Extraction, and Inference. The Code Pattern contains a self-explanatory notebook illustrates following algorithms from the kit:- 
 
#### 1) Protodash Explainer
`Highlights the profile of similar instances classified 'no fraud risk' to the loan office.`

#### 2) Contrastive Explanations Method (CEM) algorithm using AI Explainability 360 on Fraud Data
`This step explains the significant factors influencing the favorable outcome which is to be classified as No-Fraud-risk.`

#### 3) Unveiling Fraud Detection AI Model for Data Scientist using Boolean Rule Column Generation explainer
`The results shows the rules using decision trees which are identified by the model to a data Scientist or ML engineer.`

### 4) Adversarial-Robustness-Toolbox for LightGBM. 
`This notebook show how to generates the adversarial training data using Adversarial-Robustness-Toolbox. This will prepare the model against adversarial attacks so it doesn't misclassify and is able to distinguish noise from the real data. This step shows how robust the model is for making predictions using new data`


**[Demonstrate fairness, explainability & robustness in a single notebook](https://github.ibm.com/IBMCode/IBMCodeContent/issues/5284):** The final code pattern demonstrates how to use AI 360 toolkit for creating an end to end pipeline for AI models by demonstrating fairness, eliminate bias, make the models explainable & showcase the robustness of the models. We will take a binary classification usecase to demonstrate all these features of AI 360 toolkit which will help the production deployed models to seamlessly work without any issues. This series will help the stakeholders, developers to understand the AI model life cycle completely and can take informed decisions. The black box of AI models will be made transparent, bias free, robust & explainable to the end users. This Code Pattern will be very helpful for developers, ML engineers to explore the open sourced IBM AI 360 toolkit on IBM platform to solve multiple usecases under different domains.

### Related Links

* [Bias mitigation of AI models](https://github.com/IBM/bias-mitigation-of-machine-learning-models-using-aif360)
* [Make AI models explainable](https://github.com/IBM/unveiling-machine-fraud-prediction-decision-with-ai-explainability-360)
* [Explore fairness, explainability & robustness on AI models](https://github.com/IBM/predict-an-event-with-fairness-explainability-robustness-using-ai-360-toolkit)
