1. Project objective: Build a decision tree model that predicts whether a consumer will terminate his/her contract.
In this classification problem, I explored how changing parameters affect the predictive capacity of decision tree model.

2. Data description:


----- ---------- --------------------------------------------------------------
- 1     revenue:    Mean monthly revenue in dollars
- 2     outcalls:   Mean number of outbound voice calls
- 3     incalls:    Mean number of inbound voice calls
- 4     months:     Months in Service
- 5     eqpdays:    Number of days the customer has had his/her current equipment
- 6     webcap:     Handset is web capable
- 7     marryyes:   Married (1=Yes; 0=No)
- 8     travel:     Has traveled to non-US country (1=Yes; 0=No)
- 9     pcown:      Owns a personal computer (1=Yes; 0=No)
- 10    creditcd:   Possesses a credit card (1=Yes; 0=No)
- 11    retcalls:   Number of calls previously made to retention team
- 12    churndep:   Did the customer churn (1=Yes; 0=No)

3. Modeling Steps:
- Data exploration
- Data Visualization
- Modeling and Evaluation

4. Insights: 
- Accuracy (0.61): The model correctly classifies 61% of instances overall. While this accuracy is better than random guessing, 
it’s relatively low, indicating that the model might struggle to consistently make accurate predictions across both classes.
- Precision (0.58): The precision score of 0.58 suggests that when the model predicts "Churners," it’s correct only 58% of the time. 
This could indicate a high number of false positives (incorrectly labeling "Non churners" as "Churners"). 
This may be a concern if the cost of falsely predicting churn is high, such as wasting resources on retaining customers who aren't likely to churn.
- Recall (0.77): The model has a relatively high recall of 0.77, meaning it successfully captures 77% of actual "Churners." 
This shows that the model is good at identifying most of the true "Churners," which is often a priority when you want to take actions like retention efforts. 
However, this comes at the expense of precision, meaning some customers labeled as churners may not actually churn.
- F1-Score (0.66): The F1-score, a balance between precision and recall, is 0.66. 
This score is moderately high and suggests a trade-off between recall (finding as many churners as possible) and precision (reducing false positives). 
Given that recall is higher than precision, the F1-score reflects that the model may favor capturing more potential churners even at the risk of misclassifying some non-churners.

5. Recommendations: 
- Explore additional features to see if a higher overall accuracy and balanced precision-recall can be achieved.
- Further tune the parameters using grid search to improve performance.

6. Skills and Tools
- Exploratory Data Analysis (Variable identification, Univariate analysis, Bi-Variate analysis)
- Data Pre-processing
- Decision Tree Regression
- Model Evaluation

