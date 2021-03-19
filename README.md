# Article Recommendation Project
article-recommendations-watson-studio consists primarily of a Jupyter Notebook that analyzes data from the IBM Watson Studio community platform, and explores several recommendation engine methods to make article suggestions for users engagement. The Watson Studio community is a collaborative ecosystem of curated datasets, articles, notebooks and other kinds assets (herein referred to as articles) related to data science, machine learning and artificial intelligence. Users on the platform interact with these articles. The goal of this project is to explore recommendation options to later build a system that creates a personalized recommendation experience.

The current version of this project uses three main methods for implementing recommendations:

* Rank Based Recommendations
* User-User Based Collaborative Filtering
* Matrix Factorization

## Base Dependencies:
This project does require Python 3.6 or above, along with the following dependencies:
```
numpy
pandas
matplotlib
pickle
```

## Data and File Overview
The data used in this project was provided by [IBM Watson Studio](https://www.ibm.com/cloud/watson-studio). This data was provided in two CSV files, one containing thousands of anonymized interactions between users and articles  (user-item-interactions.csv) and one containing the article content (articles_community.csv).

An outline and summary of the files contained in this project are provided below.

```
├── README.md
├── Recommendations_with_IBM.ipynb # main notebook file for project
├── Recommendations_with_IBM.html # HTML version of notebook
├── user_item_matrix.p # pickle of user item matrix data
├── data
│   ├── articles_community.csv # article content data
│   └── user-item-interactinos.csv # user item interaction data
└── tests
    ├── project_test.py # test file for project
    ├── top_5.p  # pickle solution list top 5
    ├── top_10.p # pickle solution list top 10
    └── top_20.p # pickle solution list top 20
```
