# Graph-Structured Diffusion Model for Legal Document Summarization

## Project Overview

This project focuses on developing an intelligent legal document summarization system for Indian legal judgments using Natural Language Processing, Knowledge Graphs, Graph Neural Networks, and Transformer-based architectures.

The proposed framework combines semantic representations, multi-relational graph construction, graph diffusion, and hybrid extractive–abstractive summarization to generate concise, context-aware, and legally faithful summaries.

## Proposed Methodology

The system follows a multi-stage pipeline:

1. **Data Preprocessing:** Cleaning and preparing Indian legal judgments for further processing.
2. **Sentence Chunking and Embeddings:** Generating contextual sentence representations using InLegalBERT.
3. **Named Entity Recognition:** Extracting legal entities such as judges, courts, statutes, and case references.
4. **Graph Construction:** Building enriched sentence graphs using shared-entity, semantic similarity, and sequential relationships.
5. **Relational GNN:** Applying Relational Graph Attention Networks to learn sentence importance and contextual dependencies.
6. **Graph Diffusion:** Refining sentence importance scores through information propagation across the graph.
7. **MMR-Based Selection:** Selecting relevant sentences while reducing semantic redundancy.
8. **Abstractive Summarization:** Generating coherent summaries using long-document transformer models such as LED/BART.
9. **Factual Verification:** Incorporating entity-aware generation and Natural Language Inference (NLI) to improve factual consistency.

## Technology Stack

- **Language:** Python
- **Environment:** Google Colab, Jupyter Notebook
- **NLP:** spaCy, Hugging Face Transformers
- **Language Model:** InLegalBERT
- **Deep Learning:** PyTorch
- **Graph Learning:** PyTorch Geometric, Relational GAT
- **Summarization:** LED / BART
- **Evaluation:** ROUGE, BERTScore, Entity Hallucination Rate
- **Version Control:** Git, GitHub

## Repository Structure

```text
legal-document-summariser/
│
├── notebooks/       # Implementation notebooks
├── src/             # Reusable source code
├── data/            # Dataset references
├── results/         # Experimental results
├── docs/            # Project documentation
│
├── README.md
├── requirements.txt
└── .gitignore
```

## Current Progress

| Module | Status |
|---|---|
| Data Preprocessing | Completed |
| Sentence Chunking | Completed |
| Embedding Generation | Completed |
| Named Entity Recognition | Completed |
| Graph Construction | Completed |
| GNN Training | In Progress |
| Graph Diffusion | Upcoming |
| MMR-Based Selection | Upcoming |
| Abstractive Summarization | Upcoming |
| Evaluation and Verification | Upcoming |

## Evaluation Strategy

The proposed framework will be evaluated using:

- ROUGE-1, ROUGE-2 and ROUGE-L
- BERTScore for semantic similarity
- Entity hallucination rate
- Entity recall and factual consistency
- Comparative evaluation against extractive and transformer-based baselines

## Research Objective

The primary objective is to develop a graph-enhanced hybrid summarization framework that captures semantic relationships, legal context, and document structure while minimizing redundancy and preserving factual accuracy in generated legal summaries.

---

**Institution:** PES University

**Department:** Computer Science and Engineering (AI & ML)

**Project ID:** PW25_JR_07

**Project Guide:** Dr. Jayashree R

**Project Team:**
- Swayam Advani
- Tanuushree M
- Gahnavi B
- Tharun M.S.