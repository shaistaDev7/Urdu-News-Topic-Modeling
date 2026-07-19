# BERTopic for Urdu News: A Benchmark Study on Classical and Neural Topic Modeling Techniques

## Overview

This repository contains the complete implementation of the research presented in the manuscript:

**"BERTopic for Urdu News: A Benchmark Study on Classical and Neural Topic Modeling Techniques."**

The project provides a comprehensive benchmarking framework for topic modeling on Urdu news articles by comparing traditional statistical topic modeling techniques with modern neural topic modeling approaches.

The repository includes:

- Data preprocessing pipeline
- BERTopic implementation
- Classical topic modeling algorithms
- Neural topic modeling algorithms
- Evaluation metrics
- Experimental scripts
- Result generation
- Visualization scripts

This repository is intended to ensure the reproducibility of all experiments reported in the manuscript.

---

# Table of Contents

- Project Structure
- Dataset Information
- Code Information
- Installation
- Requirements
- Usage
- Methodology
- Evaluation
- Results
- Reproducibility
- Citation
- License
- Contribution
- Contact

---

# Project Structure

```
Urdu-News-Topic-Modeling/
│
├── Data/
│   ├── Raw/
│   ├── Processed/
│   └── Embeddings/
│
├── Preprocessing/
│
├── BERTopic/
│
├── LDA/
│
├── NMF/
│
├── CTM/
│
├── LSA/
│
├── Evaluation/
│
├── Visualization/
│
├── Results/
│
├── Figures/
│
├── requirements.txt
│
├── README.md
│
└── LICENSE
```

---

# Dataset Information

This study utilizes the **Urdu Digest Corpus (UDC)** as the primary dataset.

The corpus consists of Urdu news articles collected from multiple news categories.

Please refer to the manuscript for detailed dataset statistics.

If the dataset cannot be redistributed due to licensing restrictions, please download it from the original source.

After downloading, place the dataset inside:

```
Data/Raw/
```

Dataset statistics used in this study include:

- Number of Documents
- Number of Categories
- Vocabulary Size
- Total Tokens

(These values are reported in the manuscript.)

---

# Code Information

The repository contains implementations of the following topic modeling approaches.

| Model | Description |
|--------|-------------|
| BERTopic | Transformer-based topic modeling |
| LDA | Latent Dirichlet Allocation |
| NMF | Non-negative Matrix Factorization |
| LSA | Latent Semantic Analysis |
| CTM | Contextual Topic Model |

Additional scripts include:

- Data preprocessing
- Text cleaning
- Embedding generation
- Topic extraction
- Topic visualization
- Model evaluation

---

# Installation

Clone the repository

```bash
git clone https://github.com/shaistaDev7/Urdu-News-Topic-Modeling.git
```

Move to the project directory

```bash
cd Urdu-News-Topic-Modeling
```

Create a virtual environment

```bash
python -m venv venv
```

Activate the environment

Windows

```bash
venv\Scripts\activate
```

Linux / macOS

```bash
source venv/bin/activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# Requirements

Python 3.10 or higher

Major libraries

- bertopic
- sentence-transformers
- umap-learn
- hdbscan
- gensim
- scikit-learn
- pandas
- numpy
- matplotlib
- seaborn
- plotly
- nltk
- scipy

---

# Usage

## Step 1

Download the dataset and place it in

```
Data/Raw/
```

---

## Step 2

Run preprocessing

```bash
python preprocessing.py
```

---

## Step 3

Train BERTopic

```bash
python bertopic_model.py
```

---

## Step 4

Train baseline models

```bash
python lda.py

python nmf.py

python lsa.py

python ctm.py
```

---

## Step 5

Evaluate models

```bash
python evaluation.py
```

---

## Step 6

Generate visualizations

```bash
python visualization.py
```

---

# Methodology

The workflow implemented in this repository consists of the following stages.

1. Dataset collection
2. Data preprocessing
3. Urdu text normalization
4. Tokenization
5. Stop-word removal
6. Sentence embedding generation
7. BERTopic modeling
8. Classical topic modeling
9. Neural topic modeling
10. Topic evaluation
11. Performance comparison
12. Visualization of results

---

# Evaluation

The models are evaluated using the following metrics.

- Topic Coherence
- Topic Diversity
- Number of Topics
- Topic Quality
- Execution Time

The proposed BERTopic model is compared with

- LDA
- NMF
- LSA
- CTM

Evaluation scripts are provided in the repository.

---

# Results

The repository reproduces the experiments reported in the manuscript.

Generated outputs include:

- Topic lists
- Topic keywords
- Interactive topic visualization
- Topic hierarchy
- Topic similarity
- Performance comparison tables
- Figures used in the manuscript

---

# Reproducibility

To ensure complete reproducibility:

- All source code is included.
- Experimental scripts are provided.
- Hyperparameters are documented.
- Library dependencies are listed.
- Random seeds are fixed where applicable.
- Evaluation scripts are included.

Running the scripts in the order described above should reproduce the experimental results reported in the paper.

---

# Citation

If you use this repository in your research, please cite:

```
Shaista Zulfiqar et al.

BERTopic for Urdu News:
A Benchmark Study on Classical and Neural Topic Modeling Techniques.

PeerJ Computer Science (Under Review)
```

If accepted, please update this section with the final DOI.

---

# License

This repository is released under the MIT License unless otherwise specified.

See the LICENSE file for details.

---

# Contribution

Contributions are welcome.

If you find a bug or would like to improve the repository:

1. Fork the repository.
2. Create a new branch.
3. Commit your changes.
4. Submit a Pull Request.

Please include a clear description of your proposed modifications.

---

# Contact

**Shaista Zulfiqar**

Government College Women University Sialkot

Email: your_email@example.com

GitHub:
https://github.com/shaistaDev7

---

## Acknowledgements

This work was developed as part of research on benchmark topic modeling for low-resource Urdu language datasets.

We acknowledge the developers of:

- BERTopic
- Sentence Transformers
- Scikit-learn
- Gensim
- UMAP
- HDBSCAN

whose open-source software made this work possible.