# Predicting-Donor-Retention-for-Nonprofit-Organizations
## Donor Retention Prediction System
📊 Predict donor churn and empower nonprofits with actionable insights
### 🎯 Initial Project Goal & Prompt
Prompt: Use data and technology to help nonprofit organizations address real-world challenges.
My Goal: Build a system that predicts donor retention (churn vs. repeat giving) and communicates results in a way that:
Supports analysts with technical detail and metrics.
Empowers nonprofit leadership with clear, actionable insights for improving donor engagement.
### Features Added
#### Data Preprocessing Pipeline
   Cleaned raw CSV donor datasets.
   Handled missing values, standardized date formats, and engineered features (donation frequency, recency, campaign type).
#### Machine Learning Models
Implemented Logistic Regression, Random Forest, and Gradient Boosting for donor churn prediction.
Compared performance using AUC, precision-recall, and F1-score.
#### Model Interpretability
Used SHAP values to highlight which features most influence donor retention.
Example: Donors who give within 90 days of their first donation are significantly more likely to return.
#### vInteractive Dashboard (Streamlit)
Analyst View → technical metrics, feature importance, churn probability distribution.
Leadership View → donor risk segmentation, high-level insights, actionable recommendations.
Demo Dataset
Provided a sample_donors.csv file with realistic donor data for testing and demos.
### ⚙️ Technical Challenges & Solutions
#### Challenge	Solution
Handling diverse donor data formats	Designed a standardized CSV schema (donor_id, age, gender, income_bracket, donation_date, donation_amount, campaign_type, communication_channel, donor_retained). Also included demo data for consistent testing.
Class imbalance (few churn cases vs. many retained donors)	Used oversampling techniques (SMOTE) and adjusted class weights in ML models to improve recall.
Making models interpretable to non-technical users	Integrated SHAP-based visualizations and wrote plain-language explanations for leadership dashboards.
Time constraints of a hackathon	Focused on a minimal viable product (MVP) with classical ML models and clear dashboards first, then documented future enhancements (deep learning, time-series, real-time streaming).
### 📚 New Technologies & Concepts Learned
#### SHAP for Model Interpretability → translating technical model outputs into actionable insights for non-technical stakeholders.
#### Streamlit → rapid prototyping of interactive dashboards for dual user audiences.
#### Data-Driven Storytelling → balancing technical detail with clear communication, ensuring nonprofits understand what to do next.
#### Agile Hackathon Development → prioritizing MVP features under time pressure while planning future extensions.
### 🚀 Future Enhancements
Deploy as a web app with role-based access control (different dashboards for analysts vs. leadership).
Integrate real-time donation feeds (AWS, Spark) for live predictions.
Extend to recommendation systems (e.g., best outreach channel for high-risk donors).
Explore NLP on donor communication text to identify sentiment impact on retention.
### 💡 Key Takeaway
This project demonstrates how machine learning + visualization + clear communication can make a measurable impact for nonprofits. By predicting donor churn and providing actionable retention strategies, nonprofits can save costs, improve fundraising efficiency, and build stronger long-term donor relationships.
