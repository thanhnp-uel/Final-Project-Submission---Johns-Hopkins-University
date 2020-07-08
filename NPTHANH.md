Final Project Submission -  Johns Hopkins University
========================================================
author: Ngo Phu Thanh 
date: 08/07/2020
autosize: true

Introduction
========================================================
-     The goal of this exercise is to create a product to highlight 
the prediction algorithm that we have built and to provide an 
interface that can be accessed by others
-     For this project you must submit:
1. A Shiny app that takes as input a phrase (multiple words) in a 
text box input and outputs a prediction of the next word. 
To see the shiny app, go here: https://ngophuthanh.shinyapps.io/FinalProjectSubmission-NPTHANH/
2. A presentation consisting of no more than 5 slides created with R Studio Presenter pitching my algorithm and app as if i'm presenting to your boss or an investor.

Summary of Project Steps
========================================================
*. Loading Libraries: First step of the project is to load all the libraries necessary to complete all the tasks outlined in the introduction.

*. Loading Data: The data used in this project can be found https://github.com/piotrpio2017/Peer-graded-Assignment-Final-Project-Submission

*. Summarizing Data Files: create a very basic overview of the data file statistics in terms of File Names, File Sizes, Number of Rows in each file as well as word count. Creating a Data Sample - 1000 lines from each file were sampled. Total sample size will be 2000.

*. Cleaning Data: Convert all text to lowercase, remove all punctuation, numbers, whitespace and "english" stop words.

*. Creating the corresponding n-gram frequencies Saving n-grams as .rds files

Algorimth
========================================================

- N-gram model used ( from 1 to 4 n-gram )

- If no match is found in any of the 4 n-grams, the algorimth indicates that the sample is too small.

- Stupid back-off strategy implemended.

- Important: Sample size was limited to 2000 due to relatively small processing power of the pc that was used

Shiny App - How it works
========================================================

*. User inputs a word into the app interface

*. The app then checks the word against the prediction algorithm

*. The next word is proactively predicted

*. This prediction is based from longerst to shortest N-gram frequency

*. Prediction is displayed

Thank you for see my presentation.
