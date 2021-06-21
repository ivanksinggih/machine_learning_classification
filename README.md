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
V12: TypeOfSteel_A300  
V13: TypeOfSteel_A400  
V14: Steel_Plate_Thickness  
V15: Edges_Index  
V16: Empty_Index  
V17: Square_Index  
V18: Outside_X_Index  
V19: Edges_X_Index  
V20: Edges_Y_Index  
V21: Outside_Global_Index  
V22: LogOfAreas  
V23: Log_X_Index  
V24: Log_Y_Index  
V25: Orientation_Index   
V26: Luminosity_Index  
V27: SigmoidOfAreas  
  
Output data: 6 types of defects  
V28: Pastry  
V29: Z_Scratch  
V30: K_Scatch  
V31: Stains  
V32: Dirtiness  
V33: Bumps

![image](https://user-images.githubusercontent.com/42261330/122784006-09e4be00-d2ed-11eb-9903-0a3b383be229.png)

Analysis points:  
- Given the input data information, how to automatically detect type of defects.  
- Show the priority of each input data for detecting the defect (operators might focus more on controlling such input variables).
