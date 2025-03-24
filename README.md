# WiDS_2025
# GitHub Kaggle Project README
# WiDS_Team_Dendrites
---

### **👥 Team Members**

| Name | GitHub Handle | Contribution |
| ----- | ----- | ----- |
| Ruth Velasquez | [@Abillama05](https://github.com/abillama05) | Built CNN model, performed data cleaning, minor feature engineering |
| Frantzia Theodat | @FranTheo | Exploratory data analysis |
| Marzana Afroz | @marzanaafroz | Explored and interpreted the data to guide model selection; researched multi-output TensorFlow CNN approaches |
| Christiana Nardi | @cbekk | Built multi-output regression model, performed data cleaning and analysis, and parameter tuning |

---

## **🎯 Project Highlights**

* Built a PyTorch Convoluted Nueral Network using an Multi Output Model to solve a binary classification of fMRI FCM, categorical, and quantitative data.
* Achieved an F1 score of \[insert score\] and a ranking of \[insert ranking out of participating teams\] on the final Kaggle Leaderboard
* Used \[explainability tool\] to interpret model decisions
* Implemented \[data preprocessing method\] to optimize results within compute constraints

🔗 [WiDS Datathon 2025 | Kaggle Competition Page](https://www.kaggle.com/competitions/widsdatathon2025/overview)

---

## **👩🏽‍💻 Setup & Execution**

**Provide step-by-step instructions so someone else can run your code and reproduce your results. Depending on your setup, include:**

* How to clone the repository
* How to install dependencies
* How to set up the environment
* How to access the dataset(s)
* How to run the notebook or scripts

---

## **🏗️ Project Overview**

This project was developed for the WiDS Datathon 2025, hosted on Kaggle and supported by the Break Through Tech AI Program. Our team, WiDS_Team_Dendrites, collaborated to tackle the challenge of predicting ADHD diagnoses using a combination of functional MRI-derived Functional Connectome Matrices (FCMs) and accompanying categorical and quantitative features.

The dataset required extensive exploration to understand brain connectivity patterns and their relationship to ADHD. FCMs, which represent the functional connectivity between different brain regions, had to be normalized and resized for modeling—particularly when working with deep learning models like CNNs.

Our initial focus was on understanding the dataset structure, identifying preprocessing requirements, and researching suitable multi-output model architectures. We explored various modeling strategies—including TensorFlow-based CNNs and PyTorch multi-output models—to handle the multi-label classification task efficiently within compute constraints.

This work not only enhanced our technical understanding of neuroimaging and deep learning but also holds real-world significance by contributing to research in ADHD diagnosis and mental health analytics through AI-driven approaches.

---

## **📊 Data Exploration**

**Describe:**

* The datasets used were from the WiDS 2025 Kaggle competition.
* Data exploration and preprocessing approaches
  
      1. Fill Null values with a range of random values between the mean and standard deviation.
      2. Fill Null values in test data with -1 since creating a new value could mess with predictions
      3. Remove highly correlated features
      4. Convert fMRI FCM into graph objects
* Challenges and assumptions when working with the dataset(s)
  
      1. Working with fMRI as Functional Connectome Matrices was new for us
      2. Assumed at first that the training solutions would have no null values but there were a few instances which affected out first model's accuracy


### Data Preprocessing Visualizations: 
<table>
  <tr>
    <th>"Track_Age_At_Scan" before imputation</th>
    <th>"Track_Age_At_Scan" after imputation</th>
  </tr>
  <tr>
    <td><img src="https://github.com/VIR-WiDS-Team-Dendrites/WiDS_2025/blob/cd4e83c8c259a12ea55aa27a92a6534e4ff838c2/Images/b4_impute.png" width="350px"></td>
    <td><img src="https://github.com/VIR-WiDS-Team-Dendrites/WiDS_2025/blob/cd4e83c8c259a12ea55aa27a92a6534e4ff838c2/Images/after_impute.png" width="350px"></td>
  </tr>
  <tr>
    <th>Correlation Matrix to find most correlated features</th>
  </tr>
  <tr>
    <td><img src="https://github.com/VIR-WiDS-Team-Dendrites/WiDS_2025/blob/1632d2f5f3eb376257e7824454d8a39afcbe1a58/Images/corr_features.png" width="350px"></td>
  </tr>
</table>

---

## **🧠 Model Development**

**Describe (as applicable):**

* Model(s) used (e.g., CNN with transfer learning, regression models)
* Feature selection and Hyperparameter tuning strategies
* Training setup (e.g., % of data for training/validation, evaluation metric, baseline performance)

---

## **📈 Results & Key Findings**

**Describe (as applicable):**

* Performance metrics (e.g., Kaggle Leaderboard score, F1-score)
* How your model performed overall
* How your model performed across different skin tones (AJL)
* Insights from evaluating model fairness (AJL)

**Potential visualizations to include:**

* Confusion matrix, precision-recall curve, feature importance plot, prediction distribution, outputs from fairness or explainability tools

---

## **🖼️ Impact Narrative**

**Answer the relevant questions below based on your competition:**

**WiDS challenge:**

1. What brain activity patterns are associated with ADHD; are they different between males and females, and, if so, how?
2. How could your work help contribute to ADHD research and/or clinical care?

---

## **🚀 Next Steps & Future Improvements**

**Address the following:**

* What are some of the limitations of your model?
* What would you do differently with more time/resources?
* What additional datasets or techniques would you explore?

---

## **📄 References & Additional Resources**

* Cite any relevant papers, articles, or tools used in your project

---

