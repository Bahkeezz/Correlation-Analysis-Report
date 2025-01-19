# Understanding the Relationships Between Agricultural Factors and Crop Productivity
The objective of this analysis is to investigate the relationships between various agricultural factors such as rainfall, soil quality, farm size, sunlight, and fertilizer usage and crop yield. By leveraging correlation analysis, this study aims to:

1.  Identify the strength and direction of relationships between these factors and crop yield.
2.  Highlight key variables that significantly influence crop productivity.
3.  Provide actionable insights for optimizing farming practices based on data-driven findings.

The ultimate goal is to enable better decision-making for farmers, agricultural planners and policymakers by understanding how these variables interact and contribute to maximizing crop yield.

## Methodology  
To calculate the correlation coefficients, the following formula was applied:  

**`=CORREL(array1, array2)`**

### Formula Implementation Table  

|               | Rainfall (`A`)         | Soil Quality (`B`)        | Farm Size (`C`)           | Sunlight (`D`)            | Fertilizer (`E`)          | Crop Yield (`F`)           |
|---------------|-------------------------|---------------------------|---------------------------|---------------------------|---------------------------|----------------------------|
| **Rainfall**  | `=CORREL($A$2:$A$3001,A$2:A$3001)` | `=CORREL($A$2:$A$3001,B$2:B$3001)` | `=CORREL($A$2:$A$3001,C$2:C$3001)` | `=CORREL($A$2:$A$3001,D$2:D$3001)` | `=CORREL($A$2:$A$3001,E$2:E$3001)` | `=CORREL($A$2:$A$3001,F$2:F$3001)` |
| **Soil Quality** | `=CORREL($B$2:$B$3001,A$2:A$3001)` | `=CORREL($B$2:$B$3001,B$2:B$3001)` | `=CORREL($B$2:$B$3001,C$2:C$3001)` | `=CORREL($B$2:$B$3001,D$2:D$3001)` | `=CORREL($B$2:$B$3001,E$2:E$3001)` | `=CORREL($B$2:$B$3001,F$2:F$3001)` |
| **Farm Size**  | `=CORREL($C$2:$C$3001,A$2:A$3001)` | `=CORREL($C$2:$C$3001,B$2:B$3001)` | `=CORREL($C$2:$C$3001,C$2:C$3001)` | `=CORREL($C$2:$C$3001,D$2:D$3001)` | `=CORREL($C$2:$C$3001,E$2:E$3001)` | `=CORREL($C$2:$C$3001,F$2:F$3001)` |
| **Sunlight**   | `=CORREL($D$2:$D$3001,A$2:A$3001)` | `=CORREL($D$2:$D$3001,B$2:B$3001)` | `=CORREL($D$2:$D$3001,C$2:C$3001)` | `=CORREL($D$2:$D$3001,D$2:D$3001)` | `=CORREL($D$2:$D$3001,E$2:E$3001)` | `=CORREL($D$2:$D$3001,F$2:F$3001)` |
| **Fertilizer** | `=CORREL($E$2:$E$3001,A$2:A$3001)` | `=CORREL($E$2:$E$3001,B$2:B$3001)` | `=CORREL($E$2:$E$3001,C$2:C$3001)` | `=CORREL($E$2:$E$3001,D$2:D$3001)` | `=CORREL($E$2:$E$3001,E$2:E$3001)` | `=CORREL($E$2:$E$3001,F$2:F$3001)` |
| **Crop Yield** | `=CORREL($F$2:$F$3001,A$2:A$3001)` | `=CORREL($F$2:$F$3001,B$2:B$3001)` | `=CORREL($F$2:$F$3001,C$2:C$3001)` | `=CORREL($F$2:$F$3001,D$2:D$3001)` | `=CORREL($F$2:$F$3001,E$2:E$3001)` | `=CORREL($F$2:$F$3001,F$2:F$3001)` |

### Correlation Matrix  

|               | Rainfall | Soil Quality | Farm Size | Sunlight | Fertilizer | Crop Yield |
|---------------|----------|--------------|-----------|----------|------------|------------|
| **Rainfall**  | 1.00     | -0.02        | 0.00      | -0.01    | -0.03      | 0.09       |
| **Soil Quality** | -0.02 | 1.00         | 0.01      | 0.00     | 0.01       | 0.04       |
| **Farm Size** | 0.00     | 0.01         | 1.00      | -0.01    | -0.01      | 0.99       |
| **Sunlight**  | -0.01    | 0.00         | -0.01     | 1.00     | 0.02       | -0.01      |
| **Fertilizer** | -0.03   | 0.01         | -0.01     | 0.02     | 1.00       | 0.10       |
| **Crop Yield** | 0.09    | 0.04         | 0.99      | -0.01    | 0.10       | 1.00       |

### Correlation Heatmap

![Chart](https://github.com/user-attachments/assets/b65f2903-48db-40bb-baf9-bfddcb595cc9)

## Key Findings  

### Farm Size and Crop Yield  
The correlation coefficient of **0.99** indicates a very strong positive relationship between farm size and crop yield. Larger farms tend to produce higher yields.  

### Fertilizer Usage and Crop Yield  
A moderate positive correlation of **0.10** suggests that increased fertilizer usage has a slight positive impact on crop yield.

### Rainfall and Crop Yield  
A weak positive correlation of **0.09** implies that while rainfall may influence crop yield, other factors likely play a more significant role.

### Sunlight and Crop Yield  
The near-zero correlation (-0.01) suggests no significant relationship between sunlight and crop yield, although specific crop types might influence this result.

### Soil Quality and Crop Yield  
The correlation of **0.04** indicates a very weak positive relationship, suggesting that soil quality's impact on crop yield may be minor or dependent on other interacting variables.

## Conclusion  
This analysis highlights the relationships between key agricultural factors and crop yield, with a particular focus on the strong correlation between farm size and crop yield. Future research may explore other variables and their impact on agricultural productivity.
