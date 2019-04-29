# Project Title : Match-A-Quote

# Description
Given a quote, find a picture which best matches the quote.

# Abstract

We come across a lot of quotes throughout the day. They are motivating and inspirational but most of them are dull in background on plain text. What if we want an appropriate picture behind it? Our Project finds the best suitable picture for the given quote.

# Implementation Timeline (Proposed)

 - <b> Week 1: 18-25 March (Image and Quote Collection for DataSet Creation and Analysis) </b>
  We propose to collect free images available on the internet and quotes and categorize them acccording to suitable tags which will help in matching the quotes to the images.
 - <b> Week 2: 26-2 April (Discussion on suitable Algorithms for the project) </b>
  Give the quotes and images limited categories along with tags which will help in efficient matching.
 - <b> Week 3: 3-10 April (Implementation of Algorithm) </b>
  Implementation and testing the algorithm and modifying dataset accordingly.
 - <b> Week 4: 11-18 April (Testing and Results Output) </b>
  Testing the algorithm on new unseen quotes.
- <b> Last Week (Bug Fixes, Reports and Presentation) </b>
  Final testing and bug fixing, Report and presentation making.

# About the DataSet

The dataset consists of 2 parts:
- Quotes (Categories, Quote, Tags)
    - Downlaoded the raw dataset from [https://www.kaggle.com/akmittal/quotes-dataset]
    - Filtered 30-40 quotes from each category.
    - Re-Tagged the quotes manually to make the dataset according to the project.
- Images (Categories, Image Name, Tags)
    - Downlaoded the images from the free sources on internet.
    - Divided them into proper categories.
    - Suitable description of images by giving tags.
Categories: A broad umbrella which defines a quote or image. The given categories are as follows:
    - Motivation
    - Wisdom
    - Truth
    - Arts
    - Books
    - Death
    - Faith
    - God
    - Happiness
    - Hope
    - Inspiration
    - Science
    - Soul
    - Writing
    - Positive
    - Philosophy
    - Mind
    - Friendship
    - Life
    - Love
    - Success
Tags: Specific details and emotions from the image or quote which particularly expresses it. Some examples are: person, smile, sadness, climb, believe etc.

# Approach

- Match-A-Quote Algorithm
    - Matching the given categories of quote along with category of images and giving each match a score of 5. Storing it in score1.
    - Matching the given tags of a quote along with tags of images and giving each match a score of 1. Storing it in score2.
    - Matching Score = score1 + score2
    - Conditional checking and making sure that the image belongs to the category matched.
    - Matching Cases
        - Strict Matching Case: if score1 >= 5 and score2 > 0.
        - Loose Matching Case: if matchingScore > 0
    - Returing the matched image results.
- Sorting the results of the Match-A-Quote Algorithm and picking up the top 3 results.
- Displaying the details of the quote and images matched along with matched tags and categories.
- Displaying the images inline for a better user experience.

# Team members

- Kishan Shankar Singhal (2018201023)
- Rajat Dua (2018201066)
- Nawab Alam (2018201030)
- Shashi Jangra (2018202001)

# Contribution of team members

- Quotes DataSet Collection : (Nawab, Shashi)
    - collecting quotes online
    - Clubbing repetitive quotes together into multiple categories
- Images DataSet Collection : (Kishan, Rajat)
    - Downloading images online categories wise.
- Quotes Filtering and visualisation : (Nawab, Kishan, Shashi) 
    - Removing miss attributed tags
    - Giving manual categories and tags
    - Removing stem words from tags
    - Filtering more quotes on each category to create an equally distributed dataset.
- Images Filtering : (Kishan, Rajat)
    - Giving them suitable categories and tags
    - Generating a csv file for all images
- Algorithm : (Nawab, Shashi, Rajat)
    - Giving separate scores on the basis of category match and tag match
    - Removing all the images which gave score=0
    - Sorting images based on scores
- DataSet Improvisation : (Kishan, Rajat, Nawab)
    - Adding more required tags to quotes and images by testing the algorithm on filtered categories.

# DataSet Links
- [Quotes DataSet](https://drive.google.com/drive/folders/1M5yTSxumOPSAOI4phHEduZYaKiG4QuR3?usp=sharing)
- [Images DataSet](https://drive.google.com/drive/folders/1YGsDNrBXy3ZXQYUYFphUGgmgoUtfTq-0?usp=sharing)

# Repository Link 

[https://github.com/shashijangra22/Match-A-Quote](https://github.com/shashijangra22/Match-A-Quote)
