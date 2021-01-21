# AB-test-analysis
This project aim to use regression analysis to analyze a AB test result from an online store company.

## Table of Contents
- [Introduction](#intro)
- [Datasets](#data)
- [Analysis](#analysis)
- [Conclusions](#conclusions)
- [License](#license)
- [Contact](#contact)

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

#### Probability
In this part, the `ab_data.csv` was cleaned. After cleaning some probabilities were calculated. The probabilities calculated include:
- Probability of a user being in either of the groups (control or treatment).
- Probability that a user converted regardless of their landing page.
- Probability that a user converted when in either group.

#### A/B Test.
The A/B test section was where the null and alternative hypothesis was stated, other things like
- The probability of conversion under the null, P_new.
- Simulation of n-transactions with a conversion rate of P_new.
- The p-value
were calculated. The decision whether to reject or fail to reject the hypothesis was decided.

#### Regression.
In this part, a logistic regression approach was used to check for the p-value. Also in this section, countries from `country.csv` were added to the variable to decide if a user converted based on where users logged in from. 

<a id='conclusions'></a>
### Conclusions
The conclusion reached based on the analysis was given stating why it was so.

<a id='license'></a>
### License
This analysis is done under an [ Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0) license.](https://creativecommons.org/licenses/by-nc-sa/4.0/)

<a id='contact'></a>
### Contact
For more details, you can [mail me](mailto:ola.ia1523@gmail.com).
