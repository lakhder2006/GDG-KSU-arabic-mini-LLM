# GDG-KSU-arabic-mini-LLM
# arabic-mini-llm

**Arabic Mini-LLM** is the third project of the Technical Committee at **GDG KSU** (Google Developer Groups, King Saud University). It aims to build a small, open Arabic language model, trained on carefully selected Arabic data with clear licensing.

## Project Idea

Instead of writing a Transformer from scratch, the project relies on an **open-source architecture** and puts its effort into **data quality and training**. The final output is a small Arabic model published under the GDG KSU name, together with a documented dataset and transparent evaluation results.

**Open decision:** train a small model from scratch using an open architecture, or continue training an open base model such as Gemma (Apache 2.0, trained on 140+ languages). The choice depends on the available compute.

## Project Files (Google Drive)

Datasets, documents, and project materials:

[Open the Drive folder](https://drive.google.com/drive/folders/1jDCJQUgvbcXEo1IT1TK9sho7fpU9oS2q)

## Deliverables

| # | Requirement | Details |
|---|-------------|---------|
| R1 | Source and license inventory | Every data source is listed with its license; sources with unclear licenses are excluded |
| R2 | Data quality pipeline | Arabic normalization, language ID, quality filters, deduplication, personal-data removal |
| R3 | Dataset release | Versioned dataset with a data card on HuggingFace |
| R4 | Approach and tokenizer decision | From scratch or continued training; reuse the base model tokenizer or train an Arabic one |
| R5 | Training | Runs on available resources with checkpoints and experiment tracking |
| R6 | Evaluation | Arabic benchmarks, a human evaluation set, and an eval-leakage check |
| R7 | Release | Model card, license, and code published |

## Tech Stack

- **Framework:** PyTorch + HuggingFace Transformers
- **Training environment:** Google Colab (available resources)
- **Publishing:** HuggingFace Hub + GitHub (GDG KSU)
- **Data:** licensed Arabic sources + NLP_Arabic tools

## Timeline (8 weeks)

| Phase | Weeks | Output |
|-------|-------|--------|
| 1. Data | 1-3 | R1, R2, R4: quality pipeline running on a full sample |
| 2. First data release | 4 | R3: dataset published |
| 3. Training | 5-7 | R5, R6: model beats the agreed baseline |
| 4. Release | 8 | R7: model published with its model card |

**Beyond the MVP:** a Gradio Space demo and a small Arabic instruction-tuning set (P1); a larger model if compute allows (P2).

## Success Metrics

1. A clean Arabic dataset, published with a data card and clear licenses.
2. A trained model with documented checkpoints and training results.
3. Transparent evaluation on Arabic benchmarks plus human evaluation.
4. Open release of the model and code on HuggingFace and GitHub.

## Team

| Name | Role |
|------|------|
| نوره فهد المنصور (Project Lead) | Evaluation |
| شذى الدلبحي | Evaluation |
| شهد أحمد الحيدري | Data Engineering |
| شذى حمد بن مانع | Data Engineering |
| نوره مرعي بن ماضي | Data Engineering |
| خالد سعود العقيلي | Data Engineering |
| نايف محمد المهيد | Training & Optimization |
| محمد أحمد الونيس | Training & Optimization |
| محمد لخضر خلايفية | MLOps & Deployment |
| عبدالله عبدالحليم الرشودي | Technical Documentation & Support |
| محمد إسلام زروطة | Technical Documentation & Support |
| طلال عبدالله اليابس | Technical Documentation & Support |

## Status

Work in progress (PRD v0.5).
