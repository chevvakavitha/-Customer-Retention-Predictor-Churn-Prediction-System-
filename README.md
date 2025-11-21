# Customer-Retention-Predictor-Churn-Prediction-System
<!-- Banner -->
<p align="center">
  <img src="assets/churn_banner.png" alt="Customer Retention – Churn Prediction System Banner" style="width:100%; max-width:1600px; height:auto; border-radius:6px;" />
</p>

<h1 align="center">📊 Customer Retention Predictor – Churn Prediction System</h1>
<p align="center"><strong>Machine Learning system that predicts customer churn and identifies high-risk customers with actionable insights.</strong></p>

<hr/>

<h2 id="overview">📌 Overview</h2>
<p>
The <strong>Customer Retention Predictor (Churn Prediction System)</strong> is a complete end-to-end project for identifying customers highly likely to churn.  
Businesses lose significant revenue when customers leave unexpectedly—this system helps detect early signals using ML, allowing companies to take proactive retention steps.
</p>

<p>This repository includes data preprocessing, EDA, model training, evaluation, explainability, and optional API/UI integration.</p>

<hr/>

<h2 id="problem">🎯 Problem Statement</h2>
<p>
Customer churn is one of the biggest challenges for subscription-based and service-oriented businesses.  
Companies need a <strong>data-driven approach</strong> to:
</p>
<ul>
  <li>Identify customers likely to leave</li>
  <li>Understand WHY they may churn</li>
  <li>Take targeted retention actions</li>
</ul>

<p>
This churn prediction system solves that using <strong>ML models + explainability tools (SHAP)</strong>.
</p>

<hr/>

<h2 id="features">✨ Key Features</h2>
<ul>
  <li><strong>Binary classification</strong> to identify churn risk</li>
  <li><strong>Full preprocessing pipeline</strong> (cleaning, encoding, scaling)</li>
  <li><strong>Multiple ML models</strong> (Logistic Regression, Random Forest, XGBoost)</li>
  <li><strong>Model comparison dashboards</strong> (accuracy, ROC-AUC, F1-score)</li>
  <li><strong>Explainability (SHAP)</strong> – see WHY a customer is predicted to churn</li>
  <li><strong>Retention recommendation logic</strong> (optional)</li>
  <li><strong>Optional API / UI with Gradio or Streamlit</strong></li>
</ul>

<hr/>

<h2 id="architecture">🏗 System Architecture</h2>

<pre><code>Raw Data
   └── Data Cleaning & Preprocessing
         └── Feature Engineering
               └── Model Training (several candidates)
                     └── Model Evaluation (metrics, plots)
                           └── Churn Predictions
                                 └── Explainability (SHAP)
                                       └── Retention Actions / UI
</code></pre>

<hr/>

<h2 id="pipeline">🔄 ML Pipeline</h2>

<pre><code>Load dataset
→ Clean missing values
→ Encode categorical variables
→ Scale numerical features
→ Train ML models
→ Evaluate with AUC/F1/Recall
→ Save best model
→ Predict churn risk for new customers
→ Explain predictions (SHAP)
</code></pre>

<hr/>

<h2 id="installation">🛠 Installation</h2>

<h3>1️⃣ Clone the repository</h3>
<pre><code class="language-bash">git clone https://github.com/chevvakavitha/Customer-Retention-Predictor-Churn-Prediction-System.git
cd Customer-Retention-Predictor-Churn-Prediction-System
</code></pre>

<h3>2️⃣ Install dependencies</h3>
<pre><code class="language-bash">pip install -r requirements.txt
</code></pre>

<h3>3️⃣ Train the model</h3>
<pre><code class="language-bash">python src/train.py
</code></pre>

<h3>4️⃣ Make predictions</h3>
<pre><code class="language-python">from src.predict import predict_customer

customer_data = {...}
result = predict_customer(customer_data)
print(result)   # { "churn_probability": 0.82, "label": "High Risk" }
</code></pre>

<hr/>

<h2 id="structure">📁 Project Structure</h2>

<pre><code>Customer-Retention-Predictor-Churn-Prediction-System/
├── assets/
│   ├── churn_banner.png
│   ├── metrics/
│   └── shap_plots/
├── data/
│   └── raw_data.csv (not included if large)
├── models/
│   └── best_model.pkl
├── notebooks/
│   ├── EDA.ipynb
│   ├── Model_Training.ipynb
│   └── SHAP_Explainability.ipynb
├── src/
│   ├── preprocess.py
│   ├── train.py
│   ├── predict.py
│   ├── evaluate.py
│   └── utils.py
├── app/
│   └── churn_app.py (Streamlit / Gradio UI)
├── requirements.txt
└── README.md
</code></pre>

<hr/>

<h2 id="evaluation">📈 Model Evaluation</h2>
<p>Recommended metrics to include:</p>
<ul>
  <li>ROC-AUC</li>
  <li>Precision / Recall</li>
  <li>F1-Score</li>
  <li>Confusion Matrix</li>
  <li>Feature Importance (SHAP)</li>
</ul>

<p>Place metric images inside:</p>
<pre><code>assets/metrics/
</code></pre>

<hr/>

<h2 id="shap">🧠 Explainability (SHAP)</h2>
<p>Use SHAP to understand why a customer may churn. Add plots such as:</p>

<ul>
  <li>SHAP Summary Plot</li>
  <li>SHAP Force Plot</li>
  <li>Customer-level explanation</li>
</ul>

<p>Save them in:</p>
<pre><code>assets/shap_plots/
</code></pre>

<hr/>

<h2 id="future">🚀 Future Enhancements</h2>
<ul>
  <li>Add customer lifetime value prediction (CLV)</li>
  <li>Integrate with CRM (HubSpot, Salesforce)</li>
  <li>Automated retention recommendation system</li>
  <li>Webhook-powered real-time notifications</li>
  <li>Deploy with Docker / AWS / HuggingFace Spaces</li>
</ul>

<hr/>

<h2 id="author">👩‍💻 Author</h2>
<p><strong>Cheva Kavitha</strong></p>
<ul>
  <li>GitHub: https://github.com/chevvakavitha</li>
  <li>LinkedIn: https://www.linkedin.com/in/cheva-kavitha/</li>
</ul>

<p align="center">⭐ Star this repo if you like the project!</p>
