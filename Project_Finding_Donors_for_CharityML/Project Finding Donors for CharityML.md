# Project: Finding Donors for CharityML

## Description

CharityML is a fictitious charity organization located in the heart of Silicon Valley that was established to provide financial support for people eager to learn machine learning. After nearly 32,000 letters were sent to people in the community, CharityML determined that every donation they received came from someone that was making more than $50,000 annually. To expand their potential donor base, CharityML has decided to send letters to residents of California, but to only those most likely to donate to the charity. With nearly *15 million* working Californians, CharityML has brought you on board to help build an algorithm to best identify potential donors and reduce overhead cost of sending mail. Your goal will be evaluate and optimize several different supervised learners to determine which algorithm will provide the highest donation yield while also reducing the total number of letters being sent.

<br>

## Highlights

This project is designed to get acquainted with the many supervised learning algorithms available in sklearn, and to also provide for a method of evaluating just how each model works and performs on a certain type of data. It is important in machine learning to understand exactly when and where a certain algorithm should be used, and when one should be avoided.

The learning outcomes are:

- How to identify when preprocessing is needed, and how to apply it.
- How to establish a benchmark for a solution to the problem.
- What each of several supervised learning algorithms accomplishes given a specific dataset.
- How to investigate whether a candidate solution model is adequate for the problem.

<br>

## Files

 [Data Scientist GitHub](https://github.com/udacity/DSND_Term1)

- `finding_donors.ipynb`: This is the main file where you will be performing your work on the project.
- `census.csv`: The project dataset. You'll load this data in the notebook.
- `visuals.py`: This Python script provides supplementary visualizations for the project. Do not modify.

<br>


## Dataset

The modified census dataset consists of approximately 32,000 data points, with each datapoint having 13 features. This dataset is a modified version of the dataset published in the paper *"Scaling Up the Accuracy of Naive-Bayes Classifiers: a Decision-Tree Hybrid",* by Ron Kohavi. You may find this paper [online](https://www.aaai.org/Papers/KDD/1996/KDD96-033.pdf), with the original dataset hosted on [UCI](https://archive.ics.uci.edu/ml/datasets/Census+Income).

**Features**

- `age`: Age
- `workclass`: Working Class (Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, Local-gov, State-gov, Without-pay, Never-worked)
- `education_level`: Level of Education (Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool)
- `education-num`: Number of educational years completed
- `marital-status`: Marital status (Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse)
- `occupation`: Work Occupation (Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty, Handlers-cleaners, Machine-op-inspct, Adm-clerical, Farming-fishing, Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces)
- `relationship`: Relationship Status (Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried)
- `race`: Race (White, Asian-Pac-Islander, Amer-Indian-Eskimo, Other, Black)
- `sex`: Sex (Female, Male)
- `capital-gain`: Monetary Capital Gains
- `capital-loss`: Monetary Capital Losses
- `hours-per-week`: Average Hours Per Week Worked
- `native-country`: Native Country (United-States, Cambodia, England, Puerto-Rico, Canada, Germany, Outlying-US(Guam-USVI-etc), India, Japan, Greece, South, China, Cuba, Iran, Honduras, Philippines, Italy, Poland, Jamaica, Vietnam, Mexico, Portugal, Ireland, France, Dominican-Republic, Laos, Ecuador, Taiwan, Haiti, Columbia, Hungary, Guatemala, Nicaragua, Scotland, Thailand, Yugoslavia, El-Salvador, Trinadad&Tobago, Peru, Hong, Holand-Netherlands)

**Target Variable**

- `income`: Income Class (<=50K, >50K)

<br>

## Software and Libraries

- Python
- NumPy
- pandas
- scikit-learn
- Matplotlib

<br>


## Meeting Specifications

**Exploring the Data**

| CRITERIA         | MEETS SPECIFICATIONS                                         |
| ---------------- | ------------------------------------------------------------ |
| Data Exploration | Student's implementation correctly calculates the following: <br />Number of records<br />Number of individuals with income >$50,000, <br />Number of individuals with income <=$50,000, <br />Percentage of individuals with income > $50,000 |

**Preparing the Data**

| CRITERIA           | MEETS SPECIFICATIONS                                         |
| ------------------ | ------------------------------------------------------------ |
| Data Preprocessing | Student correctly implements one-hot encoding for the feature and income data. |

**Evaluating Model Performance**

| CRITERIA                                    | MEETS SPECIFICATIONS                                         |
| ------------------------------------------- | ------------------------------------------------------------ |
| **Question 1:** Naive Predictor Performance | Student correctly calculates the benchmark score of the naive predictor for both accuracy and F1 scores. |
| **Question 2:** Model Application           | The pros and cons or application for each model is provided with reasonable justification why each model was chosen to be explored.Please list all the references you use while listing out your pros and cons. |
| Creating a Training and Predicting Pipeline | Student successfully implements a pipeline in code that will train and predict on the supervised learning algorithm given. |
| Initial Model Evaluation                    | Student correctly implements three supervised learning models and produces a performance visualization. |

**Improving Results**

| CRITERIA                                               | MEETS SPECIFICATIONS                                         |
| ------------------------------------------------------ | ------------------------------------------------------------ |
| **Question 3:** Choosing the Best Model                | Justification is provided for which model appears to be the best to use given computational cost, model performance, and the characteristics of the data. |
| **Question 4:** Describing the Model in Layman's Terms | Student is able to clearly and concisely describe how the optimal model works in layman's terms to someone who is not familiar with machine learning nor has a technical background. |
| Model Tuning                                           | The final model chosen is correctly tuned using grid search with at least one parameter using at least three settings. If the model does not need any parameter tuning it is explicitly stated with reasonable justification. |
| **Question 5:** Final Model Evaluation                 | Student reports the accuracy and F1 score of the optimized, unoptimized, models correctly in the table provided. Student compares the final model results to previous results obtained. |

**Feature Importance**

| CRITERIA                                       | MEETS SPECIFICATIONS                                         |
| ---------------------------------------------- | ------------------------------------------------------------ |
| **Question 6:** Feature Relevance Observation  | Student ranks five features which they believe to be the most relevant for predicting an individual's’ income. Discussion is provided for why these features were chosen. |
| **Question 7:** Extracting Feature Importances | Student correctly implements a supervised learning model that makes use of the `feature_importances_` attribute. Additionally, student discusses the differences or similarities between the features they considered relevant and the reported relevant features. |
| **Question 8:** Effects of Feature Selection   | Student analyzes the final model's performance when only the top 5 features are used and compares this performance to the optimized model from **Question 5**. |

<br>

------

*Last update: 5 September 2019*