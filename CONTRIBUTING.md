# Contributing to arabic-mini-llm

## Where files go

| Folder | What goes here | Owner(s) |
|--------|----------------|----------|
| `data/` | Cleaning and collection code, data stats, source/license inventory (not the data itself) | Data Engineering |
| `src/` | Training, tokenizer and evaluation code | Training & Optimization, Evaluation |
| `configs/` | Model, tokenizer and training configs | Training & Optimization |
| `notebooks/` | Colab / Jupyter notebooks | Everyone |
| `docs/` | Data card, model card, run guides, weekly reports | Documentation & Support |
| `results/` | Experiment log, evaluation results, sample outputs | Evaluation, Documentation |

## Rules

1. **Do not push large files** (datasets, checkpoints, model weights). Put them on the shared Google Drive or HuggingFace and link to them.
2. **Do not push secrets** (API keys, tokens, `.env`).
3. Use clear file names, for example `clean_batch1.py`, not `final2_new.py`.
4. Write a short, clear commit message saying what changed.
5. Pull before you push: `git pull` then `git push`.
6. If unsure where something belongs, ask the MLOps owner (Mohamed Lakhdar Khalifia).

## Run from a fresh environment

```bash
git clone https://github.com/<org-or-user>/arabic-mini-llm.git
cd arabic-mini-llm
pip install -r requirements.txt
```

Run instructions for training will be added here once the code and config are merged.
