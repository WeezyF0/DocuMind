# DocuMind

A Retrieval-Augmented Generation (RAG) pipeline that ingests PowerPoint, PDF, and DOCX files, extracts text, tables, and images, stores them in a vector database, and leverages an LLM (e.g., Google Gemini or GPT) to answer queries by combining document content with the model’s world knowledge.

---

## 🚀 Project Overview

**Multi-modal RAG with LangChain** is a proof-of-concept demonstrating how to turn arbitrary documents (PDFs, PPTs, DOCXs) into a question-answering system that:

1. **Partitions & preprocesses** each document’s contents (text, tables, images).
2. **Embeds** extracted chunks into a vector store (Chroma).
3. **Retrieves** relevant passages at query-time.
4. **Combines** retrieved context with a large language model (LLM) (e.g., Google Gemini or OpenAI ChatGPT) to generate a polished answer that weaves in both document data and the model’s inherent knowledge.

> **Use Cases:**  
> - Instant Q&A over slide decks, research papers, or lengthy reports  
> - Summarization of tables/figures + contextual explanation  
> - Building chatbots that “know” your proprietary docs + general knowledge


## 🙋‍♂️ Acknowledgments
Unstructured by Elaine and team for seamless PDF/PPTX partitioning.
LangChain for providing a modular RAG framework.
Chroma for a lightweight, local vector store.
Google Gemini, OpenAI, and Groq teams for state-of-the-art LLM APIs.
