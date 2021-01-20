# AB-test-analysis
This project aim to use regression analysis to analyze a AB test result from an online store company.

## Table of Contents
- [Introduction](#intro)
- [Datasets](#data)
- [Analysis](#analysis)
- [Conclusions](#conclusions)
- [License](#license)

<a id='intro'></a>
### Introduction
The project was carried out as part of the requirement to completing [Udacity's Data Analyst course](https://www.udacity.com/course/data-analyst-nanodegree--nd002).
The assumption made was that an e-commerce company carried out an A/B test on its website between two landing pages, and as the in-house Data Analyst, I'm to analyze it and suggest which landing page the company is to adopt.

<a id='data'></a>
### Datasets
Two datasets were provided for the analysis.
##### ab_test.csv
This dataset contains the A/B test results from different users id. It contains **5 columns** and **290584 unique rows**.
- `user_id`: User id of the users
- `timestamp`: Time and date the user visited the website
- `group`: The group a user belongs to in the A/B test: **control**, whose members were shown the old landing page or **treatment**, whose members were shown the new landing page.
- `landing_page`: The landing page a user was shown, either old or new.
- `converted`: This indicates if a user was converted to a customer or not. 0 means no, 1 means yes.
##### countries.csv
This dataset contains the countries the user accessed the website. It contains two columns, `**user_id**` and `country`. It also contains **290584 unique rows**.

<a id='analysis'></a>
### Analysis
The analysis was carried out in three parts
- Probability
- A/B Test
- Regression
