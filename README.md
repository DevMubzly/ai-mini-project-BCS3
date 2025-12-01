# SMS Spam Detection (Group 3)

Final class project: trained SMS spam classifier delivered as a scikit‑learn Pipeline plus a Streamlit app for real‑time classification.

## Overview

- Preprocessing dataset (normalize labels, remove duplicates/nulls).
- Training multiple TF‑IDF + classifier pipelines.
- Selecting best model by F1 score on test data.
- Exporting model, metadata, and comparison metrics.
- Providing a simple web interface for message checking.

## Workflow

1. Run the notebook to train and export artifacts.
2. Start the Streamlit app to classify new SMS messages.

## Setup

Install dependencies:

```powershell
pip install -r requirements.txt
```

Train by executing all cells:

```powershell
jupyter nbconvert --to notebook --execute spam_detection.ipynb
```

Launch app:

```powershell
streamlit run app.py
```

## Using the App

- Enter an SMS message.
- Click Classify.
- Output: SPAM or Not Spam with confidence (probability) or decision score.
