# Spam Email Classification Using Decision Trees and TF-IDF

## Project Overview
This project demonstrates text classification using TF-IDF feature extraction and a Decision Tree classifier to distinguish spam messages from legitimate messages.

**Dataset note:** The current implementation uses the SMS Spam Collection dataset, which contains SMS messages rather than emails.

## Objectives
- Explore and analyze the dataset.
- Convert text into numerical features using TF-IDF.
- Train a Decision Tree classification model.
- Evaluate performance using stratified 5-fold cross-validation.
- Test the model on unseen messages.
- Demonstrate predictions using an interactive message checker.

## Methodology
1. Load and inspect the dataset.
2. Perform exploratory data analysis (EDA).
3. Extract text features using TF-IDF.
4. Train a Decision Tree classifier.
5. Evaluate with stratified 5-fold cross-validation.
6. Evaluate on a separate test set and visualize the confusion matrix.
7. Test sample messages using the interactive demo.

## Results
Cross-validation results:
- Accuracy: 96.07% ± 0.59 percentage points
- Macro precision: 91.02% ± 1.28 percentage points
- Macro recall: 92.42% ± 1.84 percentage points
- Macro F1-score: 91.67% ± 1.27 percentage points

Separate test-set confusion matrix:
- Correct ham predictions: 934
- Ham incorrectly classified as spam: 32
- Spam incorrectly classified as ham: 21
- Correct spam predictions: 128
- Test accuracy: approximately 95.34%

The cross-validation and test-set results are from separate evaluation procedures.

## Project Files
- `Spam_Email_EDA.ipynb` — exploratory data analysis.
- `Spam_Email_Classification.ipynb` — model training, evaluation, and interactive demo.
- `Spam_Email_Classification_Hackathon_PPT.pptx` — project presentation.
- `Review_3_Case_Based_Problem_Statement.pdf` — problem statement.

## Requirements
Python 3, pandas, matplotlib, scikit-learn, and ipywidgets.

## How to Run
1. Open the classification notebook in Google Colab.
2. Upload `sms_spam_dataset.csv` to the Colab session.
3. Run the notebook cells in order.
4. Use the interactive checker to classify sample messages.

## Future Scope
- Evaluate the model on a genuine email dataset.
- Compare Decision Trees with other classification algorithms.
- Improve performance and deploy the classifier as a web application.
