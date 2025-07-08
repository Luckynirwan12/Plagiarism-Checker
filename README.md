# 📄 Plagiarism Detection using TF-IDF and Cosine Similarity
This Python script checks for textual similarity (potential plagiarism) among multiple .txt files in a given directory using TF-IDF vectorization and cosine similarity.

## ✅ Features
- Automatically scans all .txt files in the current directory

- Calculates pairwise cosine similarity between documents

- Uses TF-IDF (Term Frequency-Inverse Document Frequency) for text vectorization

- Outputs similarity scores between each pair of student files

- Helps identify potential cases of plagiarism in written content

## 🧠 What This Script Does
- Reads all .txt files in the current folder (each representing a student's submission).

- Vectorizes the text using TfidfVectorizer from scikit-learn.

- Computes pairwise cosine similarity between all documents.

- Prints similarity scores between all student file pairs.

- A high similarity score (closer to 1.0) indicates greater overlap between two files and possible plagiarism.

## 🛠 Requirements
- Python 3.x

- scikit-learn

- Install dependencies using:

      pip install scikit-learn

## 🚀 How to Run
1. Place your student .txt files in the same directory as the script.

2. Run the script using:

       python plagiarism_checker.py

3. The output will show similarity scores like:

       ('Arthur.txt', 'Ben.txt', 0.459)
       ('Arthur.txt', 'Clark.txt', 0.543)
       ...
