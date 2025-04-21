# 🏃‍♂️ Sports Wear Group - Advanced Analytics for Marketing Campaigns

## 📌 Project Overview

This project was developed as part of a consulting proposal to **Sports Wear Group**, one of the region’s leading sports retailers with over 50 branches. The aim is to showcase the power of **advanced analytics and machine learning** in improving marketing efficiency and increasing overall sales performance.

We received a sample dataset from the company’s marketing campaign database, including various product attributes, customer interactions, and promotional strategies. Our goal was to extract valuable insights and build predictive models that can help the marketing and management teams make data-driven decisions.

---

## 🎯 Business Objectives

- Help the **Marketing Team** identify the key factors influencing customer purchases and improve campaign targeting.
- Help the **Management Team** understand how analytics can support better product decisions and boost overall sales.
- Demonstrate the **value of using advanced analytics** through technical analysis and business insights.
- Highlight **ML models** that can predict purchase behavior effectively.
- Deliver business insights through **BI visualizations** and **recommendations** for performance improvement.

---

## 📊 Data Description

The dataset contains the following key fields:
- **Customer Details:** customer_id, gender, country
- **Product Information:** article, category, productgroup, style, sizes, regular_price, current_price, cost
- **Marketing Attributes:** promo1 (media ads), promo2 (store events), retail week
- **Purchase Result:** label (1 = purchased, 0 = not purchased)
- **Color Attributes:** RGB intensity of main and secondary product colors
- **Pricing Ratio:** `ratio = current_price / regular_price`

---

## 📈 Exploratory Data Analysis

Insights from the dataset:

- 📌 **Top-selling product groups**: *Shoes* led in sales; *Shorts* and *Sweatshirts* underperformed.
- 🧍‍♂️ **Gender analysis**: *Unisex* items had the highest purchase rate, while *Men* and *Kids* had the lowest.
- 🌍 **Country Trends**: Some countries (like *Germany* and *Netherlands*) showed significantly higher conversion rates, suggesting location-specific preferences and opportunities for market segmentation.
- 💰 **Price Ratio Impact**: High discounts (low price ratio) were associated with reduced purchases; moderate pricing close to the regular price led to higher conversions.
- 🎯 **Promotions**: Customers exposed to both *Promo1* and *Promo2* had significantly higher purchase rates than those who received none.
- 📉 **Price vs Sales**: As price increases, purchases decrease — suggesting price sensitivity among customers.

📊 A **Power BI dashboard** was built to present this analysis interactively.

---

## 🧠 Machine Learning Models

We framed the problem as a **binary classification task** (purchase or not).

### ✅ Single Models:
```python
Single_models = {
    'Logistic Regression': LogisticRegression(),
    'KNN': KNeighborsClassifier(),
    'Naive Bayes': GaussianNB(),
    'SVM': SVC(),
    'Decision Tree': DecisionTreeClassifier()
}
🔁 Ensemble Models:
python
Always show details

Copy
ensemble_models = {
    'Random Forest': RandomForestClassifier(),
    'Extra Trees': ExtraTreesClassifier(),
    'Bagging': BaggingClassifier(),
    'AdaBoost': AdaBoostClassifier(),
    'Gradient Boosting': GradientBoostingClassifier(),
    'XGBoost': XGBClassifier()
}
Each model was trained using the available features to predict the label (conversion). Performance was evaluated using:

Accuracy

Precision, Recall, F1-score

Confusion Matrix

ROC-AUC

📌 Best results were achieved using ensemble models like Random Forest and Bagging, which captured complex patterns in customer behavior.

📂 Project Files
- sports_wear.ipynb: Full analysis and model training code

- sports_wear.pbix: BI dashboard showing trends and insights

- Sports Wear Group Recommendation.txt: Business recommendations for marketing & pricing

- README.md: Project summary and technical documentation

📝 Business Recommendations
Key takeaways provided to Sports Wear Group:

1-Focus on promoting Unisex and Shoes items which drive the most conversions.

2-Avoid deep discounts — moderate price drops perform better.

3-Combine Promo1 (ads) and Promo2 (events) for maximum impact.

4-Reconsider underperforming groups like Shorts and Sweatshirts or apply targeted promotions.

5-Target top-performing countries and customize campaigns based on regional behavior.

6-Use machine learning predictions to prioritize customers likely to convert.

🤝 Author
Mohamed Mahmoud Mohamed Al-Akhal
