# NLP--1-Build-a-Robust-NLP-Preprocessing-Engine-Advanced

Task 1: Conceptual Understanding
1. Difference between "Love" and "love" in NLP
In raw NLP, "Love" and "love" are treated as different tokens due to case sensitivity.
This increases vocabulary size unnecessarily.
After normalization (lowercasing), both become the same → improves consistency.
2. What happens if stopwords are not removed?
The model may:
Focus on irrelevant words (e.g., "the", "is", "and")
Increase computational cost
Reduce model performance due to noise
3. Two real-world scenarios where removing stopwords is harmful
Sentiment Analysis
Example: "I am not happy"
Removing "not" changes meaning completely
Question Answering Systems
Example: "What is the capital of France?"
Removing "what" or "is" breaks sentence structure
4. Difference between Stemming and Lemmatization
Feature	Stemming	Lemmatization
Approach	Rule-based cutting	Dictionary-based
Output	May not be real word	Always meaningful word
Example	"running" → "run"	"running" → "run"
Example	"better" → "better"	"better" → "good"
📌 Overview
This project implements a **robust NLP preprocessing pipeline** designed to clean and transform noisy real-world text into structured and meaningful tokens.

The solution is built as part of an internship assessment and demonstrates handling of:
* Noisy text
* Emojis
* URLs
* Repeated characters
* Token analytics
* Frequency analysis

 🎯 Objectives
* Build a scalable preprocessing pipeline
* Handle real-world text noise
* Normalize text efficiently
* Perform token-level analytics
* Write clean and modular Python code

✅ Text Cleaning
* Convert text to lowercase
* Remove URLs and email patterns
* Remove numbers
* Remove special characters & emojis
* Remove extra spaces

✅ Advanced Processing
* Handle repeated characters (e.g., *loooove → love*)
* Remove short tokens (≤ 2 characters)
* Preserve meaningful words like **"no"** and **"not"**

