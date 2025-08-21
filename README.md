# Clinical-QA-with-RAG-and-Semantic-Evaluation

**Overview:**
This project implements a Retrieval-Augmented Generation (RAG) pipeline for answering clinical guideline questions using LangChain, FAISS, and OpenAI embeddings. It integrates GPT-based response generation and evaluates semantic accuracy using BERTScore with roberta-large, enabling robust benchmarking of healthcare QA systems.

**Features:**
- End-to-end RAG pipeline built in Google Colab
- Document chunking and semantic embedding using OpenAI
- Vector search with FAISS for efficient context retrieval
- GPT-powered answer generation via LangChain's ChatOpenAI
- Semantic evaluation using BERTScore F1 scores
- Logging and flagging of borderline cases for manual review

**Dataset:**
The pipeline ingests a CSV file (cpgQA-v1.0) containing clinical guideline questions, titles, and context passages. These are preprocessed and embedded for retrieval and QA.

**Evaluation:**
Semantic accuracy is measured using BERTScore, comparing generated answers to ground truth references. Scores above 0.90 indicate strong alignment, supporting clinical relevance and factual correctness.

**Applications:**
This project is designed for researchers and practitioners in health informatics, NLP, and policy analysis. It supports benchmarking of QA systems on real-world clinical data and can be extended to other domains.
