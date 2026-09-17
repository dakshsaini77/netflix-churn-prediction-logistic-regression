# Netflix Churn Prediction Using Logistic Regression

## 📌 Project Overview

This project demonstrates how **Machine Learning** can be used to predict whether a Netflix subscriber is likely to **churn (cancel their subscription)**.

The project uses **Logistic Regression**, a simple and explainable classification model. It is suitable for learning because each feature has a clear model coefficient that helps explain its relationship with churn.

> **Note:** Netflix's real subscriber data is private. This practical uses a realistic **synthetic dataset** created for classroom learning.

## 🎯 Objectives

The project helps students understand:

* How Machine Learning can predict customer churn
* How subscriber data can be prepared for a model
* How Logistic Regression works for classification
* How to split data into training and testing sets
* How to evaluate model accuracy
* How to interpret model coefficients
* How AI/ML predictions can support business decisions

## 🧠 Machine Learning Model

### Logistic Regression

Logistic Regression is used to classify subscribers into two categories:

* `0` → Stayed
* `1` → Churned

The model learns patterns from subscriber information and predicts the probability that a subscriber will churn.

## 📊 Features Used

The model uses the following subscriber features:

| Feature              | Description                                 |
| -------------------- | ------------------------------------------- |
| `tenure_months`      | How long the subscriber has been subscribed |
| `weekly_watch_hours` | Average hours watched per week              |
| `logins_per_month`   | Number of app logins per month              |
| `support_tickets`    | Support tickets in the last 90 days         |
| `payment_failures`   | Failed payments in the last 90 days         |
| `plan_tier`          | Basic, Standard, or Premium                 |
| `churn`              | Target variable: Stayed or Churned          |

## 🔄 Project Workflow

```text
Create Dataset
      ↓
Explore Data
      ↓
Prepare Features
      ↓
Encode Plan Tier
      ↓
Split Training & Testing Data
      ↓
Scale Features
      ↓
Train Logistic Regression
      ↓
Make Predictions
      ↓
Evaluate Model
      ↓
Interpret Results
      ↓
Predict Churn for a Subscriber
```

## 🛠️ Technologies Used

* Python
* Google Colab
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Logistic Regression

## 📈 Model Evaluation

The notebook evaluates the model using:

* Accuracy
* Classification Report
* Confusion Matrix

These measures help understand how well the model distinguishes between subscribers who stay and subscribers who churn.

## 🔍 Feature Interpretation

One useful part of Logistic Regression is that each feature receives a **coefficient (weight)**.

In this classroom dataset:

* Positive weights push the prediction toward higher churn risk.
* Negative weights push the prediction toward lower churn risk.

The notebook is designed to examine factors such as:

* Payment failures
* Watch hours
* App logins
* Subscription tenure
* Plan tier

## 💼 Business Application

A streaming company could use a churn prediction system to identify subscribers who may be at higher risk of cancellation.

For example:

```text
Subscriber Data
      ↓
Churn Prediction Model
      ↓
High-Risk Subscriber
      ↓
Retention Team
      ↓
Possible Retention Action
```

Possible business actions could include:

* Discount offers
* Free upgrade periods
* Proactive customer support
* Personalized engagement campaigns

The model provides **decision support**; business teams should consider additional context before taking action.

## ⚠️ Important Limitation

This project uses **synthetic data created for a classroom exercise**, not real Netflix subscriber data.

A real-world deployment would require:

* Actual customer data
* Data privacy controls
* Appropriate governance
* Careful model validation
* Monitoring of prediction quality
* Human review of business actions

Therefore, the results of this notebook should not be treated as actual Netflix churn statistics.

## 📁 Repository Structure

```text
netflix-churn-prediction-logistic-regression/
│
├── README.md
│
├── netflix_churn_logistic_regression.ipynb
│
└── screenshots/
    └── model-results.png
```

## 🚀 How to Run

1. Open the `.ipynb` notebook in **Google Colab**.
2. Run the cells from top to bottom.
3. Allow the synthetic dataset to be created.
4. Train the Logistic Regression model.
5. Review the accuracy and confusion matrix.
6. Examine the feature weights.
7. Try different subscriber information using the prediction function.

## 🎓 Learning Outcome

This practical demonstrates how an AI/ML model can transform customer information into a **churn prediction** that can support customer-retention activities.

### Key Concept

**Customer Data → Machine Learning Model → Churn Probability → Business Action**

## 👨‍🎓 Course Context

This project is designed as a practical learning exercise for **BBA AI/ML students** and focuses on understanding the business meaning of Machine Learning rather than memorizing Python code.
