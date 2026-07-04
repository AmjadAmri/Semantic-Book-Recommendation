# Semantic Book Recommendation System

An AI-powered semantic book recommendation system that retrieves relevant books by understanding the meaning of natural-language queries using transformer embeddings and vector similarity search, rather than relying on traditional keyword matching.

The system converts both user queries and book descriptions into dense vector embeddings using Sentence Transformers, performs efficient similarity search with ChromaDB, and ranks the most relevant books through a semantic retrieval pipeline.
<p align="center">
  <img src="https://img.shields.io/badge/Python-3.12-blue?logo=python" alt="Python">
  <img src="https://img.shields.io/badge/Sentence_Transformers-all--MiniLM--L6--v2-FF6F00" alt="Sentence Transformers">
  <img src="https://img.shields.io/badge/ChromaDB-Vector_Database-5B21B6" alt="ChromaDB">
  <img src="https://img.shields.io/badge/Hugging_Face-Transformers-FFD21E?logo=huggingface" alt="Transformers">
  <img src="https://img.shields.io/badge/Gradio-Web_Interface-F97316" alt="Gradio">
  <img src="https://img.shields.io/badge/Information_Retrieval-Evaluation-14B8A6" alt="Evaluation">
</p>

## Overview

Traditional book recommendation systems often rely on keywords, genres, or manually assigned categories, which may fail to capture the actual meaning behind a user's request.

This project introduces an AI-powered semantic recommendation system that understands natural-language descriptions and retrieves books based on semantic similarity rather than exact keyword matching.

The system leverages Sentence Transformers to generate dense vector embeddings for both user queries and book descriptions, stores embeddings in ChromaDB for efficient vector retrieval, and returns the most semantically relevant books through an interactive Gradio interface.

## Problem

- Traditional recommendation systems rely primarily on keyword matching and predefined categories.
- Keyword-based search often fails to understand the semantic intent behind user queries.
- Users may struggle to discover books that match themes, emotions, or concepts described in natural language.

## Objectives

- Recommend books using semantic similarity instead of keyword matching.
- Understand natural-language descriptions provided by users.
- Retrieve relevant books efficiently using vector similarity search.
- Provide an intuitive interface for semantic book discovery.

## Key Features

- Semantic book recommendation
- Natural-language query understanding
- Transformer-based sentence embeddings
- Vector similarity search with ChromaDB
- Interactive Gradio interface
- Configurable Top-K recommendations


## Recommendation Pipeline
flowchart LR

A[User Query]
-->B[Sentence Transformer]

B-->C[Query Embedding]

C-->D[ChromaDB Vector Search]

D-->E[Similarity Ranking]

E-->F[Top-K Recommended Books]

## Evaluation Framework

The recommendation pipeline was evaluated using standard information retrieval metrics to assess recommendation quality and retrieval effectiveness.

- Precision@K
- Hit Rate@K
- Normalized Discounted Cumulative Gain (nDCG@K)

## Technology Stack

| Category | Technologies |
|----------|--------------|
| Programming Language | Python |
| Embedding Model | Sentence Transformers (all-MiniLM-L6-v2) |
| Vector Database | ChromaDB |
| NLP Framework | Hugging Face Transformers |
| User Interface | Gradio |
| Data Processing | Pandas, NumPy |
| Evaluation | Precision@K, Hit Rate@K, nDCG@K |


### Semantic Book Recommendation Interface

<p align="center">
<img src="https://github.com/user-attachments/assets/4c6e9830-488f-469f-baf8-56dec8e098c6" width="900">
</p>


## Future Improvements

- Integrate Large Language Models (LLMs) to generate personalized book recommendations and explanations.
- Implement hybrid recommendation by combining semantic search with collaborative filtering.
- Support multilingual book recommendations.
- Incorporate user profiles and reading history for personalized recommendations.
- Expand the recommendation pipeline with Retrieval-Augmented Generation (RAG).
- Deploy the system as a cloud-hosted web application.

