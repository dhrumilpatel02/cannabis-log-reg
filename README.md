# cannabis-quality

# Introduction
•	This report generates analysis and evaluation of the cannabinoid potency.  
•	The analysis will give us valuable insights on which plant quality we should consider as the best, that shall help us differentiate it either for medical use or for recreational use.


# Key Questions
•	If Data Analysis can help us gain any insights out of the processes or not  
•	If a plant of the best quality (which can be used for medical purpose) or not  
•	If a plant is of comparatively lower quality (which can be used for recreational purpose) or not. Which may not be Starseed’s main aim, but it can bring them extra revenue to support the medical process  

# Dataset Summary
•	PMCno-seedlot number  
•	dbh-diameter at breast height  
•	ht-heat treatment  
•	surv-survival trees  
•	vig-vigour  
•	ins_res-insect resistance  
•	Stem_Fm-stem form  
•	Crown_Fm-crown form  
•	Brnch_Fm-branch form  
•	Utility-utility rating    
•	During the EDA after eliminating all the null values we retained 1282 non-null values for all the variables, we can see it by running a simple .info statement.  
•	With .describe it can be seen that there is a pattern between variables.  
•	With the Boxplot visualizations of the features, we could see that there are a significant number of outliers in the dataset.  
•	We could fix them with using Tukey method for eliminating outliers.  
•	For any kind of analysis, the data needs to be balanced. For this need to see if we have enough data which is balanced so we can predict various scenarios.  
•	We used SMOTE to balance the dataset, and finally we had the dataset ready for model building.  

# Model Analysis
•	During the Model Building phase, after splitting the training testing and the validation dataset, I tried to construct pipelines which could plot me Logistic Regression Learning curve.  
•	Here we can see that right from the 1st training sample, it started to learn from the model. At around 275 samples out validation dataset got closer for the first time to the training.  
•	Finally at around 400-500 training samples, we achieved the meeting point of the validation and as well as training curve.  
•	Next we tried to evaluate the model via boxplot where we could see how much our Logistic Regression Model and the Recall values fair with each other.  
•	As we can see that the boxplot view shows us, that the model and recall values are from the range of 70% and above.  
•	This is a good sign as we could possibly achieved hood accuracy for the dataset provided.  
•	Next, I tried to Optimize the model via Grid Search Function.  
•	While testing and validating the model, we could achieve a NestedCV Weighted Accuracy of 76%, a NestedCV Weighted Precision of 86%, a NestedCV Weighted Recall of 76%, which is fairly good as we cross validated it by not only using the training, testing but also the validation data.  
•	When we see the ROC curve, as the breaking point is at around (0.7 and 0.2) it can be said that the model is performing well as it tells us if the model is capable of distinguishing between classes.  

# Results
•	The insights and findings that we gain from the analysis is that as this dataset is built in a particular nature, even a recall of 76% is good to achieve.  
•	As the Learning curve depicts, that the model is learning through the whole process, our EDA, and model selection criteria have paid off as it is a good fit.  
•	It is evident that we Starseed can set up a pipeline where they can start selling recreational cannabis as we could see there is a fair amount of plants that will be wasted if we ignore it all together, and it can definitely give a good revenue source for Starseed.  

# Conclusion
•	Our analysis helps us understand the plants better by spotting the best ones.  
•	Similarly, our analysis can also help them understand if there is a potential in the recreational market as the company should consider selling recreational cannabis from there existing resources which shall help them in their revenues.  
