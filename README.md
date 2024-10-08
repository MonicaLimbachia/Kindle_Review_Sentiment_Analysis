**Kindle Review Sentiment Analysis**

This repository contains a comprehensive sentiment analysis project focused on Amazon Kindle reviews. The objective is to classify review sentiments into positive, negative, or neutral categories using advanced NLP and machine learning techniques.

### Project Overview

1. **Dataset:**
   - The dataset comprises Amazon Kindle reviews extracted from the Amazon Product Review dataset. It includes various features such as review text, rating, and review date.
   - The data was cleaned and preprocessed to remove HTML tags, special characters, and stopwords, ensuring a focus on meaningful content.

2. **Data Preprocessing:**
   - **Text Cleaning:** Utilized regular expressions to strip out HTML elements and non-alphanumeric characters.
   - **Tokenization & Lemmatization:** Applied tokenization to break text into words and lemmatization to reduce words to their root forms.
   - **Handling Imbalanced Data:** Implemented SMOTE (Synthetic Minority Over-sampling Technique) to balance the classes in the dataset.

3. **Feature Extraction:**
   - **TF-IDF Vectorization:** Employed TF-IDF to convert the text data into numerical vectors, capturing the importance of words relative to the entire corpus.
   - **Word2Vec Embeddings:** Integrated pre-trained Word2Vec embeddings to capture semantic meaning and context of words in reviews.

4. **Model Building:**
   - **Models Tested:**
     - **Logistic Regression:** Served as a baseline model for binary classification.
     - **Support Vector Machine (SVM):** Used with linear and RBF kernels to explore different decision boundaries.
     - **Random Forest Classifier:** Applied to handle complex relationships and feature interactions.
     - **XGBoost:** Utilized for boosting performance with gradient boosting techniques.
   - **Model Evaluation:** Assessed model performance using accuracy, precision, recall, F1-score, and AUC-ROC. Cross-validation was performed to ensure robustness.

5. **Results:**
   - **Best Performing Model:** XGBoost achieved the highest accuracy and F1-score, indicating strong performance in classifying sentiments.
   - **Confusion Matrix & ROC Curves:** Provided detailed insights into model performance, highlighting areas of strength and improvement.