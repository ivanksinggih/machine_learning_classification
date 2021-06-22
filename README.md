# Semiconductor Operation Test

Source: https://www.kaggle.com/paresh2047/uci-semcom?select=uci-secom.csv  
  
The data are collected using continuously observing sensors in a complex semiconductor manufacturing system.  
- Some input features are irrelevant, and can be considered as noise.  
- Engineers typically have a much larger number of signals than are actually required.  
  
It is necessary to perform feature selection to identify the most relevant signals.  
- The Process Engineers may then use these signals to determine key factors contributing to yield excursions downstream in the process.  
- This will enable an increase in process throughput, decreased time to learning and reduce the per unit production costs.  
Input data: 590 features, Output data: pass/fail information (in house line testing)  
  
![image](https://user-images.githubusercontent.com/42261330/122785883-b6736f80-d2ee-11eb-89c4-9bf928001d9e.png)
  
Analysis points: Generate various prediction models after removing empty values:  
- Model 1: Using all features (columns), but only complete records (rows)  
- Model 2: Removing all features (columns) with any empty values and all records (rows)  
- Model 3: Any model with some selected features and records. Select important features from Model 1
