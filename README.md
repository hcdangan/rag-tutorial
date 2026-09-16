# Retrieval-Augmented Generation (RAG) Tutorial

This tutorial will guide you through building **Retrieval-Augmented Generation** (RAG) systems — one of the most practical and powerful architectural patterns for working with large language models today.

## Prerequisites

- Python 3.8+
- Basic knowledge of Python programming
- Familiarity with LLMs (optional, but helpful)

## Getting Started

1. Clone or download this repository
2. **Install dependencies using pyproject.toml** (recommended):
   ```bash
   pip install -e .
   # or for specific groups:
   pip install -e ".[llm]"      # with LLM support (OpenAI/Ollama)
   pip install -e ".[pdf]"      # with PDF processing
   pip install -e ".[evaluation]"  # with evaluation tools
   pip install -e ".[dev]"      # with development tools
   ```

3. Open `rag_tutorial.ipynb` in Jupyter Notebook or VS Code
4. Follow the lessons sequentially, running each cell

## Development Setup

```bash
# Install with development dependencies
pip install -e ".[dev]"

# Run tests
pytest

# Format code
black .
```

## Tutorial Structure

### Lesson 1: Introduction to RAG
- Understanding RAG and its importance
- Traditional LLMs vs RAG comparison
- Key benefits and use cases
- Real-world examples

### Lesson 2: Core Components of RAG
- Document stores and vector databases
- Embedding models and their role
- Retrievers and similarity search
- LLM integration and context management

### Lesson 3: Document Processing and Chunking
- Text preprocessing strategies
- Chunking methods (fixed-size, overlapping, content-aware)
- Handling different document formats (PDF, Word, HTML)

### Lesson 4: Vectorization and Embeddings
- Understanding embeddings
- Cosine similarity and vector distance
- Popular embedding models
- Best practices and multilingual support

### Lesson 5: Simple RAG with LangChain
- Setting up the environment
- Basic RAG pipeline implementation
- Creating a retriever
- Querying the system

### Lesson 6: Deep-RAG with LangChain
- Hybrid chains (MapReduce, Refine, Map-Rerank)
- Recursive retrieval
- Re-ranking with cross-encoder
- Multi-query generation

### Lesson 7: Advanced RAG Techniques
- Multi-vector retrieval
- Document transformation strategies
- Query decomposition
- Knowledge graph integration

### Lesson 8: Evaluation of RAG Systems
- Metrics that matter (F1, Context Precision)
- Evaluation frameworks (RAGAS, TruLens)
- Human evaluation

### Lesson 9: Production Considerations
- API design
- Vector database selection
- Scalability and caching
- Security and monitoring

### Lesson 10: Project - Building a PDF RAG System
- End-to-end implementation
- Loading PDF documents
- Building query interface
- Troubleshooting

## File Structure

```
rag-tutorial/
├── rag_tutorial.ipynb       # Main tutorial notebook (10 lessons)
├── README.md                 # This file
├── AI_CONTEXT.md             # Original context
├── lesson1_content.md        # Lesson 1 original content (reference)
```

## Resources

### Core Resources
- [LangChain Documentation](https://python.langchain.com/docs/)
- [Hugging Face Tutorials](https://huggingface.co/docs)
- [FAISS Documentation](https://faiss.ai/documentation/faiss-tutorial.html)

### Advanced Resources
- [RAGAS Framework](https://docs.ragas.io/)
- [DeepRAG GitHub](https://github.com/DataWonderAI/DeepRAG)
- [TruLens](https://www.trulens.org/)

## Contributing

Feel free to improve the tutorial, add new examples, or fix any issues you encounter!

## License

This tutorial is provided as-is for educational purposes.

---

*Last Updated: 2024*
