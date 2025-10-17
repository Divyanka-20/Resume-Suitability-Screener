# 📄 Resume Suitability Screener
---

## Overview
A Machine Learning-based Resume Screening Application built with Streamlit, which helps in identifying how suitable a candidate’s resume is for a selected job role.

The app uses Natural Language Processing (NLP) and a Random Forest Classifier to predict how closely a resume aligns with a specific job category.

---

## 🚀 Features
✅ Upload up to 5 resumes (PDF format) at once<br>
✅ Select the target job role (e.g., Data Scientist, Java Developer, HR, etc.)<br>
✅ Automatically extracts and cleans text from resumes<br>
✅ Uses a TF-IDF Vectorizer and Random Forest Model for prediction<br>
✅ Generates an interactive donut chart showing suitability scores<br>
✅ Simple, fast, and completely browser-based (built using Streamlit)<br>

---

## 🧠 Model Details

🔹Algorithms Tried

- Random Forest Classifier (final model) → Best accuracy and stability
- K-Nearest Neighbors (KNN) → Tried but achieved lower accuracy and longer prediction time

🔹 Data Preprocessing

- All resumes were cleaned using a helper script (clean_helper.py)
- Removed punctuation, stopwords, URLs, and special symbols
- Converted text to lowercase
- TF-IDF vectorization used for transforming text data into numerical features

🔹 Output

- Each resume receives a suitability probability score for the selected job role, expressed as a percentage.

---

## 📊 Usage

- Launch the Streamlit interface.
- Select a target job role from the dropdown.
- Upload up to 5 resume PDFs.
- Wait for the system to analyze and process.
- View the donut chart showing how suitable each resume is for the chosen role.

---

## 🛠️ Tech Stack

- Python
- Streamlit (UI)
- scikit-learn (ML model)
- PyPDF2 (Resume text extraction)
- Matplotlib (Visualization)
- Pickle (Model serialization)

---

## 🧹 Resume Cleaning Logic (clean_helper.py)

The text cleaner performs:
- Lowercasing text
- Removing HTML tags, punctuation, and special characters
- Removing stopwords

---
