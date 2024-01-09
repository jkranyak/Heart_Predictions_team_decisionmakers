# PROJECT_1_Team_DecisionMakers

## Heart Disease Prediction Metrics
![Alt text](<images/Project Cover img.jpg>)

## **All Code created by:**
- Jesse Kranyak
- Jeff Boczkaja
- Mohamed Altoobi
- Siriesha Mandava


This project focuses on the factors that predict heart disease in adults.  To determine the factors that predict heart attacks in adults several data sets were utilized and cleaned in this project, and referenced below.  

## Questions we hope to answer in this project;

1. What is the most important factor in determining heart disease?
2. What are the highest coorelated factors for heart disease?
3. What groups are the most at risk for heart attacks?
4. What could be the most important choices made to reverse the potential negative outcoes of heart disease?
5. How will this data help hospitals to make informed decisions and develop effective business plans and strategies?

![Alt text](<project_1 data/project_heart.jpeg>)



### Project Purpose / Description

This project focuses on the factors that predict heart disease in adults. To determine the factors that predict heart disease in adults we used a single large data set from the CDC.  To simplify our workload we utilized a previously cleaned dataset in this project.  

The original dataset from the CDC had over 300 data points, and nearly half a million participants spanning decades. Our trimmed dataset from this larger group of data contained 18 data points and 319,795 participants. 

### Goals/Questions to be addressed

When we started this project we envisioned the following questions would be important for our project;

1. What is the most important factor in determining heart disease?
2. What are the highest correlated factors for heart disease?
3. What groups are the most at risk for heart attacks?
4. What could be the most important choices made to reverse the potential negative outcomes of heart disease?
5. How will this data help hospitals to make informed decisions and develop effective business plans and strategies?

After directing and researching our data, we were happy with the questions that we had originally came up with although the 5th question left us a little stumped.  We will get to that later. 

### Overview of data collection, cleanup and exploration process

As we mentioned earlier our data was already cleaned, for the most part.  We did need to convert a lot of the data entries into 0 and 1 to replace the values for keys in the data dictionary, as well as mapping some of the values into integers; one example is listed below, where we categorized BMI into a value map from 1-5, so that we could later use the data more readily in creating our analysis. 

For example;
Index for BMI 
Category 1: BMI <= 18.5
Category 2: 18.5 < BMI <= 24.9
Category 3: 24.9 < BMI <= 29.9
Category 4: 29.9 < BMI <= 34.9
Category 5: BMI > 34.9

Additionally we arranged the ages into categories this way as well. Using the original age grouping was creating some issues for our data set.

After we finished this final bit of cleaning we began exploring the data.       Most of our data exploration we’re sure will get covered exhaustively in these presentations so we will go over some of our more creative uses of code that perhaps haven’t been explored by other groups yet. 

DROP CODE

DROP CODE 

DROP CODE


### Approach taken to achieve goals

To answer our questions we mainly focused on correlations and risk factors that seemed to stand out.  
1. What is the most important factor in determining heart disease?

For this we determined that general health was the largest determinant in developing heart disease. You can see from the following graph that even through our lifespan it remains as one of the highest variables correlated to disease.  Following general health we can see that physical activity also plays a lifelong role in your hearts health.  

Some interesting points we notice looking at this data are that as we age heart disease becomes more prevalent in men, although men remain at a higher risk than women according to this data, it increases with age.  

2. What are the highest correlated factors for heart disease?

We reframed this question to ask; what are the highest correlated factors TO heart disease and ran our data.  The highest correlated factors were age and general health, this seemed intuitive.  Other than that, some more data we uncovered seemed to also be rather intuitive; such as the correlation between general health and difficulty walking, which had the highest heat map correlation.  

3. What groups are the most at risk for heart attacks?

We found that the most at risk groups for heart disease were aging populations, men, Native Americans followed by Whites, smokers vs non smokers (12% v 6%), and having diabetes 

DROP GRAPHS

4. What could be the most important choices made to reverse the potential negative outcomes of heart disease?

Its hard to extrapolate from our data the information we need to answer this question, aside from the obvious factors, such as stop smoking if you smoke, sleeping for about 7 hours per night and taking care of your general health.  

However, as a critical thinking exercise we would suggest that this data is indicative of reducing heart disease by living an active and healthy lifestyle; perhaps that would include exercise, staying physically active and maintaining your ability to walk as long as possible.  Also the data around BMI seems to suggest that staying around 20-25BMI has the least risk, so keeping a healthy diet would help in reducing your risk of heart disease… but the data also indicates that a BMI too low also increases your risk of developing heart disease! So, don’t skip dessert too many times, and have a drink!  It seems that drinking had a negative correlation on heart disease according to this data set.  

5. How will this data help hospitals to make informed decisions and develop effective business plans and strategies?

As mentioned earlier, this question poses a bit of an issue for us.  We believe that over the next few weeks as our class gets into more developed machine learning and AI tools we would be in a better position to answer a question like this using our data set.  However, at this point we would just be making uneducated guesses as to how or where this could be used.  

We did take a look at some more advanced projects around heart disease that encompassed the Random Forest Classifier, K-Nearest neighbor, Decision Tree classifier, Support Vector Machines, and Artificial Neural Networks.  

When using end to end implementation of all these methods these data sets really began to kick out some very useful data on predicting heart disease in very early stage.  

Some of the data surrounding the increases in heart disease as a comorbidity for other medical issues would also be important information for hospitals to have access to.  For instance, people that have had skin cancers, asthma, diabetes, and kidney disease all had a higher risk of developing heart disease than those people who did not.  

### Future development

Looking at the future in terms of projects in heart disease our group would be interested in looking at other data sets that included more data that revolved around specific questions.  For instance, diet, physical locale, income, stress levels.  This data could also be compared or grouped with other data frames, such as pollution levels by geography.  We are sure that the depth of information that epidemiologists have gathered is already ahead of us, and we are looking forward to discovering these projects as we continue to learn.
  


**About our Data** 

* CDC Data<sup>2</sup>

> [Our CDC dataset](https://www.kaggle.com/datasets/kamilpytlak/personal-key-indicators-of-heart-disease) comes from kaggle as well. This is a partially cleaned dataset where he author has reduced the data points from over 300 to the 40 most applicable for heart disease.   [Here is a link to the repository of the original data and how it was cleaned](https://github.com/kamilpytlak/data-science-projects/blob/main/heart-disease-prediction/2022/notebooks/data_processing.ipynb)


**Licensing of Data**

* This specific sampling of the Framingham dataset has ambiguous licensing. The licensing when downloaded from kaggel is stated as 'unknown', full use of the Framingham dataset requires an application and approval of research.  The full data set covers a much larger dataset than the sampling we have accessed off kaggle.com.

* CDC dataset has CC0: Public Domain licensing

**References**

<sup>2</sup> CDC dataset was taken from https://www.kaggle.com/datasets/kamilpytlak/personal-key-indicators-of-heart-disease 

Unused Dataset
<sup>1</sup> This data set dates from 1988 and consists of four databases: Cleveland, Hungary, Switzerland, and Long Beach V. It contains 76 attributes, including the predicted attribute, but all published experiments refer to using a subset of 14 of them. The "target" field refers to the presence of heart disease in the patient. It is integer valued 0 = no disease and 1 = disease.
  -https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset?resource=download



