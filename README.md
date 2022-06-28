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
- [Modeling and Preprocessing](#Modeling-and-Preprocessing)
- [Data Dictionary](#Data-Dictionary)
- [Executive Summary](#Executive-Summary)

## Problem Statement 

We are meeting with key members of the staff of John Kerry - Special Presidential Envoy for Climate - to discuss the characteristics of the nation in the context of their belief in global warming
Leveraging their internal marketing and public service announcement capabilities, they want to know the types of people they should investigate further for reaching out to. 
A major boon will be to convince persons that don’t believe global warming is happening otherwise.

**What types of characteristics and features have the largest effect on whether or not a person believes global warming is happening?**

## The Data

We used the following dataset available on the website of Yale climate communication website.The link to it can be found [here](https://climatecommunication.yale.edu/visualizations-data/ycom-us/) 

## Notebook Descriptions

1. 01_EDA.ipynb : Carried out EDA in this notebook
2. 02_Preprocessing.ipynb : Carried out preprocessing in this notebook
3. 03a_Modeling_logistic_regression.ipynb : Modeled logistic regression algorithm on the processed data in this notebook
4. 03b_Modeling_SVM_model.ipynb : Modeled SVM algorithm on processed data in this notebook
5. 03c_Modeling_Ensemble.ipynb : Modeled ensemble algorithms on the processed data in this notebook. Our Production Model.

## Modeling and Preprocessing

We cleaned the data in following steps:
1. Dummified data
2. Made ordinal labels for ordinal columns
3. Standard Scaled
4. Selected 20 best features using SelectKBest()
4. PCA to further get 5 variables into account for noise

## Data Dictionary

The data dictionary can be found [here](https://git.generalassemb.ly/ljackelen/project_4/blob/master/data/Project4_Data_Dictionary.pdf)



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


## Executive Summary

Not all stakeholders are aware of their vulnerability to climate change and the steps they might take to proactively adapt to it. Therefore, increasing public awareness is crucial to managing the effects of climate change, improving adaptive capacity, and lowering overall risk. The goal of raising public awareness is to increase passion and support, inspire self-motivation and action, and mobilize local expertise and resources. As critical players in the process of adjusting policy, politicians and policy makers, raising political awareness is crucial. 

To achieve the desired result, communication tactics that are effective are needed while raising awareness. The combination of various communication tactics targeting a specific audience over a set length of time can be widely referred to as a "awareness raising campaign." Although the objectives of awareness-raising campaigns frequently vary depending on the environment, they typically involve raising awareness, educating the intended audience, fostering a favorable perception, and making an effort to influence their behavior.

Research demonstrates that awareness levels change throughout time under the effect of external factors, despite the fact that increased consciousness is frequently thought to be crucial during the early phases of the adaptation process. In contrast, the 2011–2010 cold winters in Europe, the minor IPCC errors, and the CRU (Climate Research Unit) emails have negatively impacted public acceptance of climate change and increased public skepticism. As an example, the Al Gore film "An Inconvenient Truth" (2006) and the IPCC Nobel Peace Prize have a positive effect on the public awareness. Raising awareness is therefore essential to maintaining and raising the overall level of awareness throughout the process, not only in the early phases.

Campaigns to raise awareness can target the general public, stakeholder groups, communities affected by a specific climate issue, etc. Such programs' ultimate goal is to bring about long-lasting behavioral changes. Raising awareness aims to increase people's and organizations' knowledge. It attempts to make sure that all pertinent regional and subregional bodies are aware of the effects of specific climate changes and are acting to address them. However, they can also concentrate on a specific effect that is thought to be the most significant, such as The Netherlands' "Live with Water." Such campaigns are typically deemed successful if multiple communication channels are utilized, including the distribution of printed materials, the organization of public training sessions and meetings, professional consultation, communication and information through social and mass media, and the use of informal networks for the spread of information. Of reduce the risk to human safety and property damage, for example during a flood event, it can be supplemented with the creation of community self-protection teams that encourage self-reliance among people and companies.

## References

https://fivethirtyeight.com/features/how-you-view-climate-change-might-depend-on-where-you-live/
