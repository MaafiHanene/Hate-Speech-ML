# Hate Speech ML

This project is an attempt to write a text classifier that can automatically detect hate speech, which will have potential applications in forum moderation and filtering on social media feeds. The project was originally conceived as part of a course project for [Brandeis CS140 (*Natural Language Annotation for Machine Learning*)](http://www.cs140.org/), and was continued by Annie Thorburn as a personal project. The text corpus that is used to train and test the classifier was developed in that course by Anna Astori, Annie Thorburn, Jose Andres Molina, and Jake Freyer.

# Contents

*GoldStandards:* This folder contains the XML files containing the text corpus. The text in this corpus was collected from Twitter, and was annotated using [MAE](http://keighrim.github.io/mae-annotation/). Each file contains a set of tweets, along with XML tags representing annotations. \[*CONTENT WARNING:* Because the goal of this project is to train an algorithm to identify and filter out hate speech, the text corpus contains many examples of said hate speech, including racism, sexism, ableism, homophobia, transphobia, anti-immigrant rhetoric, body-shaming, religious intolerance, and other general nastiness. *Caveat lector.*\]

*HS_classifer.py:* A Python program to extract the data from the files in the GoldStandards folder and use it to train and test two naive Bayesian classifiers. The first is a simple classifier that uses as features all of the words in the text; this is meant to serve as a baseline against which other classifiers can be evaluated. The second classifier uses the annotations to determine which words should be considered as features.
