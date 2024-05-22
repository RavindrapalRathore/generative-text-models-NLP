# Repository Description: Automated PDF to MCQ Generator

## Overview
This repository contains a Python script designed to automatically generate multiple-choice questions (MCQs) from PDF documents. The script reads the text from a PDF file, processes it using Natural Language Processing (NLP) with spaCy, and then generates MCQs with four options, including two correct answers. The MCQs are generated based on the TF-IDF scores and cosine similarity of sentences within the document.

## Features
- **PDF Text Extraction**: Utilizes PyMuPDF (`fitz`) to read text from PDF files.
- **NLP Processing**: Leverages spaCy for tokenizing and processing text.
- **TF-IDF Vectorization**: Uses `TfidfVectorizer` from scikit-learn to compute TF-IDF scores of sentences.
- **Cosine Similarity Calculation**: Computes the similarity between sentences to find the most relevant options.
- **MCQ Generation**: Generates multiple-choice questions with four options, ensuring two correct answers.

## Dependencies
- Python 3.6+
- PyMuPDF
- spaCy
- scikit-learn

## Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/pdf-to-mcq-generator.git
cd pdf-to-mcq-generator
```

### 2. Install Required Packages
```bash
pip install fitz spacy scikit-learn
python -m spacy download en_core_web_sm
```

### 3. Add PDF Files
Place the PDF files you want to process in the `/content` directory.

### 4. Run the Script
```bash
python generate_mcqs.py
```
