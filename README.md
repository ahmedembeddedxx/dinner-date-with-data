# Dinner Date with Data: Recommending Recipes with PySpark

## Overview
This project aims to recommend recipes to users based on their preferences using PySpark and GPU acceleration. By leveraging PySpark's distributed computing capabilities and GPU-accelerated libraries like cuDF and cuML, the system can efficiently process large-scale data and perform similarity calculations for recipe recommendations.

## Contributors
- [Ahmed](https://github.com/ahmedembeddedx)
- [Ibtehaj](https://github.com/Ibtehaj778)
- Maira

## Installation
To run the project, follow these steps:
1. Install necessary packages:
   ```
   !pip install pyspark
   !pip install cudf-cu12 --extra-index-url=https://pypi.nvidia.com
   !pip install cuml-cu12 --extra-index-url=https://pypi.nvidia.com --no-cache-dir
   ```
2. Install additional libraries:
   ```
   !pip install termcolor nltk wordcloud numpy matplotlib seaborn pandas tqdm
   ```
3. Download NLTK data:
   ```
   import nltk
   nltk.download('wordnet')
   ```

## Usage
1. **Setting up Spark Session**: Initialize a Spark session to start working with Spark dataframes.
2. **Loading Data**: Load the recipe data into a Spark dataframe from a CSV file.
3. **Text Cleaning**: Perform text cleaning on the ingredients column to remove numbers and punctuation.
4. **Word Cloud and Word Frequency Analysis**: Visualize the most common ingredients using word cloud and word frequency charts.
5. **Text Preprocessing Pipeline**: Build a text preprocessing pipeline including tokenization, stop word removal, and lemmatization.
6. **GPU Setup**: Check GPU availability and setup for accelerated processing.
7. **Cosine Similarity Calculation**: Calculate cosine similarity between recipes using GPU acceleration.
8. **Recommendation Generation**: Generate recipe recommendations based on similarity scores.
9. **Ending Spark Session**: Stop the Spark session to release resources.

## Features
- Efficient handling of large-scale data using PySpark.
- GPU-accelerated processing for faster similarity calculations.
- Text preprocessing pipeline for cleaning and tokenizing recipe ingredients.
- Visualization of ingredient frequencies using word cloud and word frequency charts.
- On-the-fly similarity calculations for real-time recommendation generation.

## Ending Notes
The project showcases the use of PySpark and GPU acceleration for recipe recommendations, providing insights into the text processing pipeline and similarity calculations. It suggests potential improvements for model persistence, hyperparameter tuning, user feedback integration, and scalability. Overall, it's a well-structured project with the potential for further enhancements.

## License
This project is licensed under the [MIT License](LICENSE).
