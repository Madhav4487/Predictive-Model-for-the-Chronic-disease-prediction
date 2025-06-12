## 🩺 Project Overview: Chronic Disease Prediction using HINTS Survey Data

This project focuses on predicting the presence of chronic diseases based on self-reported behavioral, demographic, and health information from the Health Information National Trends Survey (**HINTS**) datasets. The study evaluates the predictive power of various features using multiple imputation techniques and machine learning models, with a focus on identifying key contributing factors.

---

### 📊 Dataset

- **Source**: [National Cancer Institute - HINTS](https://hints.cancer.gov)
- **Cycles Used**: HINTS 6, HINTS 5 Cycle 4, and HINTS 5 Cycle 3
- **Data Preparation**:
  - Appended data across the three survey cycles
  - Removed duplicates and survey weighting variables
  - Selected features across multiple survey sections:
    - Demographic
    - Digital Health Literacy
    - Physical Activity and Exercise
    - Tobacco Use
    - Health Information Seeking

---

### 🧼 Handling Missing Data

Applied and compared four different imputation strategies:
1. **Single Imputation (-1 as placeholder)**
2. **Multiple Imputation by Chained Equations (MICE)**
3. **K-Nearest Neighbors (KNN) Imputation**
4. **SoftImpute (Matrix Completion)**

---

### 🤖 Modeling Approach

Used a variety of machine learning models to predict the likelihood of chronic disease:
- Logistic Regression
- Random Forest
- Support Vector Machine (SVM)
- Gradient Boosting
- Deep Learning (Feedforward Neural Network)

**Evaluation Metric**: Precision-Recall AUC (PR_AUC)  
**Model Selection**: The best-performing model was selected based on the highest PR_AUC score.

---

### 📌 Feature Importance

- SHAP (SHapley Additive exPlanations) values were used to interpret the most influential features from the best model.
- **Top Contributing Factors** (in order of importance):
  1. **Demographic variables** (e.g., age, income, education)
  2. **Health information seeking behavior**
  3. **Digital health literacy** (e.g., internet usage for health)
  4. **Physical activity and exercise**
  5. **Tobacco use**

---

### 🔮 Future Work

- Include additional HINTS cycles for expanded analysis
- Evaluate time-based prediction models for disease onset
- Apply causal inference methods to assess risk factor impact
- Build interactive dashboards to visualize risk factors
- Compare more advanced imputation techniques (e.g., Variational Autoencoders)



## 📬 Contact

**Madhav Dahal**  
📧 madhavdahal16@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/madhav-dahal-ms-9a1147b0)  
🔗 [GitHub](https://github.com/Madhav4487)
