# **Sentiment Analysis Model Documentation**

### 1. Introduction
This project focuses on sentiment analysis using Naïve Bayes and CountVectorizer. The workflow includes data preprocessing, transformation, model training, and evaluation.

### 2. Dependencies & Libraries
Ensure the following Python libraries are installed:
- `pandas` (Data Handling)
- `numpy` (Numerical Operations)
- `sklearn` (Machine Learning)
- `nltk` (Text Processing)
- `pickle` (Model Serialization)

### 3. Dataset Preparation
- The dataset is imported and cleaned.
- Text preprocessing includes stopword removal, stemming, and tokenization.
- CountVectorizer is used to convert text into numerical features.

### 4. Model Training
- Data is split into training and test sets.
- Naïve Bayes classifier (`MultinomialNB`) is used for sentiment classification.
- Hyperparameters are optimized for better performance.

### 5. Model Evaluation
- Accuracy, precision, recall, and F1-score are computed.
- Confusion matrix is used to visualize performance.

### 6. Model Deployment
- The trained model and `CountVectorizer` are saved using `pickle`.
- The model is loaded and used for real-time sentiment predictions.

### 7. Usage Instructions
1. Load the pre-trained `CountVectorizer` and model.
2. Transform input text using `cv.transform()`.
3. Predict sentiment using `model.predict()`.

### 8. Error Handling
- Ensures `CountVectorizer` is fitted before transformation.
- Handles missing data and file not found errors.

### 9. Conclusion
This project successfully classifies sentiment from text using a trained Naïve Bayes model with a bag-of-words approach.

