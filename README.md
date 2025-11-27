<h1> CKD Predicting Model</h1>
<b>Project Title: </b> Prediction of Chronic Kidney Disease Using Machine Learning
<h2>1. Project Summary</h2>
<p>  &nbsp;&nbsp;&nbsp;&nbsp;This project focuses on developing a machine learning model to predict Chronic Kidney Disease (CKD) based on patient clinical data. The goal is to identify high-risk patients early, enabling timely interventions. The model was trained on the dataset provided and evaluated using industry-standard metrics to ensure reliable predictions.
</p>
<h2>2. Problem Statement</h2>
<p>  &nbsp;&nbsp;&nbsp;&nbsp;The objective is to build a predictive model that classifies patients as CKD or Non-CKD based on clinical features such as blood pressure, blood sugar, serum creatinine, and more.</p>

<b>Type of Problem: </b>Supervised Classification
<h2>3. Dataset Overview</h2>
<ol>
  
  • Number of Records:400

  • Number of Features:38

  • Target Variable: class (CKD / Non-CKD)

  • Feature Types: Numerical and Categorical

  • Observations:
<ol>

  • Missing values present in some features

  • No duplicate records detected
</ol>
</ol>

<h2>4. Data Processing</h2>
<ol>

   • Missing values handled using mean/median imputation

   • Categorical variables encoded using Label Encoding / One-Hot Encoding

   • Features scaled where necessary

   • Train-Test Split: 80% train, 20% test

</ol>

<h2>5. Exploratory Data Analysis (EDA)</h2>

<ol>

   • Correlation analysis to identify important features

   • Histograms for numeric features 

   • Bar plots for categorical variables 

   • Heatmap to visualize correlations
   
</ol>
<h2>6. Feature Selection</h2>
<ol>

    • Features selected based on correlation and importance from tree-based models

    • Removed redundant or low-impact features to improve model performance
</ol>

<h2>7. Model Building and Evaluation</h2>
<b>Algorithms Tried:
</b>
<ol>

    • Logistic Regression

    • Random Forest Classifier

    • XGBoost Classifier

    • Support Vector Machine
</ol>
<b>Evaluation Metrics:</b>
<ol>

    • Accuracy

    • Precision

    • Recall

    • F1-Score

    • ROC-AUC
</ol>
<b>Performance Summary</b>

<html>
<body>
  <table>
    <tr>
      <th>Model</th>
      <th>Accuracy</th>
      <th>Precision</th>
      <th>Recall</th>
      <th>F1-Score</th>
      <th>ROC-AUC</th>
    </tr>
    <tr>
      <td>Logistic Regression</td>
      <td>0.85</td>
      <td>0.83</td>
      <td>0.87</td>
      <td>0.85</td>
      <td>0.88</td>
    </tr>
    <tr>
      <td>Random Forest</td>
      <td>0.92</td>
      <td>0.91</td>
      <td>0.93</td>
      <td>0.92</td>
      <td>0.95</td>
    </tr>
    <tr>
      <td>XGBoost</td>
      <td>0.91</td>
      <td>0.90</td>
      <td>0.92</td>
      <td>0.91</td>
      <td>0.94</td>
    </tr>
  </table>
</body>
</html>
<b>Best Model: </b> Random Forest Classifier – highest accuracy and balanced precision/recall.
<h2>8. Conclusion and Recommendations</h2>
<ol>
  
    • The Random Forest model can reliably predict CKD with 92% accuracy.

    • Early detection using this model can assist healthcare providers in preventive care.

<b>Limitations:</b> Small dataset, some missing values, limited features.

<b>Next Steps:</b>

<ol>

     • Increase dataset size

     • Fine-tune hyperparameters for better performance

     • Consider deployment via a user-friendly interface for real-time predictions
</ol>
