# Computational-Linguistics
Computational Linguistics project (A.A. 2023-2024) @ University of Pisa. Textual and statistical analysis of two English corpora using Python &amp; NLTK

## 🎯 Project Objective
Development of two programs (implemented as Jupyter Notebooks) that utilize **NLTK** library modules to linguistically analyze two corpora, compare them based on statistical indices, and extract advanced information.

## 📂 Corpora Structure
The analyzed corpora meet the following requirements:
- **Language:** English.
- **Size:** At least 5,000 words each.
- **Format:** Plain text files with UTF-8 encoding.

## 💻 Developed Programs

### 🔹 Program 1: Corpus Comparison
Takes both corpora as input and performs linguistic annotation tasks (*sentence splitting, tokenization, PoS tagging, lemmatization*) to produce a comparative analysis based on:
1. Total number of sentences and tokens.
2. Average sentence length (in tokens) and average token length (in characters, excluding punctuation).
3. Hapax count (total and within incremental slices of 500, 1,000, and 3,000 tokens).
4. Vocabulary size and lexical richness (Type-Token Ratio - TTR), calculated incrementally every 200 tokens up to the full text.
5. Number of distinct lemmas (lemma vocabulary size).
6. Distribution of positive and negative sentiment sentences using a polarity classifier.

### 🔹 Program 2: Information Extraction
Executed individually on each of the two corpora, this program extracts:
1. The top-50 most frequent Nouns, Adverbs, and Adjectives (ordered by decreasing frequency).
2. The top-20 most frequent n-grams (for $n$ from 1 to 5) and top-20 PoS n-grams (for $n$ from 1 to 3).
3. The top-10 Adjective-Noun bigrams, ordered by: Frequency, Maximum Conditional Probability, Maximum Joint Probability, Maximum Mutual Information (MI), and Maximum Local Mutual Information (LMI), including the count of overlapping elements between the top-10 MI and LMI.
4. Analysis of sentences between 10 and 20 tokens long (where at least half of the tokens occur $\ge 2$ times in the corpus) to identify: the sentence with the highest average token frequency, the sentence with the lowest average token frequency, and the most probable sentence according to a second-order Markov model.
5. Extracted Named Entities (NE), identifying the 15 most frequent elements for each NE class.
