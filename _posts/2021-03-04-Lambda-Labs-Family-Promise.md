---
layout: post
title: Alleviating Homelessness with Data Science
subtitle: Model Building and Working on a Team
cover-img: /assets/img/fam_promise_banner.jpg
thumbnail-img: /assets/img/family-promise-of-spokane.jpg
share-img: /assets/img/family-promise-of-spokane.jpg
tags: [housing, classification]
---

The Family Promise of Spokane Organization is a US-based nonprofit organization based in Spokane, WA. They are an organization that helps homeless families as well as preventing families from becoming homeless. They provide shelter for families as well as rental assistance. My labs team developed a digital intake form for families and Family Promise Shelter employees. Currently, the institution is mainly paper-based, and digitization will result in increased efficiencies and valuable insights. ‘

Specifically, the team’s data scientists (myself included) built a multi-class random forest model that takes the guest data and predicts their exit destination. 

The possible Exit Destinations are as follows:

*  Permanent Exit
*  Temporary Exit
*  Emergency Shelter
*  Transitional Housing
*  Unknown/Other

The data science tasks included:

*  Creating a risk classifier metric and adding to the data
*  Creating data wrangling pipelines
*  Exploratory Data Analysis (EDA)
*  Creating feature matrices and target vectors for classification
*  Selecting a classification model type
*  Building a trained multi-class classification model
*  Constructing a modeling pipeline
*  Training the model
*  Hyperparameter tuning
*  Serializing / Pickling the model
*  Querying features from Postgres database
*  Returning output of trained model on ingested data
*  POST 'exit_destination' to API
*  AWS Deployment
*  Data Visualization 

Takeaways:

*  Communication between FE, BE, DS, UI teams are the key to success.

It’s cliche, but true. Tasks and workloads are simply not distributed equally across a project. Mid-way through week one, data scientists had built a working API and migrated dummy data. We also spun up a working model that outperformed the baseline. Then came the bottlenecks. We were not able to work with BE database engineers because they were completely focused on connecting with DocuSign’s API. This took weeks, while us data scientists were mainly idle, tweaking with the model and trying to feature engineer a few more points in accuracy. We (data science) were able to work with FE folks to incorporate visualizations on the dashboard, but it was difficult to self-evaluate because we were still waiting on BE for the correct data. 

**Key takeaway**: Data science is super interesting... But one individual could have easily done everything necessary for this project. Once you learn how to build and optimize model pipelines, python and its libraries do most of the work for you. As I navigate the job market, I imagine that I am competing against people with advanced degrees in statistics and/or computer science. I could spend hours talking about the intricacies of model techniques, why using a GRU in some cases is better than an LSTM, but businesses just want insights, and the difference between good enough and optimal is sometimes insignificant. The real need lies in data engineering, the less-sexy movement of data from one system or format to another system or format. Upon leaving Lambda, I am making an effort to bolster my data engineering skills, from mastering SQL to earning my Google Cloud, Microsoft Azure, and AWS certifications.

*  There’s a world of difference between starting a project from scratch and adopting an existing code base.

Getting acquainted with an unfamiliar tech stack takes time and patience. In this case, we had to first wrap our arms around the goals of the project (i.e. user stories) and then craft a strategy. From there, our team meticulously went through the existing code base’s architecture and components. We were unpleasantly surprised to find out there was no working API and the model performance was poor. With other data scientists on the team, we went through the jupyter notebooks and .py files in the repository and did housekeeping: what would we keep, what needed major changes, and where we needed to reinvent the wheel. 

*  Use-case matters

When all is said and done, our efforts will materially improve the lives of vulnerable communities. I have worked in government and nonprofit organizations before, and that’s always been a motivating factor— but being able to apply a more specialized skill like computer programming to a worthy cause is a different feeling entirely. 
