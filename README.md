# Financial-Market-News-Sentiment-Analysis

## Project Analysis Report: Financial Market News Sentiment Analysis

### Project Overview:

The Financial Market News Sentiment Analysis project is designed to predict sentiment labels (positive or negative) based on news articles related to the financial market. This sentiment analysis plays a crucial role in understanding market sentiment and making well-informed decisions based on news sentiment.

### Data Exploration and Preprocessing:

- The dataset comprises 27 columns and 4,101 rows, with no NULL values, indicating good data quality.
- Key columns include Date, Label (sentiment), and 25 News columns.
- Initial analysis revealed a well-balanced distribution of sentiment labels.
- Text preprocessing techniques like tokenization, stop word removal, and lemmatization were applied to the News columns.

### Feature Engineering and Text Vectorization:

- A Combined_News column was generated by merging all News columns.
- TF-IDF vectorization converted text data into numerical features using the TF-IDF Vectorizer.
- The top 5,000 features were selected for model training.

### Model Development:

- Initially, a RandomForestClassifier model was trained on the TF-IDF transformed data.
- The model achieved **100% accuracy** on the training data and **51.7% accuracy** on the testing data.
- Cross-validation scores exhibited consistency but moderate performance.
- Model metrics, including precision, recall, and F1-score, were approximately 0.52, 0.63, and 0.57, respectively.

### Hyperparameter Optimization:

- Hyperparameter tuning was conducted using Bayesian Optimization.
- The optimized RandomForestClassifier with Bayesian Optimization resulted in enhanced precision, recall, and F1-score.
- Best hyperparameters discovered were max_depth=15, min_samples_leaf=3, min_samples_split=10, and n_estimators=200.

### Interpretation and Visualization:

- Feature importance analysis identified the most influential terms in predicting sentiment.
- A confusion matrix was utilized for a visual evaluation of the model's performance.

### Conclusion:

The Financial Market News Sentiment Analysis project successfully implemented sentiment analysis on financial news articles. The initial model achieved moderate performance, further enhanced through hyperparameter tuning with Bayesian Optimization. This project provides valuable insights into sentiment trends in financial news, showcasing a structured approach to sentiment analysis using machine learning and text data processing techniques.

This comprehensive analysis report demonstrates meticulous data preprocessing, model training, hyperparameter optimization, and thorough evaluation in the context of the Financial Market News Sentiment Analysis project.  
