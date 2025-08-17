# Next-Word Prediction & Auto-Correction Engine

**Authors:** Shoumik Das (24N0457), Sandipan Mondal (24N0457)

------------------------------------------------------------------------

## Abstract

This project presents the design and implementation of an Advanced NLP
Auto-Correction & Prediction System. It focuses on correcting misspelled
words and suggesting predictive completions using Natural Language
Processing (NLP) techniques. The system integrates phonetic matching,
edit distance, and frequency-based ranking to achieve accurate results.
This report outlines the methodology, performance, and practical
applications of the system.

------------------------------------------------------------------------

## 1. Introduction

Spelling errors and incomplete word inputs are common in digital
communication. An intelligent system that automatically corrects
mistakes and predicts the intended word can significantly improve typing
efficiency and user experience. This project builds upon classical NLP
techniques and modern enhancements to develop a lightweight, accurate,
and real-time correction and prediction tool.

------------------------------------------------------------------------

## 2. Methodology

### 2.1 Data Preprocessing

The corpus is loaded and cleaned by removing special characters,
converting to lowercase, and tokenizing into words. A frequency
dictionary is created to prioritize common words.

### 2.2 Auto-Correction Algorithm

The auto-correction pipeline combines: - **Phonetic Encoding (Double
Metaphone):** captures similar sounding words.\
- **Edit Distance (Levenshtein):** measures similarity between user
input and candidate words.\
- **Frequency Ranking:** selects the most probable correction from
frequent candidates.

### 2.3 Prediction Mechanism

The system predicts likely next words using: - **Word co-occurrence
statistics (bigram probabilities).**\
- **Context-aware ranking** to ensure predictions match common usage.

------------------------------------------------------------------------

## 3. Results & Observations

The system was tested on a sample English corpus. It successfully
corrected common spelling errors such as *"recieve" → "receive"* and
*"enviroment" → "environment"*. Prediction accuracy was around
**70--80%** for frequent word pairs. Performance was efficient,
requiring less than **0.1s** for single-word correction on a standard
machine.

------------------------------------------------------------------------

## 4. Applications & Limitations

### Applications:

-   Spell-check in text editors and messaging apps.\
-   Intelligent typing assistance in mobile keyboards.\
-   Pre-processing tool for NLP pipelines.

### Limitations:

-   Accuracy depends on corpus size and quality.\
-   Context-awareness is limited compared to deep learning models.\
-   Complex grammar-level corrections are not handled.

------------------------------------------------------------------------

## 5. Conclusion

The project demonstrates that a hybrid NLP system combining phonetics,
edit distance, and frequency analysis can deliver strong performance for
auto-correction and prediction tasks. Future improvements may include
integration of deep learning models (e.g., LSTMs, Transformers) for
context-sensitive predictions.
