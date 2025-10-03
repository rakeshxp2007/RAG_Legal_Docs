```markdown
# RAG Legal Documents Pipeline

This repository implements a **Retrieval-Augmented Generation (RAG) pipeline** for extracting and analyzing information from legal documents. The project demonstrates data cleaning, exploratory analysis, chunking, embedding, building a vector database, setting up a RAG QA chain, and evaluating performance with legal benchmarks.

---

## 📋 Project Objective

- **Process and analyze legal agreements** (e.g., NDAs) to enable question-answering using a RAG approach.
- Prepare data, explore insights, and evaluate system performance using relevant metrics.

---

## 🚀 Process Pipeline Overview

Below is a summary table of the stepwise process followed in this repository:

| **Step**                    | **Activity**                                                                                     |
|-----------------------------|--------------------------------------------------------------------------------------------------|
| Data Loading/Preparation    | Load `.txt` files, preprocess for noise, normalize text, handle errors                           |
| Exploratory Analysis        | Document stats, word frequency, TF-IDF similarity analysis                                       |
| Document Chunking           | Split documents into overlapping chunks for retrieval                                            |
| Vector Database & Embedding | Generate OpenAI embeddings, store in ChromaDB                                                    |
| RAG Pipeline Setup          | Create a retriever & LLM; set up RAG chain using LangChain                                       |
| QA Function                 | Function to answer queries, returning both generated answer and source docs                      |
| Evaluation                  | Extract benchmarks, run evaluation (ROUGE, BLEU, RAGAS), summarize metrics                       |
| Insights & Conclusions      | Assess pipeline, suggest improvements (semantic fidelity, relevance, chunking strategies)        |

---

## 📂 Folder Structure

- `contractnli/`, `cuad/`, `maud/`, `privacyqa/` — cleaned legal documents (text files)
- `evaluation/` — benchmark question/answer JSON files
- `notebooks/` — Jupyter notebook documenting stepwise pipeline
- `vector_db/` — ChromaDB vector database and embeddings

---

## 📊 Evaluation Metrics

- **Linguistic Overlap**: ROUGE-L, BLEU scores
- **Quality Metrics**: RAGAS (context precision/recall, faithfulness, answer relevancy)
- **Testing**: First 100 questions from each benchmark category

---

## ✨ Key Insights

- **Semantic fidelity**: RAG pipeline produces contextually accurate answers.
- **Metrics**: RAGAS metrics are preferred for legal QA over BLEU/ROUGE.
- **Improvement areas**: Chunking strategy and retrieval process can further boost precision/recall.

---

## 💡 Getting Started

1. Prepare your environment (see `requirements.txt`).
2. Run the notebook stepwise to process data and build the pipeline.
3. Evaluate using sample benchmarks.

---

## 📞 Contact

Project by Rohit Vashishth, Saurabh Singh, Ankita Mhargude, Rakesh Kumar Sahoo.

```
This Markdown README is formatted for GitHub and highlights the summary pipeline table as requested. You can copy this as `README.md` for your repository!

[1](https://www.perplexity.ai/finance/NVDA)
