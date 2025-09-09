# Retrieval Augmented Generation (RAG) - Complete Implementation Guide

A comprehensive repository demonstrating Retrieval-Augmented Generation (RAG) techniques, from basic data ingestion to advanced agentic RAG systems. This repo provides hands-on examples of building production-ready RAG systems with multiple data sources, embedding techniques, vector databases, and intelligent agents.

## Overview

Retrieval-Augmented Generation (RAG) is a powerful technique that combines the knowledge retrieval capabilities of vector databases with the generative power of Large Language Models (LLMs). This repository contains complete implementations covering every aspect of RAG systems.

## RAG Architecture

```
Data Sources → Data Ingestion → Text Splitting → Embeddings → Vector Store
                                                                    ↓
User Query → Query Embedding → Similarity Search → Context Retrieval → LLM Generation
```

## Quick Start

### 1. Environment Setup

```bash
# Clone the repository
git clone https://github.com/beniamine3155/Retrieval_Augmented_Generation_RAG.git
cd Retrieval_Augmented_Generation_RAG

# Install dependencies
pip install -r requirements.txt

# Or using uv (recommended)
uv sync
```

### 2. Environment Variables

Create a `.env` file with your API keys:

```env
OPENAI_API_KEY=your_openai_api_key_here
GROQ_API_KEY=your_groq_api_key_here  # Optional
```

### 3. Run Basic RAG Example

```bash
python main.py
```

## Learning Modules

### 1. Data Ingestion (`Data_Ingestion/`)

Learn how to process and load various data formats:

- **📄 Text Files** (`01_data_ingestion_textfiles.ipynb`)
  - Document structure understanding
  - Metadata handling
  - Custom document loaders
  - Text preprocessing techniques

- **📑 PDF Documents** (`02_pdf_files.ipynb`)
  - PyPDF and PyMuPDF integration
  - Page-based document splitting
  - Metadata extraction from PDFs
  - Handling complex PDF layouts

- **📝 Word Documents** (`03_word_documents.ipynb`)
  - DOCX file processing
  - Unstructured document loader
  - Content and formatting extraction
  - Cross-platform compatibility

- **📊 Structured Data** (`04_csv_excel.ipynb`)
  - CSV and Excel file processing
  - Pandas integration
  - Row-wise document creation
  - Data validation and cleaning

- **🔗 JSON Data** (`05_json_data.ipynb`)
  - JSON and JSONL processing
  - Nested data structure handling
  - Custom document formatters
  - Schema validation

- **🗃️ SQL Databases** (`06_sql_data.ipynb`)
  - SQLite integration
  - Dynamic query generation
  - Relational data to documents
  - Database connection management

### 2. Embeddings (`Embedding/`)

Master vector representations and similarity metrics:

- **Vector Concepts** (`embedding_technique.ipynb`)
  - 2D visualization of embeddings
  - Cosine similarity calculations
  - Distance metrics comparison
  - Semantic relationship mapping

### 3. Vector Stores (`VectorStore_VectorDB/`)

Implement efficient vector storage and retrieval:

- **ChromaDB Implementation** (`vectorstore.ipynb`)
  - Vector database setup
  - Document chunking strategies
  - Embedding generation with OpenAI
  - Similarity search optimization
  - Persistent storage configuration

### 4. Agentic RAG (`Agentic_Rag/`)

Build intelligent RAG systems with autonomous agents:

- **LangGraph Agents** (`agentic_rag.ipynb`)
  - Multi-tool agent architecture
  - Document relevance checking
  - Dynamic retrieval strategies
  - Conversational memory
  - Tool-based decision making

## Technologies Used

### Core Libraries
- **LangChain**: Document processing and RAG orchestration
- **LangGraph**: Agent-based workflows and decision trees
- **ChromaDB**: Vector database for embeddings storage
- **FAISS**: Fast similarity search and clustering
- **Sentence Transformers**: Advanced embedding models

### Data Processing
- **PyPDF/PyMuPDF**: PDF document processing
- **python-docx**: Word document handling
- **pandas**: Structured data manipulation
- **BeautifulSoup4**: Web content extraction
- **unstructured**: Multi-format document processing

### AI/ML Integrations
- **OpenAI**: GPT models and embeddings
- **Groq**: High-speed inference
- **Hugging Face**: Open-source models and embeddings

## Use Cases

### 1. Document Q&A Systems
- Legal document analysis
- Technical documentation search
- Research paper exploration
- Policy and procedure queries

### 2. Knowledge Management
- Corporate knowledge bases
- Customer support automation
- Training material navigation
- Institutional memory preservation

### 3. Content Analysis
- Literature review automation
- Competitive intelligence
- Market research synthesis
- Academic research assistance

### 4. Intelligent Chatbots
- Domain-specific conversational AI
- Technical support agents
- Educational tutoring systems
- Professional consultation tools

## 🔧 Advanced Features

### Multi-Source RAG
- Combine multiple data types in a single system
- Cross-reference information from different sources
- Weighted retrieval from various databases
- Source attribution and citation

### Agentic Workflows
- Self-correcting retrieval systems
- Multi-step reasoning processes
- Tool selection and usage
- Context-aware response generation

### Performance Optimization
- Chunk size optimization
- Embedding model selection
- Vector database indexing
- Caching strategies

## 📖 Learning Path

1. **Start with Data Ingestion**: Learn how to process different data formats
2. **Understand Embeddings**: Master vector representations and similarity
3. **Implement Vector Stores**: Set up efficient storage and retrieval
4. **Build Basic RAG**: Create simple question-answering systems
5. **Explore Agentic RAG**: Develop intelligent, autonomous systems
