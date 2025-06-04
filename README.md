# DocuMind

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
![Made with LangChain](https://img.shields.io/badge/Made%20with-LangChain-blue)
![Platform](https://img.shields.io/badge/Platform-PDF%2C%20PPT%2C%20DOCX-lightgrey)
![Status](https://img.shields.io/badge/Status-Prototype-yellow)
![LLMs](https://img.shields.io/badge/LLM-Gemini%20%7C%20GPT%20%7C%20Groq-orange)

A Retrieval-Augmented Generation (RAG) pipeline that ingests PowerPoint, PDF, and DOCX files, extracts text, tables, and images, stores them in a vector database, and leverages an LLM (e.g., Google Gemini or GPT) to answer queries by combining document content with the model’s world knowledge.

---

## 🚀 Project Overview

**DocuMind** is a proof-of-concept demonstrating how to turn arbitrary documents (PDFs, PPTs, DOCXs) into a question-answering system that:

1. **Partitions & preprocesses** each document’s contents (text, tables, images).
2. **Embeds** extracted chunks into a vector store (Chroma).
3. **Retrieves** relevant passages at query-time.
4. **Combines** retrieved context with a large language model (LLM) (e.g., Google Gemini, Groq, or OpenAI ChatGPT) to generate a polished answer that weaves in both document data and the model’s inherent knowledge.

> **Use Cases:**  
> - Instant Q&A over slide decks, research papers, or lengthy reports  
> - Summarization of tables/figures + contextual explanation  
> - Building chatbots that “know” your proprietary docs + general knowledge  

---

### 🧠 Architecture Overview

![DocuMind Flow Diagram](https://github.com/user-attachments/assets/2fb817bb-4479-4b03-9f68-bfdb8116a21e)


---

## 🙋‍♂️ Acknowledgments

1. **Unstructured** by Elaine and team for seamless PDF/PPTX partitioning  
2. **LangChain** for providing a modular RAG framework  
3. **Chroma** for a lightweight, local vector store  
4. **Google Gemini**, **OpenAI**, and **Groq** teams for state-of-the-art LLM APIs  
