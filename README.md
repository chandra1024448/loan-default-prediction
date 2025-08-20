# Loan Default Prediction App 🚀

This project predicts whether a loan applicant is likely to default or not, using machine learning models.  
Multiple algorithms were tested (Logistic Regression, Random Forest, XGBoost), and *XGBoost* was chosen as the final model for deployment due to its superior performance.  

## 🔗 Demo
- Streamlit App - https://huggingface.co/spaces/chandra1024/Loan-Default-Prediction

---

## 📌 Features
- Exploratory Data Analysis (EDA) on loan dataset  
- Model training using Logistic Regression, Random Forest, and XGBoost  
- Feature importance visualization  
- Interactive *Streamlit web app* for real-time loan default predictions  

---

## 🛠️ Tech Stack
- *Programming Language*: Python  
- *Libraries*: Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn  
- *Deployment*: Streamlit 
- *Model Persistence*: Pickle  

---

## 📂 Project Workflow
1. Data preprocessing (missing values, encoding categorical features, scaling numeric values)  
2. Model training & evaluation on multiple algorithms  
3. Model selection → XGBoost chosen as final model  
4. Saving trained model & encoders using Pickle  
5. Deployment via Streamlit (UI) 

---

## ⚙️ Installation & Usage
Clone this repository and install dependencies:

---

## **Run Streamlit App**
streamlit run app.py

---

## 📊**Result & Insights**

🔹 Model Performance (Default Threshold = 0.5)
	•	Accuracy: ~72%
	•	Precision (Defaulters = 1): 0.23
	•	Recall (Defaulters = 1): 0.62
	•	F1-Score (Defaulters = 1): 0.34

➡️ The model captures many defaulters (high recall) but also produces a high number of false positives (low precision).

⸻

🔹 After Threshold Optimization (Best = 0.65)
	•	Accuracy: ~83%
	•	Precision (Defaulters = 1): 0.31
	•	Recall (Defaulters = 1): 0.41
	•	F1-Score (Defaulters = 1): 0.36

➡️ Increasing the threshold improves accuracy and balances precision/recall better.

➡️ False positives reduce, while still catching a reasonable portion of defaulters.

---

**🔹 Key Insights**

	•	XGBoost outperformed Logistic Regression & Random Forest.
	•	Threshold tuning significantly improved results for the minority class (defaulters).
	•	Limitations:
	•	Precision and recall for defaulters remain relatively low due to dataset imbalance.
	•	Model may miss some defaulters, which can be costly in real banking scenarios.
	•	Future focus: handling imbalance (SMOTE, class weights), cost-sensitive learning, and advanced models.

**✨ Verdict:**
This is a strong baseline model (83% accuracy with threshold tuning).
Further improvements are needed for production-level deployment in financial institutions.

⸻

**🚀 Future Improvements**
	•	Apply SMOTE / class weighting for better handling of imbalance
	•	Perform advanced hyperparameter tuning (GridSearchCV / RandomizedSearchCV)
	•	Deploy with Docker / Cloud (AWS, GCP, Azure)
	•	Add monitoring for model drift in production
	•	Explore ensemble stacking or deep learning methods

⸻

**📸 Screenshots**

<img width="1896" height="861" alt="image" src="https://github.com/user-attachments/assets/6f1e3f10-f7c9-426d-b598-00ec5280b6f7" />

⸻

**🤝 Contributing**

Contributions, issues, and feature requests are welcome!
Feel free to fork this repo and submit a pull request.

⸻

**📜 License**

This project is licensed under the MIT License – see the LICENSE file for details.

⸻

**🙋‍♀️ About Me**

Hi, I’m Chandrakala Somanath Chippa 👋

	•	🎓 PGP in AIML from Austin University, Texas
 
	•	💼 7+ years experience in Finance (TCS, Gallagher, Propark Mobility)
 
	•	🤖 Passionate about AI/ML, Data Science & Model Deployment
 
	•	🌐 [(https://www.linkedin.com/in/chandrakala-chippa-402529280/?trk=PROFILE_DROP_DOWN] |
 			[https://github.com/chandra1024448/loan-default-prediction/edit/main]

```bash
# Clone repo
git clone - https://github.com/chandra1024448/loan-default-prediction/new/main
cd loan-default-prediction

# Install dependencies
pip install -r requirements.txt

---



