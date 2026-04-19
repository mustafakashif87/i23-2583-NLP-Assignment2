# i23-2583-NLP-Assignment2

NLP Assignment 2 — Neural NLP Pipeline built on BBC Urdu news data.
Course: CS-4063 | FAST NUCES

## Structure

| Path | Contents |
|------|----------|
| `data/` | `pos_train.conll`, `pos_test.conll`, `ner_train.conll`, `ner_test.conll` |
| `embeddings/` | `tfidf_matrix.npy`, `ppmi_matrix.npy`, `embeddings_w2v.npy`, `word2idx.json` |
| `models/` | `bilstm_pos.pt`, `bilstm_ner.pt`, `transformer_cls.pt` |
| `i23-232583_Assignment2_DS-B.ipynb` | Main notebook (all cells executed) |
| `report.pdf` | Written report |
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
