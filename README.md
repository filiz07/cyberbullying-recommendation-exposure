# Cyberbullying Exposure in Recommendation Systems

This repository contains the implementation developed for an MSc dissertation investigating cyberbullying exposure in text-based recommendation systems.

## Study Overview

The study examines how different text-based recommendation approaches influence users' exposure to cyberbullying content. User profiles are constructed from historical tweet content and compared with candidate tweets to generate Top-10 recommendations.

The study evaluates both overall cyberbullying exposure and differences in exposure across cyberbullying types and user groups.

## Recommendation Methods

Four recommendation approaches are evaluated:

- Random Ranking (Baseline)
- TF-IDF + Cosine Similarity
- Doc2Vec + Cosine Similarity
- Sentence-BERT + Cosine Similarity

Random Ranking is used as a baseline, while the other three methods generate recommendations based on textual similarity between user profiles and candidate tweets.

## Evaluation Metrics

Cyberbullying exposure is evaluated using three metrics:

- Harmful Content Ratio (HCR)
- Type Exposure Rate (TER)
- Group Exposure Gap (GEG)

These metrics are used to examine overall harmful-content exposure, exposure to different cyberbullying categories, and differences in exposure across user groups.

## User Group Analysis

Exposure is compared across users based on:

- Activity
- Reach
- Dominant sentiment

These characteristics are used for exposure analysis and are not used as direct inputs to the recommendation ranking process.

## Datasets

Two publicly available Kaggle datasets are used in this study.

### 1. COVID-19 Twitter Dataset

Used to construct user textual profiles and derive activity, reach, and sentiment-based user groups.

Dataset:
https://www.kaggle.com/datasets/arunavakrchakraborty/covid19-twitter-dataset

### 2. Cyberbullying Classification Dataset

Used as the candidate tweet pool for recommendation generation and subsequent cyberbullying exposure evaluation.

Dataset:
https://www.kaggle.com/datasets/andrewmvd/cyberbullying-classification

The original dataset files are not redistributed in this repository. They can be accessed directly from their original Kaggle sources using the links above.

## Implementation

The complete experimental implementation is provided in:

`Dissertation.ipynb`

The notebook includes:

- Data preparation
- User profile construction
- Activity, reach, and sentiment-based user grouping
- Random Ranking
- TF-IDF recommendation
- Doc2Vec recommendation
- Sentence-BERT recommendation
- Top-10 recommendation generation
- Cyberbullying exposure evaluation
- HCR, TER, and GEG calculations
- Result visualisation

The notebook can also be opened directly in Google Colab using the **Open in Colab** option.

## Author

Filiz Kodat  
MSc Computer Science and Artificial Intelligence  
University of Bradford
