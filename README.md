# Diesel Engine Optimization

Source: http://www.irphouse.com/ijert19/ijertv12n12_41.pdf  
Input data: 2 features (biodiesel fuels: C16 and C18:1)  
Output data: 2 factors to be minimized (BSFC and NOx)  
It is expected to define the required input values to minimize the output values.  
The output values should be classified into some classes based on their quartile values.  
  
Analysis points: Range of input values to produce each output in lower quartile classes, compared with higher quartile classes.
- Individual observation only for BSFC
- Individual observation only for NOx
- Simultaneous observation for BSFC and NOx (e.g., using a weighted function)
  
![image](https://user-images.githubusercontent.com/42261330/122784178-31d42180-d2ed-11eb-804b-895252c80110.png)

Preprocessing:  
- Classifying output data into quartiles  
- Combining BSFC and NOx values with 50% portion for each factor  

![image](https://user-images.githubusercontent.com/42261330/122844860-81dad480-d33d-11eb-8372-c77931320e3f.png)

Output:  
- Low accuracy (might be because of the small dataset size)  
  
Detailed boxplots:  
Boxplot 1 (output: BSFC quartiles)  
![image](https://user-images.githubusercontent.com/42261330/122844936-a46ced80-d33d-11eb-8810-6a4fe377aa87.png)  
  
Boxplot 2 (output: NOx quartiles)  
![image](https://user-images.githubusercontent.com/42261330/122844984-b5b5fa00-d33d-11eb-8be3-fc9bc8d1a51f.png)  
  
Boxplot 3 (output: Combined BSFC and NOx quartiles)  
![image](https://user-images.githubusercontent.com/42261330/122845009-bea6cb80-d33d-11eb-84e7-e1cefd48f860.png)
