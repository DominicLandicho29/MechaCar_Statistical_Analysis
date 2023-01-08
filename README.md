# MechaCar_Statistical_Analysis
## Overview
- The purpose of this project is to analyze data in R using a variety of scripts to compare car performance aross different metrics
## Linear Regression to Predict MPG
![image](https://user-images.githubusercontent.com/111463407/211217376-e6f6cc48-6af5-4f51-aad0-4a344ebde36a.png)

Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

- Vehicle length and ground clearance provided a non-random amount of variance given their coeficients

Is the slope of the linear model considered to be zero? Why or why not?

- The slope is not zero due to the small p-value

Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

- Our "Multiple R-Squared" value is roughly 71%, meaning this linear model is fairly effective in predicting mpg.

## Summary Statistics on Suspension Coils
![image](https://user-images.githubusercontent.com/111463407/211219129-65c6454c-de79-419d-b9f0-32cdf548769f.png)
![image](https://user-images.githubusercontent.com/111463407/211219140-f512f150-c4fb-42c8-95b1-cf7048c50758.png)

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

- Looking at the Summary of all lots, the variance of the suspensions coils remains in compliance, however, upon individual statistics, "Lot 3" has a median variance of 170, exceeding our limit of 100.

## T-Tests on Suspension Coils
![image](https://user-images.githubusercontent.com/111463407/211219952-3e14fef5-5f9e-4445-99c8-ff86af18b9eb.png)
![image](https://user-images.githubusercontent.com/111463407/211220192-f44988d3-acd9-428f-9d0c-5e9264514487.png)
![image](https://user-images.githubusercontent.com/111463407/211220204-79c081f5-139c-4eeb-a77a-575b8e272f31.png)
![image](https://user-images.githubusercontent.com/111463407/211220225-8ec1e5c3-1834-4cb2-81b5-8c285e328522.png)

- We fail to reject the null hypothesis in both Lot 1 & Lot 2 due to both p-values being > 0.05
- In Lot 3 we can reject the null hypothesis with it's p-value being 0.05.

## Study Design: MechaCar vs Competition
 
An additional study that could be run to compare MechaCar vs Competition would be on fuel efficiency. 

Necessary metrics:
- MPG (City and Highway)

The null hypothesis would be that both mpg are similar, meaning the alternate hypothesis would be the mpgs differ.

I would use two-sample t-tests and use their p-values to determine the validity of the null hypothesis.

Data on MPG would be needed to run the tests. I would also compare City and Highyway data seperately.

