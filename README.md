# Retrieval Augmented Generation (RAG) - Complete Implementation Guide

A comprehensive repository demonstrating Retrieval-Augmented Generation (RAG) techniques, from basic data ingestion to advanced agentic RAG systems. This project provides hands-on examples of building production-ready RAG systems with multiple data sources, embedding techniques, vector databases, and intelligent agents.

## 🎯 Overview

Retrieval-Augmented Generation (RAG) is a powerful technique that combines the knowledge retrieval capabilities of vector databases with the generative power of Large Language Models (LLMs). This repository contains complete implementations covering every aspect of RAG systems.

### Key Benefits of RAG:
- **Reduces Hallucinations**: Provides factual, source-backed responses
- **Up-to-date Information**: Access to current data without retraining models
- **Source Attribution**: Ability to cite and reference original documents
- **Domain-Specific Knowledge**: Leverage proprietary or specialized content
- **Cost-Effective**: No need for expensive model fine-tuning

## 🏗️ RAG Architecture

```
Data Sources → Data Ingestion → Text Splitting → Embeddings → Vector Store
                                                                    ↓
User Query → Query Embedding → Similarity Search → Context Retrieval → LLM Generation
```

## 📁 Project Structure

```
├── main.py                           # Main application entry point
├── requirements.txt                  # Python dependencies
├── pyproject.toml                   # Project configuration
├── 
├── Data_Ingestion/                  # 📥 Data Loading & Processing
│   ├── 01_data_ingestion_textfiles.ipynb    # Text file processing
│   ├── 02_pdf_files.ipynb                   # PDF document handling
│   ├── 03_word_documents.ipynb              # Word document processing
│   ├── 04_csv_excel.ipynb                   # Structured data (CSV/Excel)
│   ├── 05_json_data.ipynb                   # JSON data processing
│   ├── 06_sql_data.ipynb                    # Database integration
│   └── data/                                # Sample datasets
│       ├── text_files/                      # Plain text samples
│       ├── pdf/                             # PDF documents
│       ├── word_files/                      # Word documents
│       ├── structured_files/                # CSV/Excel files
│       ├── json_files/                      # JSON datasets
│       └── databases/                       # SQLite databases
│
├── Embedding/                       # 🔢 Vector Representations
│   └── embedding_technique.ipynb            # Embedding methods & similarity
│
├── VectorStore_VectorDB/           # 🗄️ Vector Database Management
│   ├── vectorstore.ipynb                    # ChromaDB implementation
│   ├── chroma_db/                           # Persistent vector storage
│   └── data/                                # Sample documents
│
└── Agentic_Rag/                    # 🤖 Intelligent RAG Agents
    └── agentic_rag.ipynb                    # LangGraph-based RAG agents
```

## 🚀 Quick Start

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

## 📚 Learning Modules

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

## 🛠️ Technologies Used

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

## 🎯 Use Cases

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

## 🤝 Contributing

We welcome contributions! Please feel free to:
- Add new data source integrations
- Improve embedding techniques
- Enhance vector store implementations
- Create new agent architectures
- Fix bugs and improve documentation

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- OpenAI for providing powerful language models and embeddings
- LangChain team for the comprehensive RAG framework
- ChromaDB for efficient vector storage solutions
- The open-source community for various data processing libraries

## 📞 Support

For questions, issues, or discussions:
- Open an issue in this repository
- Check the documentation in individual notebooks
- Review the code examples for implementation details

---

**Start your RAG journey today!** 🚀 Begin with the data ingestion notebooks and gradually work your way up to building sophisticated agentic RAG systems.