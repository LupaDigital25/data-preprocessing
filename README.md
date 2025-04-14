# Data Preprocessing Pipeline

This repository contains tools and scripts to clean, deduplicate, and standardize raw news data and topic labels. It is a critical component in the LupaDigital25 ecosystem, preparing datasets for downstream tasks such as analysis and visualization in a web application.

## Project Structure

#### `dataPrep.ipynb`
- Used with the extracted data from `data/news/` to preprocess articles for the web application.
- Handles tasks such as formatting columns, removing duplicates, and standardizing structure.
- Outputs the cleaned dataset to `data/news_preprocessed/`, which is used in further applications.

#### `dataPrep topicEDA.ipynb`
- Performs exploratory data analysis (EDA) on the topic labels.
- Helps understand the distribution, frequency, and structure of topics in the dataset.

#### `dataPrep topicPrep.ipynb`
- Preprocesses and simplifies the topic labels.
- Maps original (often inconsistent) topics to a cleaner set of standardized topics.
- Removes unmapped or invalid topics to streamline the preprocessing in `dataPrep.ipynb`.

#### `dataEDA.ipynb`
- Used to analyze the overall preprocessed data.
- Demonstrates example visualizations and interactions for integrating with the web application.

## Data Files

- `topics.txt`: List of unique cleaned topic labels used in the dataset.
- `topics.json`: Dictionary mapping original raw topics to cleaned and standardized versions.

## Output

- The preprocessed data is saved to `data/news_preprocessed/` and is intended for downstream tasks such as analysis, or frontend integration.