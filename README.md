**Title: Stock Market Prediction Using News Headlines with Text Classification**

This project focuses on creating a text classification model using news headlines to predict whether the stock market will go up or down. By analyzing the sentiment and content of daily news headlines, the model aims to provide insights into the relationship between media coverage and market behavior.

### Project Steps:

1.  **Data Loading:**

    -   The project begins by loading a dataset of historical news headlines. The dataset includes dates, labels (indicating market movement), and multiple news headlines for each date.
2.  **Data Preprocessing:**

    -   The headlines are cleaned by removing non-alphabetic characters and converting text to lowercase. This preprocessing helps in standardizing the data for the model.
    -   The data is split into training and testing sets based on the date.
3.  **Feature Extraction:**

    -   A `CountVectorizer` is used to convert the textual data into numerical features. Specifically, a bigram model (ngram_range=(2,2)) is applied to capture pairs of words.
4.  **Model Training:**

    -   A `RandomForestClassifier` is used as the machine learning model. It is trained on the transformed headline data to learn patterns that might predict stock market movements.
5.  **Prediction:**

    -   The trained model can then be used to predict the market movement (up or down) based on new headlines.

### Tools & Libraries:

-   **Pandas:** For data manipulation and preprocessing.
-   **Scikit-learn:** For feature extraction (`CountVectorizer`) and model training (`RandomForestClassifier`).

### Objective:

The project aims to explore how well news sentiment, captured through headlines, can predict stock market movements, providing insights into the relationship between media coverage and market behavior.
