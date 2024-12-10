# Sentiment_Analysis_Reddit_Project

# Project Overview
This project focuses on sentiment analysis of Reddit posts related to climate change using data
collected from 2010 to 2024. Posts were retrieved by filtering with subreddit and query
keywords, which are specific terms relevant to climate change. Sentiment analysis was
performed using the TextBlob model, which is selected after evaluating three different sentiment
models, TextBlob, VADER, and BERT, by using a sample Reddit dataset from Kaggle. Each
model's accuracy was assessed, and TextBlob was chosen because it gave better accuracy score
and performance across other metrics. For data collection, processing, and storage, a custom
Python implementation was used instead of SparkStreaming or other streaming tools as it gave
me greater customization and detailed tracing of each process. An interactive dashboard,
developed with the Dash package, is used for visualization for finding insights. Key features
include a line graph, a pie chart, a word cloud, and a table. This analysis revealed a steady
increase in positive and neutral sentiments in climate change discussions on Reddit, while
negative sentiments remained relatively stable.

# File Structure Documentation

This document provides an overview of the files and folders included in the project. It is designed to help users locate specific files and understand their purposes, ensuring efficient navigation through the dataset, code, and supporting materials.

## Folder Structure

### 1. `For_Streaming` Folder
This folder contains all files related to streaming data processing, including collected data, exploratory analysis, and dashboard creation.

- **`climate_change_posts_streaming.csv`**
  - Stores post details such as `ID`, `Title`, `SelfText`, and `Date` for streaming data processing.

- **`climate_change_sentiment_analysis_streaming.csv`**
  - Stores post details along with their sentiment scores for streaming data processing.

- **`Dashboard_Nov_data.ipynb`**
  - Code for creating a dashboard to analyze posts from November 2024.

- **`EDA_Streaming.ipynb`**
  - Code for performing Exploratory Data Analysis (EDA) on streaming data.

- **`filtered_data_november_2024_Streaming.csv`**
  - Contains filtered post data for November 2024.

- **`Interactive_Dashboard_Streaming.ipynb`**
  - Code for creating an interactive dashboard for analyzing overall streaming data.

- **`Reddit_streaming_data_collection.ipynb`**
  - Code for collecting Reddit data and applying sentiment analysis on streaming posts.

---

### 2. `For_Batch` Folder
This folder contains files and scripts for processing batch data, including datasets, analysis scripts, and dashboards.

- **`climate_change_posts_batch.csv`**
  - Stores post details such as `ID`, `Title`, `SelfText`, and `Date` for batch data processing.

- **`climate_change_sentiment_analysis_batch.csv`**
  - Stores post details along with their sentiment scores for batch data processing.

- **`EDA_Batch.ipynb`**
  - Code for performing Exploratory Data Analysis (EDA) on batch data.

- **`Interactive_Dashboard_Batch.ipynb`**
  - Code for creating an interactive dashboard for analyzing batch data.

- **`Reddit_data_collection_Batch.ipynb`**
  - Code for collecting Reddit data and applying sentiment analysis on batch posts.

---

### 3. `Model_Selection` Folder
This fol
