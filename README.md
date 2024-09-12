# Statistical-Modelling

# Music Popularity Analysis

This repository contains a Python-based analysis of music tracks to explore factors affecting their popularity. The analysis includes data cleaning, visualization, and a linear regression model to understand how various features impact the popularity of music tracks.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Data Description](#data-description)
3. [Data Cleaning](#data-cleaning)
4. [Exploratory Data Analysis](#exploratory-data-analysis)
5. [Correlation Analysis](#correlation-analysis)
6. [Feature Impact Analysis](#feature-impact-analysis)
7. [Linear Regression Model](#linear-regression-model)
8. [Results](#results)
9. [Usage](#usage)
10. [Dependencies](#dependencies)
11. [License](#license)

## Project Overview

This project aims to analyze a dataset of music tracks to determine how various features (such as danceability, energy, and loudness) influence the popularity of the tracks. The analysis involves:

- Data cleaning and preprocessing
- Visualization of data distributions and correlations
- Building and evaluating a linear regression model

## Data Description

The dataset consists of 100 music tracks with the following features:

- `Track Name`: Name of the music track
- `Artists`: Name of the artists
- `Album Name`: Name of the album
- `Album ID`: Unique identifier for the album
- `Track ID`: Unique identifier for the track
- `Popularity`: Popularity score of the track
- `Release Date`: Release date of the track
- `Duration (ms)`: Duration of the track in milliseconds
- `Explicit`: Boolean indicating if the track is explicit
- `External URLs`: URLs to the track
- `Danceability`: Danceability score
- `Energy`: Energy score
- `Key`: Musical key of the track
- `Loudness`: Loudness of the track
- `Mode`: Musical mode of the track
- `Speechiness`: Speechiness score
- `Acousticness`: Acousticness score
- `Instrumentalness`: Instrumentalness score
- `Liveness`: Liveness score
- `Valence`: Valence score
- `Tempo`: Tempo of the track

## Data Cleaning

The following steps were performed to clean the dataset:

1. **Dropped Unnecessary Column**: Removed the `Unnamed: 0` column.
2. **Handled Missing Values**: Filled missing values in `Track Name`, `Artists`, and `Album Name` with 'Unknown'.

## Exploratory Data Analysis

1. **Distribution of Popularity**: A histogram with KDE to visualize the distribution of popularity scores.
2. **Correlation Matrix**: A heatmap to show correlations between numerical features.
3. **Individual Popularity Analysis**: Scatter plots to analyze how individual features affect popularity.

## Correlation Analysis

A correlation matrix was generated to visualize the relationships between numerical features. This matrix helps in understanding which features have strong correlations with popularity.

## Feature Impact Analysis

Scatter plots were used to explore how specific features like `Danceability` and `Energy` impact the popularity of music tracks, with additional analysis on explicit content.

## Linear Regression Model

1. **Data Preparation**: Features were standardized and split into training and testing sets.
2. **Model Training**: A linear regression model was trained to predict track popularity.
3. **Evaluation**: Model performance was evaluated using Mean Squared Error (MSE) and R-squared metrics.

### Model Coefficients

Here are the coefficients of the linear regression model:

- `Danceability`: 1.249640
- `Energy`: -3.204815
- `Loudness`: 1.141456
- `Acousticness`: 2.469403
- `Valence`: 2.125671
- `Explicit`: 1.620926e-14
- `Key`: -3.189486
- `Mode`: -5.859715
- `Speechiness`: 0.033982
- `Instrumentalness`: 0.339075
- `Tempo`: -1.865736

## Dependencies

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

## License
Feel free to modify or add sections as needed to fit your specific use case and repository details.
