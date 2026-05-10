# EmoDetection – Academic NLP Project

EmoDetection is our **6th semester NLP academic project** focused on **emotion detection from text**.  
The system performs **multi-label emotion classification** on user-written posts and predicts mental/emotional states.

## Project Objective

The main goal is to detect one or more emotions in a single text sample, which makes this a **multi-label NLP classification** task (not single-class sentiment analysis).

## Emotion Labels

The dataset contains these target labels:

- anger
- brain dysfunction (forget)
- emptiness
- hopelessness
- loneliness
- sadness
- suicide intent
- worthlessness

## Repository Structure

- `Training/`
  - training CSV and embedding files
- `Validating/`
  - validation CSV and embedding files
- `testing/`
  - testing CSV and embedding files
- `NLP-Project-Module-2 (22-SE-21,65,08,102)/`
  - Module 2 work (data preprocessing + baseline models like LSTM/BERT in notebooks)
- `NLP-Project-Module-3(22-SE-21,65,08,102)/`
  - Module 3 work (LLM-oriented experimentation notebook and notes)

## Workflow Summary

1. Load and clean text data.
2. Convert text into vector representations (embeddings).
3. Train multi-label classifiers.
4. Evaluate predictions using common classification metrics (accuracy, precision, recall, F1).
5. Compare model behavior across modules/experiments.

## Implemented Models / Experiments

- **Module 2**
  - Data loading, preprocessing, and embedding preparation
  - Baseline deep learning models (e.g., LSTM)
  - BERT-based experimentation
- **Module 3**
  - Further LLM-oriented experimentation (including embedding-based approach)
  - Notes about RoBERTa compatibility issues in the provided environment

## Data Format

Each dataset row includes:

- a `post` text field
- binary columns for each emotion label (`0` or `1`)

Because multiple labels can be active in one row, predictions are multi-label.

## Academic Context

This repository is maintained as a **course project submission** for NLP.  
It demonstrates the complete pipeline from data preparation to model experimentation and evaluation for emotion detection.

## License

This project is distributed under the terms of the `LICENSE` file in this repository.
