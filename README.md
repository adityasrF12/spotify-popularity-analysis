# Spotify Song Popularity Analysis
> **STAT 530: Applied Regression Analysis**

## Project Overview
This project explores the determinants of song popularity using a dataset of 18,000+ Spotify tracks. The goal was to build and compare multiple statistical models to identify which audio features (e.g., energy, acousticness, instrumentalness) most significantly impact a song's popularity score.

## Dataset Information
The analysis utilizes the Song Popularity Dataset, which contains various musical metadata for tracks on the Spotify platform.
* **Source:** [Song Popularity Dataset (Kaggle)](https://www.kaggle.com/datasets/yasserh/song-popularity-dataset)
* **Observations:** 18,835 tracks
* **Key Features:** Danceability, Energy, Loudness, Acousticness, Instrumentalness, Liveness, Valence, and Tempo.

## Statistical Methodology
The project follows a comprehensive data science workflow implemented in R:

1. **Exploratory Data Analysis (EDA):** Correlation heatmaps and distribution plots to identify multicollinearity and feature relationships.
2. **Multiple Linear Regression:** Predicting the continuous popularity score and assessing model fit through Adjusted R-squared and residual analysis.
3. **Logistic Regression:** A binary classification approach to predict if a song is a "Hit" based on a popularity threshold.
4. **Random Forest:** An ensemble learning method used to handle non-linear relationships and determine variable importance.

## Key Findings and Performance
* **Linear Regression:** Achieved an Adjusted R-squared of 0.222, with loudness and danceability emerging as the strongest positive predictors.
* **Logistic Regression:** Attained a classification accuracy of 76.2%.
* **Random Forest:** Delivered the highest predictive power with a test accuracy of 82.3% and an OOB error rate of 17.75%.
* **Variable Importance:** Instrumentalness and loudness were consistently identified across all models as critical factors in determining popularity.

## Technical Stack
* **Language:** R
* **Libraries:** ggplot2, corrplot, caret, randomForest, dplyr, broom
* **Reporting:** R Markdown (Knitted to HTML/PDF)

## Repository Structure
* `/data`: Contains `song_data.csv`.
* `/scripts`: R Markdown files (`.Rmd`) for EDA, Linear Regression, Logistic Regression, and Random Forest.
* `/output`: Knitted HTML outputs.
* `Final Project.Rproj`: RStudio project configuration file.

## How to Use
1. **Clone the Repo:** `git clone https://github.com/adityasrF12/spotify-popularity-analysis.git`
2. **Open Project:** Open `Final Project.Rproj` in RStudio.
3. **View Results:** Open the `.html` files in the `/output` folder to view the full analysis and visualizations without running code.

