# Document-summarisation-using-transformers
Overview

This project implements an end-to-end document summarization pipeline using Transformer-based models from Hugging Face.
Given any text document, it produces a concise and coherent summary while preserving key information.

The pipeline handles:
	•	Text cleaning and preprocessing
	•	Chunking of long documents
	•	Summarization using BART (facebook/bart-large-cnn)
	•	Easy inference for new documents

This project demonstrates practical skills in NLP, Python pipelines, and Transformer-based deep learning models.

⸻

Objectives
	•	Preprocess raw text for summarization
	•	Split long documents into manageable chunks
	•	Generate summaries using state-of-the-art Transformer models
	•	Combine chunk summaries into a final output
	•	Provide a reusable pipeline for production-ready inference

⸻

Tech Stack
	•	Language: Python 3.10+
	•	Libraries:
	•	transformers, torch, sentencepiece
	•	nltk
	•	Environment: Jupyter Notebook, Python scripts

⸻

Project Structure

document-summarization/
│
├── data/
│   └── sample.txt             # Example document
│
├── src/
│   ├── preprocess.py          # Text cleaning and chunking
│   ├── summarize.py           # Summarization pipeline
│   └── inference.py           # Summarize new documents
│
├── notebooks/
│   └── 01_demo.ipynb          # Demo notebook
│
├── requirements.txt
└── README.md


⸻

Setup Instructions

1. Clone repository

git clone https://github.com/<your-username>/document-summarization.git
cd document-summarization

2. Create virtual environment

python -m venv venv
source venv/bin/activate       # macOS/Linux
venv\Scripts\activate          # Windows

3. Install dependencies

pip install -r requirements.txt

4. Add sample document

Place your text file inside the data/ folder (e.g., sample.txt).

⸻

How to Run

Summarize a document

python src/inference.py

The script reads data/sample.txt by default and prints the generated summary.

Example Notebook

Run notebooks/01_demo.ipynb to:
	•	Load a document
	•	Display the original text
	•	Generate and display the summary

⸻

Features
	•	Modular and reusable Python code
	•	Handles long documents via chunking
	•	Uses state-of-the-art Transformer model (BART)
	•	Easy to adapt to other models (e.g., T5)
	•	Compatible with CPU and GPU

⸻

Extensions
	•	Build a REST API using Flask or FastAPI for document summarization
	•	Integrate into a web or desktop application
	•	Fine-tune the model on domain-specific datasets for better performance
	•	Add evaluation metrics (ROUGE scores) for automated testing

⸻

