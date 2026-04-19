# 123-XXXX-NLP-Assignment2

NLP Assignment 2 — Neural NLP Pipeline built on BBC Urdu news data.
Course: CS-4063 | FAST NUCES

## Structure
├── data/               # CoNLL annotation files (POS & NER)
├── embeddings/         # TF-IDF, PPMI, Word2Vec matrices
├── models/             # Saved PyTorch model weights
├── 123-XXXX_Assignment2_DS-X.ipynb
└── report.pdf

## How to Reproduce

1. **Install dependencies**
```bash
   pip install torch numpy scikit-learn matplotlib
```

2. **Add data files** — place `cleaned.txt` and `Metadata.json` in the root directory.

3. **Run the notebook** — execute all cells top to bottom in order:
   - Part 1: Word Embeddings (TF-IDF → PPMI → Word2Vec)
   - Part 2: BiLSTM POS Tagger & NER with CRF
   - Part 3: Transformer Encoder for Topic Classification

## Notes

- All models implemented from scratch using PyTorch only
- No pretrained models, Gensim, or HuggingFace used
- Tested on Python 3.10+, PyTorch 2.x
