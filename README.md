# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 4: Group Project

## Team

1. Andy Deemer
2. Larry Jackelen
3. Saba Suhail
4. Vilo Avilo

## Contents

- [Problem Statement](#Problem-Statement)
- [Data](#The-Data)
- [Notebook Descriptions](#Notebook-Descriptions)
- [Conclusions and Recommendations](#Conclusions-and-Recommendations)
- [Future Enhancements](#Future-Enhancements)
- [Data Dictionary](#Data-Dictionary)
- [Executive Summary](#Executive-Summary)
- [References](#References)

## Problem Statement 

We are meeting with key members of the staff of John Kerry - Special Presidential Envoy for Climate - to discuss the characteristics of the nation in the context of their belief in global warming
Leveraging their internal marketing and public service announcement capabilities, they want to know the types of people they should investigate further for reaching out to. 
A major boon will be to convince persons that don’t believe global warming is happening otherwise.

**What types of characteristics and features have the largest effect on whether or not a person believes global warming is happening?**

## The Data

Data was downloaded from the [Yale Program on Climate Change Communication](https://climatecommunication.yale.edu/visualizations-data/ycom-us/). We cleaned the data by dropping persons who refused to answer 5 or more questions. Categorical features were either dummified or ordinal encoded. The 80 features were reduced to 20 through feature selection using SelectKBest() and the 60 other features were reduced to 5 PCA variables to account for noise. The dataset was train-test split, the null values were iteratively imputed, and the dataset was standard scaled. This left us with 25 features for modeling.


## Notebook Descriptions

1. 01_EDA.ipynb : Carried out EDA in this notebook
2. 02_Preprocessing.ipynb : Carried out preprocessing in this notebook
3. 03a_Modeling_logistic_regression.ipynb : Modeled logistic regression algorithm on the processed data in this notebook
4. 03b_Modeling_SVM_model.ipynb : Modeled SVM algorithm on processed data in this notebook
5. 03c_Modeling_Ensemble.ipynb : Modeled ensemble algorithms on the processed data in this notebook. Our Production Model.


**Software Recommendations**
Pandas, Sci-Kit Learn, Numpy, MatPlotLib, Seaborn

## Conclusions and Recommendations

Conclusions:
-  For our best model we found that many of the questions that were asked relating to whether or not global warming may be harmful were most important for predicting our target. This holds true for our logistic regression model as it shared many of the same features
-  This may come as no surprise but we found there to be a strong divide in belief in climate change based on political affiliation and even wider still depending on the ideology.
-  Education level plays an important factor. The more educated a person is the more likely they are to believe in climate change. 
-  Age can be a factor however small. The older generations seem to not believe in climate change as much as the more recent ones. 
-  People who believe in climate change have fewer or no children at all.
-  More religious people are more likely to not believe in climate change.

Recommendations:
- Recommend media that helps friends and family to learn about climate change more tangibly. It will make them worried. HBO should probably be telecasting “Our World” and “Before the Flood” more often.
- Speak to people in a language they understand- popular leaders,actors, famous scientists etc. Make climate awareness a compulsory subject in schools
- Highlight the heatwaves in US and Canada in social media
- Have climate change be taught in schools from an early age
- Convince people to change their political views
- Incorporate climate change programme in service attendance and old age homes
- Most people are worried about the effects of climate change, even if they say they don’t believe in it or don’t know. Based on this fact, we recommend focusing on showing the current natural disasters that are directly caused by global warming. These events directly impact the US population, more so in certain high risk areas like floodplains and hurricane prone environments. 
- There’s a large discrepancy in people’s idea of why global warming is happening (by humans, natural, or both). Many people that don’t believe in global warming or don’t know still say it’s caused by humans. The scientific community all believe it is caused by humans. We recommend addressing this discrepancy in lessons and public discussions. 

## Future Enhancements
The analysis can be further improved by:
-  More feature creation and consolidation, especially with the Harm series of questions
-  Imputing Nulls and Refused separately rather than together. This will capture signal separately for people not being served a question versus refusing to answer the question.
-  Leveraging the wave weight and weight aggregate in the analysis. This will allow the findings to be more generalizable toward the United States population as a whole, rather than just similar demographic populations

## Data Dictionary

The data dictionary can be found [here](https://git.generalassemb.ly/ljackelen/project_4/blob/master/data/Project4_Data_Dictionary.pdf)




## Executive Summary

Our nation is divided on whether or not global warming is happening; all while the planet burns. The Paris Climate Agreement was met with global participation; however, the withdrawal of the United States did not receive national condemnation, further showing this division. The United States is now back in the Paris Climate Agreement, but it is still not politically costly to withdraw in the future. The country’s view needs to change.

This is not a new problem for John Kerry – Special Presidential Envoy for Climate – and his staff. Understanding the characteristics of the nation in the context of their belief in global warming is critical. It is critical for developing leads on who to do more targeted research on in order to leverage their internal marketing and public service announcement capabilities. It is crucial for getting to the final goal of convincing people global warming is happening and that it is time to act.

The Yale Program on Climate Change has been at the forefront of collecting and analyzing survey data on global warming in the nation. From 2008 through 2018, they have gather over 20,000 survey responses from across the country spanning all manners of religion, race, gender, age, and income. As part of their mission, having this survey data available to the public allows us to find additional insights.

The target question we wanted to model and explore was: Do you think that global warming is happening? The possible answers being Yes, No, Don’t Know, and Refused. The Refused were immediately dropped from the dataset for this analysis.

Utilizing the survey data, features were extracted and cleaned. A major issue was people who refused to answer other questions. They were treated as missing data in this analysis for their lack of participation. These and other missing data were imputed based on their other responses relative to the dataset. Starting with 80 features, the top 20 most important were kept and the other 60 condensed into 5 noise variables for modeling.

Three approaches were taken for modeling with the ultimate goal being to classify a survey respondent’s answer to the target question. Logistic Regression, Support Vector Machines (SVM), and Random Forest Classifier (RFC) were analyzed. Ultimately, the strongest performing model was RFC with a model score of 79%.

Logistic Regression and SVM scored very well also, but for modeling future respondents, RFC is the production model.

Insights were able to be gathered from modeling that indicate the major things to focus on and explore for our problem are:
-	Emphasizing the scientific consensus on the issue
-	Highlighting how it is harming the world and the United States today … not in the future
-	Allowing people’s worry on the issue to translate into public response and action, rather than despair, alienation, and inaction.

This model is just the stepping stone and can be further improved through more feature creation and consolidation, but also with more surveys to get a more accurate gauge on where the country is now. Global warming is here and is a huge issue, the communication strategy needs to match the urgency.

## References

https://fivethirtyeight.com/features/how-you-view-climate-change-might-depend-on-where-you-live/

https://climatecommunication.yale.edu/visualizations-data/ycom-us/
