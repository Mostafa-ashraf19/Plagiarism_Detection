# Plagiarism Detection
  - plagiarism detector following this [**paper**](https://github.com/Mostafa-ashraf19/Plagiarism_Detection/blob/main/Paper/developing-a-corpus-of-plagiarised-short-answers.pdf) that examines a text file and performs binary classification; labeling that file as either plagiarized or not, depending on how similar the text file is to a provided source text.

  <p align="center">
  <img width="460" height="300" src="https://github.com/Mostafa-ashraf19/Plagiarism_Detection/blob/main/assets/screen-shot-2019-02-28-at-2.59.48-pm.png?raw=true">
</p>

----- 

## Problem Statment and Analysis
  - Plagiarism is defined as “the appropriation of another person's ideas, processes, results, or words without giving appropriate credit”, so our goal here to try to find a solution for this by using some comparing between original and target text after making some preprocessing techniques for text before fitting it into Machine learning model to classify this model is plagiarized or not, according to the paper mentioned above will try to make some text processing after calculating containment and longest common subsequence using dynamic programming algorithm.
      <p align="center">
      <img width="460" height="300" src="https://github.com/Mostafa-ashraf19/Plagiarism_Detection/blob/main/assets/features%20.png?raw=true">
      <p align="center">Created features.</p>
       </p>
  - before we prepare our final dataset I'm made multiple features using multiple N-gram with containment and longest common subsequence, then try to calculate a correlation matrix to ignore very high correlated columns
  <p align="center">
  <img width="460" height="300" src="https://github.com/Mostafa-ashraf19/Plagiarism_Detection/blob/main/assets/correlation%20matrix.png?raw=true">
  <p align="center">Correlation Matrix.</p>
</p>

## DataSet  
  - This data is a slightly modified version of a dataset created by Paul Clough (Information Studies) and Mark Stevenson (Computer Science), at the University of Sheffield. You can read all about the data collection and corpus, [at their university webpage](https://ir.shef.ac.uk/cloughie/resources/plagiarism_corpus.html)
> **Citation for data:** Clough, P. and Stevenson, M. Developing A Corpus of Plagiarised Short Answers, Language Resources and Evaluation: Special Issue on Plagiarism and Authorship Analysis,


## Project Flow

  - Data Exploration 

  - Defining Features

  - Train and Deploy Model into AWS SageMaker
