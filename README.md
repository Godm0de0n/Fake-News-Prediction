# Fake News Prediction using Logistic Regression

## Overview
This project predicts fake news using a **Logistic Regression** model. The model is trained using only the `author` and `title` fields, which are combined into a new feature. **NLTK** is used for text preprocessing.

## Dataset
The dataset used for this project is available on Kaggle: [Fake News Dataset](https://www.kaggle.com/c/fake-news/data)

The dataset contains the following columns:
- **id**: Unique identifier for each news article.
- **title**: The headline of the news article.
- **author**: The name of the article's author.
- **text**: The full text of the article (not used in this model).
- **label**: The target variable (0 for real news, 1 for fake news).

## Dependencies
Before running the project, install the required libraries using:

```bash
pip install pandas numpy scikit-learn nltk re
```

Dependencies used in the project:
- `numpy` : For numerical computations
- `pandas` : For data manipulation and preprocessing
- `scikit-learn` : For machine learning models and evaluation
- `nltk` : For natural language processing tasks
- `re` : For text cleaning using regular expressions

## Preprocessing Steps
1. **Handling Missing Values**: Filling missing `author` and `title` values with empty strings.
2. **Feature Creation**: Combining `author` and `title` into a single `content` field.
3. **Text Cleaning**: Removing special characters, converting text to lowercase.
4. **Stopword Removal & Stemming**: Using `nltk` to remove stopwords and apply stemming.

## Model Training
- The dataset is split into **training** and **testing** sets.
- **TF-IDF Vectorization** is applied to convert text into numerical features.
- A **Logistic Regression** model is trained on the transformed data.

## Model Evaluation
- **Accuracy Score** is used to measure performance.  (95%+)
- The model's predictions are compared against actual labels.

## Contribution
Feel free to contribute by opening an issue or submitting a pull request.

## License
This project is licensed under the MIT License.

## Author
**Abhisek Nag**

