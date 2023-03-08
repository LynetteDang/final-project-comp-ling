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
## Content
1. `cleanup.ipynb`[https://github.com/LynetteDang/final-project-comp-ling/blob/main/cleanup.ipynb] and `text_processing.ipynb`[https://github.com/LynetteDang/final-project-comp-ling/blob/main/text_processing.ipynb]: clean up the messy and unstructured scraped result from Linkedin, group each observation into education or experience, sort data into attributes such as position, company, and description
2. `cleanup.ipynb`[https://github.com/LynetteDang/final-project-comp-ling/blob/main/cleanup.ipynb]: clean up the messy and unstructured scraped result from Linkedin, group each observation into education or experience
3. `TestEmailModule` for the email submission utility class `SendGridEmail`. 
4.  a `data` folder that contains a list of test data, including multiple pdf attachments for email submissions and a json file with coordinates for reverse geocoder. 
