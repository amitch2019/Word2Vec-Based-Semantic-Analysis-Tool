# Word2Vec-Based-Semantic-Analysis-Tool
This project implements a sophisticated natural language processing tool leveraging word embeddings (Word2Vec) to analyze word similarities and relationships. It demonstrates proficiency in handling large datasets, efficient data processing, and applying advanced NLP techniques.


# Word Similarity and Relationships

## Project Overview

This project leverages the advances in natural language processing through word2vec (word embeddings) to study the similarity between words. Utilizing Stanford's GloVe project data, the project implements a robust system for finding similar words and solving word analogies. This project showcases skills in handling large datasets, natural language processing, and implementing efficient algorithms.

## Key Features

1. **Word Similarity Search**:
   - **Find Closest Words**: Given a word, find the n closest words based on word vector similarities.
   - **Partial Analogies**: Solve analogies of the form "x is to y as z is to _____".

2. **Efficient Data Handling**:
   - Preprocess large word vector files into efficient binary formats using NumPy for faster loading and processing.

3. **Interactive Command-Line Interface**:
   - Provides a user-friendly command-line interface for entering words or partial analogies and getting real-time results.

4. **Advanced Visualization**:
   - Optional visualization of word vectors using PCA to project high-dimensional data into 2D space, enhancing understanding of word relationships.

## Technologies Used

- **Python**: Core programming language for implementation.
- **NumPy**: For efficient numerical computations and data storage.
- **Matplotlib**: For optional visualization of word vectors.
- **Scikit-learn**: For PCA in visualizing word vectors.

## Implementation Details

### 1. Data Preprocessing (`save_np.py`)
- Converts the GloVe word vector text file into a binary format using NumPy for efficient storage and quick loading.
- Saves the word vectors into `glove.42B.300d.npy` and the vocabulary list into `glove.42B.300d.vocab.txt`.

### 2. Word Similarity and Analogy (`wordsim.py`)
- **Find Closest Words**:
    ```python
    def closest_words(gloves, word, n):
        """
        Given a gloves dictionary of word:vector and a word, return the n nearest words
        based on Euclidean distance between word vectors.
        """
    ```

- **Solve Word Analogies**:
    ```python
    def analogies(gloves, x, y, z, n):
        """
        Given a gloves dictionary of word:vector and 3 words from
        "x is to y as z is to _____", return the n best words that fill in the blank.
        """
    ```

### 3. Command-Line Interface (`wordsim.py`)
- Main program to interactively query word similarities and analogies from the user.
- Handles user input, processes the GloVe data, and outputs results in real-time.

## Challenges and Solutions

1. **Handling Large Datasets**: 
   - Preprocessed large GloVe word vector files into a more efficient binary format to speed up data loading.
   
2. **Efficient Similarity Computations**:
   - Implemented Euclidean distance calculations and vector arithmetic for fast and accurate word similarity and analogy solving.

3. **Interactive User Interface**:
   - Developed a command-line interface for a seamless user experience.

## Future Improvements

1. Implement more advanced text processing techniques (e.g., stemming, removing stop words).
2. Enhance analogy solving with support for more complex queries.
3. Develop a web-based front-end for a more intuitive user interface.
4. Optimize further by incorporating parallel processing for large datasets.

## Installation and Usage

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/word-similarity-relationships.git
    ```

2. **Navigate to the project directory**:
    ```bash
    cd word-similarity-relationships
    ```

3. **Preprocess the GloVe data**:
    ```bash
    python save_np.py ~/data
    ```

4. **Run the word similarity and analogy program**:
    ```bash
    python wordsim.py ~/data
    ```

### Access to Code

- The source code for this project is **not publicly available at the moment.**
- However, it **can be shared with interested persons upon request.**
- Please contact me directly to request access to the code.

---
