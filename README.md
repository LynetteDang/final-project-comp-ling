# Final Project for Computational Linguistics
Authors: Lynette Dang, Pranathi Iyer

## Introduction

How well do models perform on classification tasks when they are trained on larger data, but deployed on much sparser/smaller data from a completely different source but in a similar domain? How does it compare to the per-formance from an existing pretrained model? From an industry classification case study, the authors build on previous literature and use two different types of pre-trained models to improve the performance of text classifiers on sparse data. This paper highlights the advantages, limitations, and potential pitfalls of different pre-trained models, contributes to the growing body of literature of low-resource text classification, and helps practitioners and researchers to tackle relevant challenges more effectively
 
## Dependency

The code and data in this repository is an example of a reproducible research workflow for my MACS 30200 "Perspectives on Computational Research" project.

Most of the code is written in Python 3.11.2 and all of its dependencies can be installed by running the following in the terminal (with the `requirements.txt` file included in this repository):

```
pip install -r requirements.txt
```
## Data

1. Alumni Data: This dataset contains pre-processed information about alumni's past job experiences in three columns - company, position, and job description. The dataset has been created by scraping and verifying data using Python, Selenium, Google API, and LinkedIn. Each observation in the dataset has been assigned an industry type out of ten pre-designed categories, including Business/Finance, Charity/Volunteering, Consulting, Education/Research, Healthcare, Human Resources, Law, Policy/Government/Social Work, Technology, and Others. The purpose of the dataset is to test classifiers and evaluate their performance.

2. [Kaggle UK Job Data](https://www.kaggle.com/code/chadalee/text-analytics-explained-job-description-data): This dataset contains approximately 240,000 observations from job posts by companies in the UK and will be used to pretrain logistic regression and naive bayes classifiers. The dataset was originally used in a competition by Adzuna to predict salaries for jobs based on various attributes, including industry type, company, position, and job description.

3. [Indian Job DistilBERT Data](https://nlp.johnsnowlabs.com/2021/11/21/distilbert_sequence_classifier_industry_en.html): This dataset consists of 7,000 samples of business descriptions from companies in India and was utilized to pre-train DistilBERT model. It classify these descriptions into one of 62 industry tags.

## Content
1. [cleanup.ipynb](https://github.com/LynetteDang/final-project-comp-ling/blob/main/cleanup.ipynb) and [text_processing.ipynb](https://github.com/LynetteDang/final-project-comp-ling/blob/main/text_processing.ipynb): clean up the messy and unstructured scraped result from Linkedin, group each observation into education or experience, sort data into attributes such as position, company, and description
2. [industry_analysis_combined.ipynb](https://github.com/LynetteDang/final-project-comp-ling/blob/main/industry_analysis_combined.ipynb): logistic regression classifier training, fitting, and performance evaluation/pre-trained DistilBERT model fitting, and performance evaluation
