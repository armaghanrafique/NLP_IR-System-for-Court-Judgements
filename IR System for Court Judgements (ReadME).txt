IR System for Court Judgements

📋 Project Overview
A comprehensive Information Retrieval System designed for searching and analysing Pakistan Supreme Court judgements. This system implements multiple retrieval models (Boolean, Vector Space, N-gram) to provide precise, semantic, and phrase-based search capabilities over a corpus of 1,460 legal documents.

🎯 Project Domain
Legal Information Retrieval & Natural Language Processing

🏗️ System Architecture

1. Data Collection & Pre processing Pipeline

Web Scraping (1000 PDFs) → PDF-to-Text Conversion → Text Cleaning → Tokenization → Corpus Creation

2. Multi-Model Search System
-Boolean Retrieval: Traditional AND/OR/NOT logical queries

-Phrase Matching: N-gram based exact phrase search (2-5 grams)

-TF-IDF Vectorization: Semantic similarity search

-Cosine Similarity: Document ranking and clustering

-------✨ Key Features-------

🔍 Search Capabilities
-Boolean Search: Complex logical queries (murder AND evidence, murder OR homicide, murder AND NOT evidence)

-Exact Phrase Search: Multi-word phrase matching

-Wildcard Search: Pattern matching (viol* matches violence, violent, etc.)

-Semantic Search: TF-IDF based similarity search

-Document Similarity: Find similar cases using cosine similarity

📊 Analytics & Visualization

-Term frequency statistics

-Document similarity matrices

-Top-N similar document pairs

-Document clustering

-TF-IDF term importance analysis

🛠️ Technical Features

-Efficient sparse matrix operations

-Batch processing for large datasets

-Interactive command-line interface

-Persistent index storage

-Real-time search with ranking


Supreme Court Judgement Search Engine


Project Description

This project implements a comprehensive Information Retrieval System specifically designed for searching and analysing Pakistan Supreme Court judgements.
Built as a hybrid search engine, it combines multiple retrieval models to provide lawyers, legal researchers, and students with powerful tools for exploring legal precedents, finding relevant case law, and analysing document relationships.
The system processes a corpus of 1,460 legal documents through a complete pipeline from raw PDF collection to sophisticated search capabilities. By integrating Boolean logic, exact phrase matching, and semantic search technologies, it addresses the unique challenges of legal text retrieval, where precision is as important as recall.
Now enhanced with a Document Summarization Module, the system also helps users quickly understand lengthy judgements without reading them in full, saving time and improving research efficiency.

At its core, this project demonstrates practical implementation of Information Retrieval (IR) and Natural Language Processing (NLP) techniques applied to domain-specific legal text. The system features three complementary search models working in harmony: a Boolean Retrieval System for precise logical queries, an N-gram Phrase Matching Engine for exact multi-word searches, and a TF-IDF Vector Space Model for semantic similarity and ranking.
The newly added Document Summarization Module employs both extractive (Text Rank, TF-IDF) and abstractive (transformer-based) methods to generate concise and coherent summaries tailored to legal documents.
What makes this system particularly valuable is its hybrid approach—it doesn't force users to choose between different search paradigms but instead intelligently combines them. For instance, a lawyer can start with a precise Boolean query to narrow down relevant cases, then use semantic search to find conceptually similar judgements that might use different terminology, employ phrase search to locate exact legal formulations within documents, and finally generate a quick summary to grasp the case essence.

Key Features and Capabilities

The search engine supports complex Boolean queries with AND, OR, and NOT operators, allowing for precise filtering of documents. Its phrase matching system uses n-grams (up to 5-word sequences) to find exact legal phrases and terminology. The TF-IDF implementation creates semantic vectors for each document, enabling similarity-based search and document clustering through cosine similarity calculations.
The Document Summarization Module provides both extractive and abstractive summarization, with options to customize summary length and focus on specific sections like facts, legal issues, or the court's ruling. Summaries are cached to improve performance for frequently accessed documents.
Beyond basic search, the system provides analytical tools including term frequency statistics, document similarity matrices, and clustering analysis. It can identify the most similar document pairs in the entire corpus, group related cases automatically, and show which terms contribute most to document relevance. The interactive command-line interface makes these advanced capabilities accessible without requiring technical expertise.

Implementation and Architecture

The project follows a modular architecture with clear separation of concerns. The pre-processing pipeline handles everything from web scraping and PDF conversion to text cleaning and tokenization. Separate modules manage Boolean indexing, n-gram extraction, and TF-IDF vectorization, all optimized for performance with sparse matrix operations and batch processing for large datasets.
The Summarization Module is implemented as a standalone component that integrates with the document retrieval pipeline. It uses a hybrid approach:

->Extractive summarization via Text Rank and TF-IDF scoring for speed and accuracy
->Abstractive summarization using a fine-tuned legal-BERT model for fluency and coherence

Section-aware summarization that prioritizes legally relevant parts (e.g., ratio decidendi)
Performance has been carefully optimized—Boolean queries typically return results in under 100 milliseconds, while more computationally intensive semantic searches complete within 500 milliseconds. Summarization times average 2-3 seconds per document, with cached results available instantly. The system maintains persistent indexes and summaries to avoid recompilations, supports incremental updates as new documents are added, and includes comprehensive testing to ensure reliability.

Educational and Practical Value

From an educational perspective, this project serves as an excellent case study in applying theoretical IR concepts to real-world problems. It covers the full spectrum from data acquisition and pre-processing through to advanced ranking algorithms, summarization techniques, and user interface design. For legal professionals, it offers a practical tool that could significantly reduce the time spent on case law research while improving the quality of legal arguments through better precedent discovery and rapid case comprehension.
The Document Summarization Module adds significant practical value by addressing a common pain point in legal research: the time required to read lengthy judgements. By providing accurate, customizable summaries, it enables faster triage of relevant cases and better overview of legal principles.
The codebase is thoroughly documented, modular, and follows software engineering best practices, making it suitable for both production use and academic study. Whether you're interested in information retrieval systems, legal technology, or practical NLP applications, this project provides valuable insights and reusable components.

