# Movie Recommendation System Using Neural Networks

This repository contains a Jupyter Notebook that implements a neural network-based movie recommendation system using a content-based filtering approach. The project is built on top of popular machine learning and data manipulation libraries such as TensorFlow, NumPy, and Pandas, among others.

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Notebook Structure](#notebook-structure)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

<a name="overview"></a>

## 1. Overview

The project explores content-based filtering for recommending movies using a neural network model. The core idea is to leverage movie attributes (like genre, year of release) and user preferences to predict user ratings for movies they haven't watched yet.

The notebook guides through the entire process, from data preprocessing, neural network model building, training, and evaluation, to making predictions and recommendations for new and existing users.

<a name="dataset"></a>

## 2. Dataset

The dataset used for this project is derived from the MovieLens ml-latest-small dataset. This dataset contains ratings for around 9000 movies rated by 600 users, with ratings on a scale from 0.5 to 5 in 0.5 step increments. For the purposes of this project, the dataset has been reduced to focus on movies released since 2000 and popular genres.

**Dataset Characteristics:**
- Number of Users: 397
- Number of Movies: 847
- Number of Ratings: 25,521

For each movie, the dataset provides a title, release date, and one or more genres. The user information is limited to the ratings provided by each user.

<a name="installation"></a>

## 3. Installation

To run the notebook, you need to have Python installed along with the following packages:

- `numpy`
- `pandas`
- `tensorflow`
- `scikit-learn`
- `tabulate`
- `pickle5` (if required)

### Install the required libraries

```bash
!pip install numpy pandas tensorflow scikit-learn tabulate pickle5
```

<a name="notebook-structure"></a>

## 4. Notebook Structure

The notebook is organized into the following sections:

### 4.1 Importing Libraries and Google Drive
Mounts Google Drive to access the dataset and imports necessary libraries like TensorFlow, NumPy, and Pandas for building the recommendation system.

### 4.2 Movie Ratings Dataset
Loads the movie ratings dataset, provides an overview of the data, and displays sample data tables.

### 4.3 Content-Based Filtering with a Neural Network
This section introduces the concept of content-based filtering and describes how user and movie vectors are generated for training the model.

### 4.4 Preparing the Training Data
Explains how the data is preprocessed, scaled, and split into training and test sets.

### 4.5 Neural Network Model for Content-Based Filtering
Constructs a neural network model using Keras' Functional API. The model is trained to predict user ratings based on the content features of the movies.

### 4.6 Model Evaluation
Evaluates the model on the test data and provides insights into its performance.

### 4.7 Making Predictions
Uses the trained model to make movie recommendations for both new users (with custom preferences) and existing users.

### 4.8 Finding Similar Items
Calculates the similarity between different movies to provide better recommendations.
