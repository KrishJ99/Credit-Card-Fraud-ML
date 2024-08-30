# Credit-Card-Fraud Machine Learning
The objective of this project was to develop a highly effective fraud detection system using machine learning techniques. We employed a Random Forest model due to its robustness and interpretability. Our analysis involved evaluating model performance, understanding feature importance, and utilizing SHAP (SHapley Additive exPlanations) for deeper insights into the model's decision-making process.

### **1. Model Performance**

**Accuracy and Metrics:** The Random Forest model demonstrated outstanding performance:

Accuracy: 99.99%

F1 Score: 0.999943

Recall: 0.999967

Precision: 0.999918

ROC AUC: 1.0

These metrics indicate that the model is highly effective in distinguishing between fraudulent and non-fraudulent transactions. The high recall means all fraudulent transactions were correctly identified, and the high precision indicates very few legitimate transactions were misclassified as fraudulent.

**Confusion Matrix:** The confusion matrix results were:

True Positives (TP): 26,221

True Negatives (TN): 26,219

False Positives (FP): 2

False Negatives (FN): 0

This confirms the model’s accuracy and effectiveness in fraud detection, with no false negatives and a very low number of false positives.

## **2. Feature Importance**

**Key Features Identified:** The feature importance analysis revealed the following key features:

Ratio to Median Purchase Price: 54.66%

Online Order: 10.73%

Distance from Home: 20.87%

Pin Number: 3.13%

Used PIN Number: 2.61%

Distance from Last Transaction: 7.22%

Repeat Retailer: 0.78%

The ratio to median purchase price emerged as the most critical feature, significantly impacting the model's ability to detect fraud. Features such as online order and distance from home also play substantial roles in predicting fraudulent transactions.

## **3. SHAP Analysis**

The SHAP analysis highlighted how each feature contributes to the model’s predictions. Key observations include:

Pin Number and Online Order: Both features significantly influence the prediction of fraud, aligning with their importance scores and indicating their critical role in fraud detection.

Ratio to Median Purchase Price: This feature shows a strong and consistent influence on fraud prediction, confirming its key role.
These plots for ratio to median purchase price illustrated that extreme values of this feature are strongly associated with fraudulent transactions. This insight suggests that transactions deviating significantly from typical purchase ratios are more likely to be flagged as fraud and to be truly fraud
 
These plots provided valuable insights into how individual features contribute to predictions for specific transactions. This analysis helps understand how different features interact to drive the overall fraud prediction.

## **4. Further Analysis and Recommendations**

Model Refinement: The Random Forest model shows excellent performance, but further refinements could include fine-tuning hyperparameters or exploring alternative models to ensure robustness and validity.

Feature Engineering: The identified key features, particularly ratio to median purchase price, online order, and pin number, should be leveraged for further feature engineering. Creating additional features or interaction terms related to these key features could enhance the model’s ability to detect fraud.

Operational Integration: Incorporating the insights from feature importance and SHAP analysis into operational fraud detection systems can help in preemptively identifying suspicious transactions. Rules or alerts based on these critical features can improve fraud detection and prevention strategies.

Continuous Monitoring: Ongoing monitoring and retraining of the model with new data are essential to adapt to evolving fraud patterns. Regular updates will help maintain the model’s effectiveness and relevance over time.

## **Conclusion:**

The Random Forest model has demonstrated exceptional performance in detecting fraudulent transactions, with a high degree of accuracy and effective identification of key fraud indicators. The analyses conducted, including feature importance and SHAP, have provided valuable insights into which features drive the model’s predictions. The key features identified—such as ratio to median purchase price, online order, and pin number—are crucial for understanding fraud patterns and can guide further model development and operational strategies. By leveraging these insights, the fraud detection system can be refined to enhance its accuracy and efficiency in identifying fraudulent transactions.
