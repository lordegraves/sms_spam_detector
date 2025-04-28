# SMS Spam Detector

## Overview
This project develops a machine learning model to classify SMS text messages as "spam" or "ham" (non-spam). Using Natural Language Processing (NLP) techniques and supervised learning algorithms, the model processes text data and predicts spam messages effectively. The project was completed as part of an applied machine learning module challenge.

## Files
- `sms_spam_detector.ipynb` — Jupyter Notebook containing data preprocessing, feature extraction, model training, and evaluation.
- `Resources/` — Directory containing the input SMS dataset.
- `README.md` — Project overview and setup instructions.

## Features
- Text preprocessing: tokenization, lowercasing, stopword removal.
- Feature extraction using TF-IDF (Term Frequency-Inverse Document Frequency).
- Training supervised machine learning models (e.g., Naive Bayes, Logistic Regression).
- Model evaluation using confusion matrices and classification reports.

## Getting Started

### Prerequisites
- Python 3.8 or higher
- Jupyter Notebook or JupyterLab
- pandas
- scikit-learn
- nltk

### Installation
Clone the repository and install the required libraries:

```bash
git clone https://github.com/lordegraves/sms_spam_detector.git
cd sms_spam_detector
pip install pandas scikit-learn nltk
```

## Usage
1. Navigate to the project folder.
2. Open the Jupyter Notebook:

```bash
jupyter notebook
```

3. Open the `sms_spam_detector.ipynb` file.
4. Run the cells sequentially to:
   - Load and preprocess the SMS text data.
   - Transform the data into numerical features using TF-IDF.
   - Train and evaluate the machine learning models.
   - Analyze model performance to identify the best approach.

## Data Sources
- SMS Spam Collection Dataset (available from UCI Machine Learning Repository).

## Acknowledgements
- Thanks to the course instructors for the project framework and support.
- Dataset sourced from UCI Machine Learning Repository.
- Syntax validation and minor troubleshooting assistance provided by ChatGPT.

## License
This project is licensed for educational use only.  
© 2025 Clayton Graves. All rights reserved.

