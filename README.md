# West Nile Virus Predictor

## Introduction

This project was completed by the mythical Disease And Treatment Agency, division of Societal Cures In Epidemiology and New Creative Engineering (DATA-SCIENCE) team, Max Reinisch, Adam Del Real, Bing Chen, and myself.

Due to the recent epidemic of West Nile Virus in the Windy City, the Department of Public Health set up a surveillance and control system. We're hoping it will let us learn something from the mosquito population as we collect data over time. Pesticides are a necessary evil in the fight for public health and safety, not to mention expensive! We need to derive an effective plan to deploy pesticides throughout the city, and that's where our team came in!

## Dataset

The dataset, along with description, was downloaded from [this site](https://www.kaggle.com/c/predict-west-nile-virus/). Data was collected between 2006 and 2010 in Chicago, Illinois. It contained counts of mosquitos trapped throughout Chicago and whether or not these mosquitos tested positive for West Nile virus (see [this notebook](https://github.com/Hadeishi/DSI_Project_4/blob/master/West-Nile-Virus.ipynb) as well as weather data measured at both Chicago airports over the same time period. Using these data, we were to develop a model to predict where and when West Nile positive mosquitos would occur over two years when we were not supplied with this target. We could check the predictions made by our models against reality by sending them in to kaggle and receiving feedback up to 5 times per day so we could iteratively improve our models.

## Exploratory Data Analysis

Each team member participated in the EDA process, contributing our unique talents to the project. My background in biology and pharmacology and came in handy researching mosquito species and instability of the insecticide, as well as looking into the underlying physics of weather forecasting. Others in our group took on different challenges. Our independent EDA is collected in jupyter notebooks in the Master folder. You can get to these folders by clickling [here](https://github.com/Hadeishi/West_Nile_Virus_Chicago/tree/master/Notebooks-WIP). The best EDA, created by Max Reinisch,

## Modeling

1. We built a number of models, the best of which and make predictions that the city of Chicago can use when it decides where to spray pesticides. Each member of our team made Jupyter Notebooks that shows our EDA process, our modeling, and predictions.
2. Our final model was a neural net and can be found [here](https://github.com/Hadeishi/West_Nile_Virus_Chicago/blob/master/Notebooks-Master/04_Build_Models.ipynb).

**Presentation**
We also created a presentation aimed at biostatisticians and epidemiologists who understand our models and metrics and will want more information as well as decision-makers, who will be focused almost exclusively on our cost-benefit analysis.

We submitted our predictions to the Kaggle site to see how we could improve our models. The public leaderboard uses roughly 30% of the dataset to score an AUC (Area Under Curve) metric, in common usage in data science and other circles to compare binary classification models; [click here](https://www.kaggle.com/wiki/AreaUnderCurve) to read more about this scoring metric. We could submit predictions as many times as we liked to Kaggle, but there was a limit of 5 submissions per day.

One of the major reasons why AUC (or ROC-AUC) scores are used so frequently in data science circles is that once a model has been created trying to maximize the area under the curve, the threshold probability can be selected so as to maximize sensitivity or specificity as required. If we had access to a huge amount of relatively inexpensive bug spray, for example, we might be inclined to maximize sensitivity over specificity when it came to our modeling. However, if we needed to conserve our bug spray, then we might be inclined to raise our threshold probability so that our model is more specific in making its predictions.

***Num Mosquitos*** Upon further reflection, we decided it may not be statistically justifiable using our data to interpolate the number of mosquitos and then using these interpolated data to further predict where West Nile positive mosquitos might be in the future without spending considerbly more time on statistical manipulation, so we gave up on this aspect of the project. Nevertheless, this mosquito predictor may prove to be a valuable side project independent of the West Nile Virus predictor. For instance, it may be that a different mosquito-borne infectious disease may strike Chicago in the future such as Zika or Chikungunya and we would need to track a different sub-species of mosquito in the Chicago area to defeat this distinct plague.
