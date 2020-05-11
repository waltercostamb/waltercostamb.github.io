---
layout: post
title: "Learn Data Analysis with Python"
date: 2020-04-07
---

I have been asked by a friend for directions on learning data analysis with python, so here is a compilation of
my suggestions. 

To start, there are two very important considerations you should make. The first is to understand your purpose. 
What exactly do you want to do with this knowledge? This only seems trivial. You only understand what you really 
want after you learn more on the topic. In other words, you start from a general knowledge and then go to specifics.
What is data science? Is it the same as big data? Is it fun? Does it require lots of equipment or software?
I would suggest in this case to start reading more about data science, career prospects and also to discuss it with
colleagues. Don't loose your own purpose of sight while learning. What makes a good data scientist 
is their focus. A bioinformatician, for instance, can be considered a data scientist. Their focus or domain knowledge
is biology. Although I see a lot of generalist approaches on posts about data science, I believe having focus is key 
to being fullfilled and competent. Choose the area you want to focus and pursue this goal. 
Some options of specializations are: biology, medicine, finance, etc. Although the methods overlap, domain knowledge is key.

<img border="0" src="https://github.com/waltercostamb/waltercostamb.github.io/blob/master/figures/data_science.jpg" width="250" height="210" /></a>  

Data science. Credit: [Michael Barber](https://towardsdatascience.com/introduction-to-statistics-e9d72d818745)

The other important thing I want to mention is to understand the difference between data analysis and "big data". Although
the two may seem the same at first glance, they are not. Data analysis is required for big data, but big data is not required 
for data analysis. Data analysis involves programming, problem solving, statistical analysis and visualization. Big data 
involves that and also other specific tools like Spark and Hadoop (which uses the MapReduce method). I am not a particular 
fan of big data, since it feels to me more like handling tons on input than analysis. I have done a course in big data, but
this is not my area of expertise, so I would advise you to talk to a specialist if you are interested in big data.

I did this [big data and statistik](https://www.alfatraining.de/gefoerderte-weiterbildung/berlinmitte/stadt/berlin/kurs/statistik/N/0/0/kombi/statistik-und-big-data/) 
course from alfatraining (in German), which I found very informative. Summarizing the content of this course:

  - Basic statistics:  
      - measure theorie (population, sample, types of samples, measurement, scaling)  
      - Univariate statistics (distributions, etc.)  
      - Bivariate statistics  
      - Visualization  
      - Comparison of two distributions with statistical tests (parametric and non-parametric tests)  
      - Comparison of more than two distributions  
      
  - Big data  
    - What is big data?  
    - Programming logic (data structures, loops, logic statements, etc.)  
    - Programming syntax in python (other languages are also possible like R, Julia, C or others)  
    - Python modules (numpy, pandas)  
    - Visualization  
    - SQL language   
    - SQL and noSQL Database Management Systems  
    - Principles of data analysis, statistics, data mining  
    - Data manipulation and storage (MapReduce method, python Spark module)  
    - Cloud computing

We did final projects for both courses. I published mine as GITHub repositories, so you can have an idea of which type of 
project and questions can be approached by these techniques. For the big data course I applied a method of machine learning
to classify breast cancer data using a [python notebook](https://github.com/waltercostamb/breast_cancer_diagnostics/blob/master/project_MB.ipynb). 
For the statistics course I studied criminal data from the USA from 1975 to 2014 with an 
[R script](https://github.com/waltercostamb/Statistical_analysis_crime_USA/blob/master/analysis_crime_USA.r), which I prefer for statistical 
analysis. You could do this in python without a problem. Python notebooks are great, especially for learning.

I recommend the following book for learning data science with python:
  
  - ["Python Data Science Handbook"](https://jakevdp.github.io/PythonDataScienceHandbook/), by Jake VanderPlas, who very
  generously put his book online for free. I have the hard copy in german, so a translation is available for german speakers. 
  I would say all chapters of this book are relevant for learning data science:
  
    - Chapter 1 (if you are interested in python notebooks, which I highly recommend)  
    - Chapter 2, Numpy
    - Chapter 3, Pandas
    - Chapter 4, Visualization with MatplotLib (I do it with R, ggplot2, but want to learn more MatplotLib, since it seems to have very interesting new functions)
    - Chpater 5, with the following topics:
        - What Is Machine Learning?
        - Linear Regression
        - Principal Component Analysis

If you want to specialize in bioinformatics or learn more about it, I recommend this book: ["Python Programming for Biology"](https://www.goodreads.com/book/show/23463543-python-programming-for-biology?ac=1&from_search=true&qid=OfhvhtIRBG&rank=1), 
by Tim J. Stevens and Wayne Boucher.

I have a very important remark about machine learning. This is a very exciting topic, and seems at first that it can solve
 almost anything. It can't. So be careful and patient. There are many problems that can be solved by basic statistics, so they
 should be at least approached first with the more classical or conservative approach. As an example that can be approached 
 by machine learning: say you have a very interesting 
 classification problem: I have many samples, each with a tag 0 or 1. I can create groups based on my previous knowledge and
 classify a new unknown sample. Is it 0 or 1? This is exactly the same problem I approached in my 
 [final project of the big data course](https://github.com/waltercostamb/breast_cancer_diagnostics): does this patient
 have benign or malign cancer? 
 
 Alternatively, you may have a prediction problem. Say you have many variables and want to predict an 
 outcome based on these variables. You should not start your project by directly applying a machine learning method. Why?
 Because if you do not understand your data, you are, on the best of cases, not producing new insights or knowledge, 
 you are only producing computational artifacts that do not help anyone. On the worst of cases, you are actually
producing wrong or harmful data, that can be used to justify [bad political policies](https://www.nytimes.com/2020/04/01/world/americas/brazil-bolsonaro-coronavirus.html). 

We have responsibilities as data scientists, especially in current times, exemplified by the [corona pandemic](https://www.williamrchase.com/post/why-i-m-not-making-covid19-visualizations-and-why-you-probably-shouldn-t-either/).
 You have to first start with the basics. Understand your data, 
 acquire a feeling for your data. Plot the distributions of the variables, calculate basic statistics for them 
 (mean, median, minimum, maximum). Make correlations afterwards, and most important of all, talk to a specialist. 
 Learn and read about the subject. In my case, for the cancer project, I read some articles about breast cancer, 
 cancer lesions and machine learning applied to breast cancer.  
 
 After doing the basic statistics and having acquired a feeling for your data, you have to see if machine learning can be 
 applied for your problem. After making sure machine learning is a good idea, then you can plan your experiments. Carefully 
 choose your variables and start with the most simple methods first, like PCA or linear regression. Afterwards go to logistic
 regression, support vector machines and random forest. Although the more charming method nowadays is neural networks (hello
 [tensor flow](https://blog.oursky.com/2018/02/14/tensorflow-business-applications-ai-hong-kong/)!), it is only appropriate for problems with lots and lots of training data. 
 
 Most important of all, don't loose sight of your initial question, start with the basics and be mindful of the consequences
 of making your work available to the public. There are lots of interesting
 data available that you can play with. After reading some chapters, you will start feeling you can already code, so create 
 a small project for yourself. I would stay clear of any sensitive data (like corona) in case you want to make your project public, say in GITHub, but if you want to do it, just keep your project private. 
 Create a python notebook and keep track of your progress. I recommend defining a subject you
 like and searching for it on repositories like [kaggle](https://www.kaggle.com/). I found the data for my big data and 
 statistics project in kaggle. It was actually fun and fullfilling doing these small projects.

I hope you enjoyed reading this, and that it was useful for you. If you would like to read more posts like this, feel free to 
[contact me](https://waltercostamb.github.io/).
