# Heart Disease Prediction Metrics

![cover Project conterbuter](<image Presentation/cover-for-project.png>)


## Table of Contents
1. [Project Purpose / Description](#project-purpose)
2. [Goals/Questions to be addressed](#goals-questions)
3. [Overview of data collection, cleanup, and exploration process](#overview-data-collection)
4. [Approach taken to achieve goals](#approach-taken)
5. [Future development](#future-development)

<a name="project-purpose"></a>
## Project Purpose / Description

This project focuses on the factors that predict heart disease in adults. To determine the factors that predict heart disease in adults we used a single large data set from the CDC. To simplify our workload we utilized a previously cleaned dataset in this project.

The original dataset from the CDC had over 300 data points, and nearly half a million participants spanning decades. Our trimmed dataset from this larger group of data contained 18 data points and 319,795 participants.

<a name="goals-questions"></a>
## Goals/Questions to be addressed

When we started this project we envisioned the following questions would be important for our project:
1. What is the most important factor in determining heart disease?
2. What are the highest correlated factors for heart disease?
3. What groups are the most at risk for heart attacks?
4. What could be the most important choices made to reverse the potential negative outcomes of heart disease?
5. How will this data help hospitals to make informed decisions and develop effective business plans and strategies?


<a name="overview-data-collection"></a>
## Overview of data collection, cleanup, and exploration process

As we mentioned earlier our data was already cleaned, for the most part. We did need to convert a lot of the data entries into 0 and 1 to replace the values for keys in the data dictionary, as well as mapping some of the values into integers...

<p align="center">
  <img src="image Presentation/Data reframining sample code.png" alt="Data Reframing" width="600" >
</p>

This image shows one of our methode to chage the Data in Some columns so we can calculate the correlation


<a name="approach-taken"></a>
## Approach taken to achieve goals

Provide a summary of the results with the supporting visualizations (at least 2 per question)
To answer our questions we mainly focused on correlations and risk factors that seemed to stand out.



<p align="center">
  <img src="image Presentation/loop dscribe.png" alt="loop Describe" width="800" >
</p>
Due to the Big number of columns we used a loop to heck the Data


1. **What is the most important factor in determining heart disease?**

   For this, we determined that general health was the largest determinant in developing heart disease. You can see from the following graph that even through our lifespan it remains as one of the highest variables correlated to disease. Following general health we can see that physical activity also plays a lifelong role in your heart's health.

   Some interesting points we noticed looking at this data are that as we age heart disease becomes more prevalent in men, although men remain at a higher risk than women according to this data, it increases with age.
   
We used this Code to Plot all the factors to find and see the correlation - we used a diffrent methods this is oe of them

<p align="center">
  <img src="image Presentation/Ploting all the factors.png" alt="Ploting all Factors code" width="800" >
</p>

   
 after using the Code this is the Result, which gave us a graph for each factor for its correlation  
   
 
<p align="center">
  <img src="image Presentation/HD with factors.png" alt="all factors ploted Graph " width="1000" >
</p>   




   This is all factors are ploted in one Graph:

<p align="center">
  <img src="[image Presentation/Data reframining sample code.png](https://github.com/jkranyak/PROJECT_1_team_decisionmankers/blob/main/images/Squid_Graph.png)" alt="Squid Graph" width="1000" >
</p>
   
 

2. **What are the highest correlated factors for heart disease?**

   We reframed this question to ask; what are the highest correlated factors TO heart disease and ran our data. The highest correlated factors were age and general health, this seemed intuitive. Other than that, some more data we uncovered seemed to also be rather intuitive; such as the correlation between general health and difficulty walking, which had the highest heat map correlation.


   ![correlation heat map](<image Presentation/Correlation Heatmap.png>)








   ![eart Disease by Age Category and Gender ](<image Presentation/Heart Disease by Age Category and Gender.png>)


3. **What groups are the most at risk for heart attacks?**

   We found that the most at-risk groups for heart disease were aging populations, men, Native Americans followed by Whites, smokers vs non-smokers (12% vs 6%), and having diabetes.



   ![Percentage of People with Heart Disease by Race](<image Presentation/Percentage of People with Heart Disease by Race.png>)


4. **What could be the most important choices made to reverse the potential negative outcomes of heart disease?**

   It's hard to extrapolate from our data the information we need to answer this question, aside from the obvious factors, such as stop smoking if you smoke, sleeping for about 7 hours per night and taking care of your general health.
   
   However, as a critical thinking exercise, we would suggest that this data is indicative of reducing heart disease by living an active and healthy lifestyle; perhaps that would include exercise, staying physically active, and maintaining your ability to walk as long as possible. Also, the data around BMI seems to suggest that staying around 20-25BMI has the least risk, so keeping a healthy diet would help in reducing your risk of heart disease… but the data also indicates that a BMI too low also increases your risk of developing heart disease! So, don’t skip dessert too many times, and have a drink! It seems that drinking had a negative correlation on heart disease according to this data set.


   ![sleep time and heart Disease](<image Presentation/Average Heart Disease Occurrence by sleep time.png>)



   ![Physical Activity and heart Disease Graph](<image Presentation/Average Heart Disease Occurrence by physical activity.png>)



   ![Smoking and Heart Disease](<image Presentation/Percentage of People with Heart Disease by Smoking Status'.png>)

5. **How will this data help hospitals to make informed decisions and develop effective business plans and strategies?**

   As mentioned earlier, this question poses a bit of an issue for us. We believe that over the next few weeks as our class gets into more developed machine learning and AI tools we would be in a better position to answer a question like this using our data set. However, at this point, we would just be making uneducated guesses as to how or where this could be used.

   We did take a look at some more advanced projects around heart disease that encompassed the Random Forest Classifier, K-Nearest neighbor, Decision Tree classifier, Support Vector Machines, and Artificial Neural Networks.

   When using the end-to-end implementation of all these methods these data sets really began to kick out some very useful data on predicting heart disease in the very early stage.

   Some of the data surrounding the increases in heart disease as a comorbidity for other medical issues would also be important information for hospitals to have access to. For instance, people that have had skin cancers, asthma, diabetes, and kidney disease all had a higher risk of developing heart disease than those people who did not.


<a name="future-development"></a>
## Future development

Looking at the future in terms of projects in heart disease, our group would be interested in looking at other datasets that included more data that revolved around specific questions. For instance, diet, physical locale, income, stress levels. This data could also be compared or grouped with other data frames, such as pollution levels by geography. We are sure that the depth of information that epidemiologists have gathered is already ahead of us, and we are looking forward to discovering these projects as we continue to learn.


![Machine Learing Sample](<image Presentation/RandomForest Importances for Heart Disease Prediction.png>)
