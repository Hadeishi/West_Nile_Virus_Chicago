# West Nile Virus Predictor

## Introduction

This project was completed by the mythical Disease And Treatment Agency, division of Societal Cures In Epidemiology and New Creative Engineering (DATA-SCIENCE) team, Max Reinisch, Adam Del Real, Bing Chen, and myself.

Due to the recent epidemic of West Nile Virus in the Windy City, the Department of Public Health set up a surveillance and control system. We're hoping it will let us learn something from the mosquito population as we collect data over time. Pesticides are a necessary evil in the fight for public health and safety, not to mention expensive! We need to derive an effective plan to deploy pesticides throughout the city, and that's where our team came in!

## Dataset

The dataset, along with description, was downloaded from [this site:](https://www.kaggle.com/c/predict-west-nile-virus/). Data was collected between 2006 and 2010 in Chicago, Illinois. It contained counts of mosquitos trapped throughout Chicago and whether or not these mosquitos tested positive for West Nile virus (see [this notebook](https://github.com/Hadeishi/DSI_Project_4/blob/master/West-Nile-Virus.ipynb) as well as weather data measured at both Chicago airports over the same time period. Using these data, we were to develop a model to predict where and when West Nile positive mosquitos would occur over two years when we were not supplied with this target. We could check the predictions made by our models against reality by sending them in to kaggle and receiving feedback up to 5 times per day so we could iteratively improve our models.

## Exploratory Data Analysis

Each team member participated in the EDA process, contributing our unique talents to the project. My background in biology and pharmacology and came in handy researching mosquito species and instability of the insecticide, as well as looking into the underlying physics of weather forecasting. Others in our group took on different challenges. Our independent EDA is collected in jupyter notebooks in the Master folder. You can get to these folders by clickling [here]().

## Modeling

1. The goal is of course to build a model and make predictions that the city of Chicago can use when it decides where to spray pesticides! Your team should have a clean Jupyter Notebook that shows your EDA process, your modeling and predictions.
2. Conduct a cost-benefit analysis. This should include annual cost projections for various levels of pesticide coverage (cost) and the effect of these various levels of pesticide coverage (benefit). *(Hint: How would we quantify the benefit of pesticide spraying? To get "maximum benefit," what does that look like and how much does that cost? What if we cover less and therefore get a lower level of benefit?)*
3. Your final submission CSV should be in your GitHub repo.

**Presentation**
* Audience: You are presenting to members of the CDC. Some members of the audience will be biostatisticians and epidemiologists who will understand your models and metrics and will want more information. Others will be decision-makers, focusing almost exclusively on your cost-benefit analysis. Your job is to convince both groups of the best course of action in the same meeting and be able to answer questions that either group may ask.
* The length of your presentation should be about 20 minutes (a rough guideline: 2 minute intro, 10 minutes on model, 5 minutes on cost-benefit analysis, 3 minute recommendations/conclusion).  Touch base with your local instructor... er, manager... for specific logistic requirements!

We submitted our predictions to the Kaggle site to see how we could improve our models.The public leaderboard uses roughly 30% of the dataset to score an AUC (Area Under Curve) metric. Click [here](https://www.kaggle.com/wiki/AreaUnderCurve) to read more about this scoring metric. We could submit predictions as many times as you liked to Kaggle, but there was a limit of 5 submissions per day.

***Num Mosquitos*** Upon further reflection, we decided it may not be statistically justifiable using our data to interpolate the number of mosquitos and then using these interpolated data to further predict where West Nile positive mosquitos might be in the future, so we gave up on this aspect of the project. Nevertheless, this mosquito predictor might be a valuable side project independent of the West Nile Virus predictor. For instance, it may be that a different mosquito-borne infectious disease may strike Chicago in the future such as Zika or Chikungunya.

---

**Your project is due at 10:00 AM EST/9:00 AM CST on Friday, June 15.**

---

### Project Feedback + Evaluation

Data science is a field in which we apply data to solve real-world problems. Therefore, projects and presentations are means by which we can assess your ability to solve real-world problems in a data-driven manner.

Your final assessment ("grade," if you will) will be calculated based on a [topical rubric](https://docs.google.com/spreadsheets/d/1V6OzSHPXCJEe_sVT7B1vE7sT-jqNMNo-NrmZHtafMXY/edit?usp=sharing). For each category, you will receive a score of 0-3. From the rubric you can see descriptions of each score and what is needed to attain those scores. Make sure you look at the "Rubric P4" tab of the [spreadsheet](https://docs.google.com/spreadsheets/d/1V6OzSHPXCJEe_sVT7B1vE7sT-jqNMNo-NrmZHtafMXY/edit?usp=sharing).
# West_Nile_Virus_Chicago
