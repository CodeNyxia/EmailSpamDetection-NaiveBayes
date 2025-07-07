# Email Spam Detection with Naive Bayes

## Overview
This project demonstrates a simple email spam detection system using the Multinomial Naive Bayes classifier from scikit-learn. The model is trained on a small dataset of email messages labeled as spam (1) or not spam (0), and can predict whether new emails are spam or not based on their content.

## Features
- Text preprocessing using CountVectorizer to convert email text into numerical features
- Train-test split for model evaluation
- Multinomial Naive Bayes classifier for spam detection
- Model evaluation with accuracy score and confusion matrix
- Prediction capability for new email messages

## Requirements
- Python 3.x
- pandas
- scikit-learn

## Installation
1. Clone this repository
2. Install the required packages:
   ```bash
   pip install pandas scikit-learn
   ```

## Usage
1. Run the Jupyter notebook `EmailSpamDetection.ipynb`
2. The notebook will:
   - Load and preprocess the sample email data
   - Train the Naive Bayes classifier
   - Evaluate the model's performance
   - Demonstrate predictions on new email examples

## Results
The current model achieves 50% accuracy on the test set, with the following confusion matrix:
```
[[0 1]
 [0 1]]
```

Example predictions:
- 'free meeting' → Spam
- 'urgent project update' → Not spam

## Limitations
- The dataset is extremely small (only 6 examples) which affects model performance
- The model uses simple bag-of-words features without advanced text processing
- No hyperparameter tuning has been performed

## Future Improvements
- Use a larger, more diverse dataset
- Implement more advanced text features (TF-IDF, n-grams)
- Try different classification algorithms
- Add hyperparameter tuning
- Implement proper cross-validation

## License
This project is open source and available under the MIT License.
