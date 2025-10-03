<img width="512" height="512" alt="RAG_Chatbot_Icon" src="https://github.com/user-attachments/assets/790dc642-1a00-415a-8820-3ebb37014cfb" />

# Legal Documents Analysis Chatbot - Using RAG

This repository showcases a **Retrieval-Augmented Generation (RAG) powered chatbot** designed specifically for analyzing and answering questions from legal documents. It enables users to interactively query a corpus of legal agreements, with the chatbot retrieving and generating context-aware, accurate responses based on the underlying documents.

The project encompasses data cleaning, exploratory analysis, efficient document chunking, vector embedding, database creation using ChromaDB, and the full pipeline for retrieval-augmented Q&A. Extensive evaluation is performed with relevant legal benchmarks to ensure high answer relevancy and faithfulness.

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

## 📊 Evaluation Results

| **Metric**          | **Score**  | **Sticker**    |
|---------------------|------------|---------------|
| ROUGE-L             | 0.2217     | 🟠 Moderate    |
| BLEU                | 0.0394     | 🟠 Low         |
| Context Precision   | 0.5209     | 🟡 Medium      |
| Context Recall      | 0.6350     | 🟡 Medium      |
| Faithfulness        | 0.8637     | 🟢 High        |
| Answer Relevancy    | 0.9085     | 🟢 High        |

- 🟢 **High**: Indicates excellent results.
- 🟡 **Medium**: Indicates satisfactory results but improvement possible.
- 🟠 **Low/Moderate**: Indicates areas for further optimization.

---

## ✨ Key Insights

- **Semantic fidelity**: RAG pipeline produces contextually accurate answers.
- **Metrics**: RAGAS metrics are preferred for legal QA over BLEU/ROUGE.
- **Improvement areas**: Chunking strategy and retrieval process can further boost precision/recall.

---

## 📞 Contact

Project by Rohit Vashishth, Saurabh Singh, Ankita Mhargude, Rakesh Kumar Sahoo.


