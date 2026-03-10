Automated Exam Evaluation System (NLP-Based Descriptive Answer Grading)

This project implements an Automated Exam Evaluation System that grades descriptive student answers using Natural Language Processing and Machine Learning. Essays are converted into semantic embeddings using Sentence-BERT, and a Random Forest regression model predicts the essay score.

The system is trained using the ASAP Automated Essay Scoring dataset, which contains student essays along with scores assigned by human graders.

Method

The grading pipeline is:

Essay Text
↓
Sentence-BERT Embedding
↓
Random Forest Regression
↓
Predicted Essay Score

The model is trained using an 80–20 train-test split, where 80% of the data is used for training and 20% is used for evaluation.

Evaluation Metrics

Since this is a regression problem, the model is evaluated using:

Mean Squared Error (MSE)

R² Score

Running the Project

The project is implemented as a Jupyter Notebook.

Run the notebook in Google Colab:

Open the notebook in Google Colab

Upload the ASAP dataset zip file

Run the cells sequentially

Technologies Used

Python

Google Colab

Sentence Transformers

Scikit-learn

Pandas & NumPy
