# *Module 14 Challenge: ML Evaluation Report* 
---

**The SVM baseline model input features:**

**Training period: 3 months, Short SMA Window: 4, Long SMA Window: 100** 

![alt text](https://github.com/Z1WenChen/ZiwenChen_Columbia_FinTech_-Challenges/blob/main/Module_14_Challenge_file/Starter_Code/SVM_Baseline.png)

**The SVM baseline model Conclusion: Based on the figure above, we can find that strategy returns always outperforms the actual returns. The strategy returns is 1.5 in the end.** 

------------------------------------------------------------------------------------------------------------

**The SVM 2nd model input features:**

**Training period: 6 months, Short SMA Window: 4, Long SMA Window: 100** 


![alt text](https://github.com/Z1WenChen/ZiwenChen_Columbia_FinTech_-Challenges/blob/main/Module_14_Challenge_file/Starter_Code/SVM_2nd.png)

**The SVM 2nd model Conclusion: Based on the figure above, we can find that strategy returns not always outperforms the actual returns. But, the strategy returns is 1.8 in the end. Therefore, it seems that the strategy returns would increase if increasing the training window from 3 months to 6 months.** 

**I would choose this SVM 2nd model with the input features: 6 months, Short SMA Window: 4, Long SMA Window: 100, because this model generates a higher return in the end.** 

------------------------------------------------------------------------------------------------------------

**The SVM 3rd model input features:**

**Training period: 3 months, Short SMA Window: 10, Long SMA Window: 100** 

![alt text](https://github.com/Z1WenChen/ZiwenChen_Columbia_FinTech_-Challenges/blob/main/Module_14_Challenge_file/Starter_Code/SVM_3rd.png)

**The SVM 3rd model Conclusion: Based on the figure above, we can find that strategy returns always underperforms the actual returns. The strategy returns is 1.4 in the end. Therefore, it seems that the strategy returns would decrease if increasing the short window of SMA features** 

------------------------------------------------------------------------------------------------------------

**The LogisticRegression 2nd model input features:**

**Training period: 6 months, Short SMA Window: 4, Long SMA Window: 100** 

![alt text](https://github.com/Z1WenChen/ZiwenChen_Columbia_FinTech_-Challenges/blob/main/Module_14_Challenge_file/Starter_Code/LogisticRegression_2nd.png)

**The LogisticRegression 2nd Conclusion: Based on the figure above, we can find that strategy returns always underperforms or aligns with the actual returns. The strategy returns is almost 1.6 in the end. Therefore, the logistic regression model performs a little bit better than the baseline model as it generates 1.6 return in the end vs 1.5 of baseline model, but it performs worse than the tuned trading algorithm as it only returns 1.6 but SVM_2nd returns 1.8 in the end** 
