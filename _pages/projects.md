---
permalink: /projects/
title: "Projects"
author_profile: true
redirect_from: 
  - /projects.html
  - /project
---

<p class="panel-success" markdown="1"><i class="fas fa-comment-dots"></i> **READ:** This is a list of some of the projects I've done. *Recently, most of the projects I've undertaken have either been research-based or company-based projects, and thus haven't been included here due to obvious reasons.* The research projects that have been completed and led to publications are residing in a separate category ([publications](/publications){:target="_blank"}). Some of listed the projects were done as self-projects to either *tackle real-world problems* or to *learn and experiment with new tools and technologies.* The other projects were done as a part of some of the courses ([info](/courses){:target="_blank"}) I've taken at IIIT-Delhi. I've added links to the demo/website, code and a blog post describing the project in detail wherever applicable.</p>

## Table of Contents

- TOC
{:toc}

## <i class="fas fa-chart-line"></i> TrenDetect 
* **Links:** [[`website`](http://www.trendetect.ml/){:target="_blank"}, [`code`](https://github.com/rg089/TrenDetect){:target="_blank"}, [`blog`](/posts/trendetect){:target="_blank"}]
* **Description**: A source to keep up with all the trending news topics, in an instant.
* **Type:** *Self-Project*  
* **Duration**: Jun'21 - Sep'21  
* **Work**:
    * Detection of trending keywords based on custom designed metrics 
    * Clustered keywords into six different categories
    * Created a connection graph to aid in the visualization of connections with relevance-based vertex and edge sizes
    * Utilized weighted heuristics like source credibility, time since publishing etc. on top of NER to assign weights to the keywords
    * Employed the [Newsemble](/projects/#-newsemble) API for collecting the news data

## <i class="fas fa-newspaper"></i> NewsHelper 
* **Links:** [[`demo`](https://huggingface.co/spaces/rg089/NewsHelper){:target="_blank"}]  
* **Description**: Automated summary and headline generation as well as source classification for news articles, specifically designed for Indian news.
* **Type:** *CSE556:Natural Language Processing Course Project, Monsoon'21*
* **Guide**: *Dr Md Shad Akhtar*
* **Duration**: Jun'21 - Sep'21  
* **Work**:
    * Utilized transfer learning by trained transformer models BART, T5 and BERT on a novel dataset of over 60k Indian news articles
    * Performed two-stage fine-tuning to increase the performance of the generation model by first training on an existing large-scale news corpus.
    * Open-sourced the custom trained models: [1](https://huggingface.co/rg089/distilbart-summarization){:target="_blank"}, [2](https://huggingface.co/rg089/t5-headline-generation){:target="_blank"}, [3](https://huggingface.co/rg089/bert_newspaper_source){:target="_blank"}
    * Hosted the demo application using on HuggingFace Spaces using Gradio.

## <img src="https://img.icons8.com/external-xnimrodx-lineal-color-xnimrodx/64/000000/external-news-communication-xnimrodx-lineal-color-xnimrodx.png" width="3%" height="3%"/> Newsemble 
* **Links:** [[`api`](http://www.newsemble.ml/news){:target="_blank"}, [`code`](https://github.com/rg089/newsemble){:target="_blank"}, [`blog`](https://medium.com/@rg089/newsemble-3311d2dc9817){:target="_blank"}]
* **Description**: API for real-time fetching of complete content and meta-data of news articles.
* **Type:** *Self-Project*  
* **Duration**: May'21 - Jul'21  
* **Work**:  
    * Developed a REST-API using Flask with custom scrapers for each selected news source (currently, a total of six news sources are defined)
    * Utilized a CRON scheduler to run the scrapers every hour in the cloud to improce performance
    * To reduce the latency factor caused by scraping, the articles are directly fetched from the database whenever a request is instantiated.
    * Employed tools like Flask, BeautifulSoup, PyMongo, MongoDB, Heroku etc. to facilitate this API.

## <i class="fas fa-laptop-code"></i> Neural Complexity Measures (Implementation) 
* **Links:** [[`code`](https://github.com/rg089/neural-complexity-measures){:target="_blank"}, [`writeup`](https://raw.githubusercontent.com/rg089/neural-complexity-measures/master/report.pdf){:target="_blank"}]
* **Description**: An implementation of the NeurIPS'20 paper, [Neural Complexity Measures](https://arxiv.org/pdf/2008.02953){:target="_blank"} on a new multitask dataset
* **Type:** *CSE663A: Meta-Learning Course Project, Winter'22*
* **Guide**: *Dr Gautam Shroff*
* **Duration**: Feb'22 - Apr'22  
* **Work**:
    * The key idea of the paper is to estimate the generalization capabilites of a task-learner by meta-learning a model that incorporates its predictions
    * Implemented the paper (in Pytorch) on a multitask dataset with multiple regression tasks and mutiple multiclass classification tasks
    * Along with the basic implementation, proposed *Uncertainty Aware Gap Estimation*, which takes uncertainty of the meta-learner into account when estimating the generalization gap
    * Demonstrated that incorporating uncertainty improves performance on classification along with providing further analysis

## <i class="fas fa-gamepad"></i> ColorSwitch 
* **Links:** [[`code`](https://github.com/rg089/ColorSwitch){:target="_blank"}, [`info`](https://github.com/rg089/ColorSwitch#readme){:target="_blank"}]
* **Description**: Java implementation of the android game ColorSwitch, employing different design patterns and with bonus features!
* **Type:** *CSE201:Advanced Programming Course Project, Monsoon'20*
* **Guide**: *Dr Vivek Kumar*
* **Duration**: Sept'20 - Nov'20  
* **Work**:
    * Implemented the game in JavaFX from scratch, while retaining gameplay smoothness by employing various physics principles
    * Utilized various design patterns to handle different parts of the game.
    * Implemented various bonus components like cheat codes, other multi-functional shapes and modules etc.
    * Used (and learned about) Object-Oriented Programming, Design Principles, JavaFX etc.

## <img src="https://img.icons8.com/external-icongeek26-linear-colour-icongeek26/64/000000/external-Sudoku-table-games-icongeek26-linear-colour-icongeek26.png" width="3%" height="3%"/> SudokuSolver 
* **Links:** [[`code`](https://github.com/rg089/SudokuSolver/){:target="_blank"}, [`info`](https://github.com/rg089/SudokuSolver#readme){:target="_blank"}]
* **Description**: Automatically detecting, recognizing and solving sudokus using OpenCV, PIL and TensorFlow.
* **Type:** *Self-Project*  
* **Duration**: Feb'21 - Mar'21
* **Work**:  
    * Designed an automated framework for solving sudokus (either image or video) using image processing techniques and CNN's
    * Integrated support for generating and overlaying the solved suodku on top of the input, as well as generating a digital copy of the solved sudoku
    * Extracted of the location of the digits using various image processing strategies like thresholding, contour-detection, homography, perspective-transformation, perspective-warping amongst others
    * Combined the MNIST dataset with a custom artificially generated dataset using PIL and OpenCV to train the recognition model
    * Implemented the recognition of digits using an ensemble of CNNs built on top of the standard LeNet architecture
    * Employed Peter Norvig's algorithm for solving the sudoku

## <img src="https://img.icons8.com/external-smashingstocks-outline-color-smashing-stocks/66/000000/external-cricket-games-smashingstocks-outline-color-smashing-stocks.png" width="3%" height="3%"/> IPL Score Prediction 
* **Links:** [[`website`](https://ipl-score-predictions.herokuapp.com/){:target="_blank"}, [`code`](https://github.com/rg089/ipl-score-prediction){:target="_blank"}, [`info`](https://github.com/rg089/ipl-score-prediction#readme){:target="_blank"}]
* **Description**: Prediction of the score of an IPL match using Machine Learning
* **Type:** *Self-Project*  
* **Duration**: Nov'20 - Dec'20  
* **Work**:  
    * Designed a website to predict the first-innings score of an IPL match
    * Collected and processed the dataset from 2008-2020 to train the regression model
    * Utilized feature-engineering to extrapolate new features like toss decision, score in the last six overs amongst other to boost performance of the regressor
    * Experimented with various different regression models for the task and chose XGBoostRegressor as it achieved the lowest $MSE$ as well as $R^2$ score on the validation set
    * Designed the responsive site from scratch using HTML, CSS and JavaScript (and got to learn these tools)

## <i class="fas fa-broom"></i> Safeya 
* **Description**: An app for digitizing various maintenance tasks at IIIT-D
* **Type:** *CSE202:Fundamentals of Database Management Systems Course Project, Winter'21*
* **Guide**: *Dr Mukesh Mohania*
* **Duration**: Feb'21 - Apr'21  
* **Work**:  
    * Designed a model application for digitizing various maintenanced and cleaning tasks at IIIT-D.
    * Responsible for conceptualization, data population, table creation, composing queries and implementing the backend (using Flask and MySQL).
    * Used and learned about various fundamental database concepts like ER Diagrams, Normalization, Query Composition etc.

