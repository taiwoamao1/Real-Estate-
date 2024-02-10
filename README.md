## Real-Estate-
#### Statistical Methods


## Table of contents
---
- [Project overview](#project-overview)
- [Data source](#data-source)
- [Tool](#tool)
- [Data preparation](#data-preparation)
- [Data Analysis](#data-analysis)
- [Results](#results)
- [Insights](#insights)
 


### Project Overview
---
This project aims to check if there is a  correlation between the  size of a house and market value. 

![image](https://github.com/taiwoamao1/Real-Estate-/assets/112169247/289bfe04-1946-4bf0-8f9b-8f43ebafee82)



### Data source
A fictitious data. 
### Tool
- Excel - analyse and report.


### Data Preparation 
- The business requirements are identified for the project.
- Fictional data was used.
- Prepared the data.
- Analysed the data.
- Visualised the data. 


### Data Analysis
- Excel was used for  analysis.
- R programming for analysis.

- 

  
### Results
#### Excel Analysis 
The data was analysed using statistical methods- mean, median, standard deviation, and correlation.
The analysis results are summarised as follows:
  
Mean 	£96,671.43
Median	£93,300.00
Max	£108,500.00
Min	£87,600.00
STDV	8137.508686
Correlation	0.894082212
Slope	£77.59
Intercept 	-£47,159.99


#### R programming Analysis

# Create a data frame
Data_Frame <- data.frame (
  Square_feet = c(1812, 1914, 1842, 1812, 1836, 2028, 1732),
  Market_Value = c(90000, 104400, 93300, 91000, 101900, 108500, 87600)
 )
 sd (Data_Frame$Square_feet)
 sd (Data_Frame$Market_Value)
# Create a scatter plot
plot (Data_Frame$Square_feet, Data_Frame$Market_Value, xlab = " Sq. Ft.", ylab = " Market Value", main = " Sq. Ft. vs. Market Value")

# Create a linear regression model
lm_model <- lm (Market_Value ~ Square_feet, Data_Frame)
summary (lm_model)
# Create a scatter plot with regression line
plot (Data_Frame$Square_feet, Data_Frame$Market_Value, xlab = " Sq. Ft.", ylab = " Market Value", main = " Sq. Ft. vs. Market Value")
abline (lm_model, col = "red")
# Create a scatter plot with regression line and confidence interval
plot (Data_Frame$Square_feet, Data_Frame$Market_Value, xlab = " Sq. Ft.", ylab = " Market Value", main = " Sq. Ft. vs. Market Value")
abline (lm_model, col = "red")
ggplot (Data_Frame, aes (x = Square_feet, y = Market_Value)) + 

![image](https://github.com/taiwoamao1/Real-Estate-/assets/112169247/cd40a1e0-82a1-4f49-8402-772a76533da0)

![image](https://github.com/taiwoamao1/Real-Estate-/assets/112169247/4fcf7125-650c-4322-a75a-d8c6d13acf32)

r2= 0.7994. 
The correlation shows a positive relationship between  the two variables. The independent variable (Square feet ) and dependent variable (market value). 

### Insights
The above results show there is a positive relation between the size of the house and market value. An increase in the size of the house will lead to an increase in the market value.
For every increase in the size of the house, the market value will increase.
The intercept shows if the size of the house is below 1700 the market value is going to be £-47, 159.99. 
The slope shows for every increase in the size of a house, the market value will be up by £77.59.
To get a good market value for a house, the size of the house will have to  increase.

