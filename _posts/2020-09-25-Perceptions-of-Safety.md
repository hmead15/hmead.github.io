---
layout: post
title: Is Colombia Safe?
subtitle: Perceptions of Public Safety in Colombia
cover-img: /assets/img/soccer pic.jpg
thumbnail-img: /assets/img/colombia-flag-02.jpg
share-img: /assets/img/colombia-flag-02.jpg
tags: [Colombia, public policy]
---

For my second build week project, I looked how Colombians view public safety and security. 

DANE is the entity responsible for the planning, collection, processing, analysis and dissemination of official statistics of Colombia. 
In 2016, they conducted their Coexistence and Citizen Security Survey (ECSC). I built a model which predicted whether respondents felt 'safe' or 'unsafe' in their neighborhood with 73 percent accuracy (nearly 80 percent accuracy when including features I deemed to be "leakage"). 

Early on and throughout the build week, I ran up against my own limitations as a data scientist often. My features were primarily binary (Yes/No), although many had relevant non-NaN third options (like: 'do not frequent this location') that I ended up dropping due to a need for simplicity. Both of my two models (RandomForestRegressor and LogisticRegression) did improve upon my baseline, and I credit the dataset I used, which included dozens of features that were easy to interpret and use for feature engineering. 

But overall, I am struck with how difficult and time consuming data science can be. I compromised my data by dropping rows in the name of simplicity and I over-simplified features. In terms of interpretation, I felt like I was 'going through the motions', and followed closely with lecture notes, rather than deploying a commanding knowledge of the material. I tried to build a plotly dash app, but ended up stumping Team Leads and the Instructor, and abandoned it. I am happy that I ended up with a finished project, but humbled by the journey. 

My Build Week II findings are explained in detail [here](https://medium.com/@henrymead/perceptions-of-safety-in-colombia-c0137325c20e).

My jupyter notebook ipnyb file can be found [here](https://github.com/hmead15/Build-Week-2/blob/master/Build%20Week%20Two%20final.ipynb). 
