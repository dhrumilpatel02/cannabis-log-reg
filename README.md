# cannabis-log-reg

# Problem and Analytical Statement
Here the problem we are addressing is that we need to know which the plants are having the quality to be considered as the best which is “1” which can be used for medical purposes, and others that shall be used for other purposes such as recreational use are the rest which will be “0”.

# EDA
During the EDA after eliminating all the null values we retained 1282 non-null values for all the variables, we can see it by running a simple .info statement.
With .describe it can be seen that apart from DBH and Surv, no variable had values less than 10. We will see how this goes with the rest of the analysis.
With the Correlation map, we could see that the lowest correlation was between Surv and Ht, and Surv and Ins_res.
Next, when I ran the qq plot on Surv, Ht and Ins_res variables to see if there is any problem in it, I found out Ins_res and Surv have a fair number of outliers which may affect our model, Ht had a good curve to it so we need not worry about it for now.
I wanted to see if there is more to it than this, so I plotted all three variables on a Histogram to see its distribution. What I could see was that Ht is positively skewed and Surv is negatively skewed, Ins_res was normally distributed.
This was not needed as of now but as I want to make Logistic Regression as my base model, next I ran was a Logistic Regression - Learning Curve just to take a look on how it goes, this was surprisingly very good as it started learning after around 500 samples which is a very good sign. Further, I also evaluated the model by depicting it in a boxplot view.
As mentioned above, the variables Surv, Ins_res, and Ht caught my eye as to if theses three variables could impact our model or not.
In the correlation map, we could see -0.11 correlation between variables Surv and Ht and -0.15 correlation between Ins_res and Surv.
Apart from Ht, Surv and Ins_res did not do well when I plotted them in the QQ plot.
The same goes with histogram, as Ht is positively skewed and Surv is negatively skewed, Ins_res was normally distributed.
Targets for Recall would be to derive the True positives out of the data i.e. the “best” quality plant which is “1”
