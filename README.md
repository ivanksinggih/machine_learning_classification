# Steel Plate Defect Detection

Source: https://www.kaggle.com/bpkapkar/steel-plates-faults-detection?select=Variable+Descriptor.txt  

Input data: 27 features  
V1: X_Minimum  
V2: X_Maximum  
V3: Y_Minimum  
V4: Y_Maximum  
V5: Pixels_Areas  
V6: X_Perimeter  
V7: Y_Perimeter  
V8: Sum_of_Luminosity  
V9: Minimum_of_Luminosity  
V10: Maximum_of_Luminosity  
V11: Length_of_Conveyer  
V12: TypeOfSteel_A300(X) 
V13: TypeOfSteel_A400(X)  
V14: Steel_Plate_Thickness  
V15: Edges_Index(X)  
V16: Empty_Index(X)  
V17: Square_Index(X)  
V18: Outside_X_Index(X)  
V19: Edges_X_Index(X)  
V20: Edges_Y_Index(X)  
V21: Outside_Global_Index(X)  
V22: LogOfAreas  
V23: Log_X_Index(X)  
V24: Log_Y_Index(X)  
V25: Orientation_Index(X)   
V26: Luminosity_Index  
V27: SigmoidOfAreas  
  
**[Note] (Selected input data characteristic: nominal data type (e.g., small = little amount, large = a lot of amount), not class type (e.g., class 1, class 2, …)**

Output data: 6 types of defects (V28)  
1: Pastry  
2: Z_Scratch  
3: K_Scatch  
4: Stains  
5: Dirtiness  
6: Bumps

![image](https://user-images.githubusercontent.com/42261330/122784006-09e4be00-d2ed-11eb-9903-0a3b383be229.png)

Analysis points:  
- Given the input data information, how to automatically detect type of defects.  
- Show the priority of each input data for detecting the defect (operators might focus more on controlling such input variables).
