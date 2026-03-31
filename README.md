# Developments in LLM/RAG — Workshop

A hands-on workshop covering LLM foundations, Retrieval-Augmented Generation (RAG), agents and evals. We use work with a project I created : natural language search for the Richard and Carole Cocks Art Museum collection at Miami University.

## Contents

- **presentation.qmd** — Quarto Reveal.js slide deck
- **presentation_code_along.ipynb** — Runnable Jupyter notebook that mirrors the slides
- **data/extracted_data.json** — 2,333 artwork records from the museum collection
- **vstore/** — Pre-built FAISS vector index (OpenAI `text-embedding-3-small`, 1536-dim)
- **assets/** — Interactive visualizations (3D vector store plot)

## Topics Covered

1. **LLM Foundations** — Tokenization, embeddings, transformers, temperature, API usage
2. **RAG** — Vector stores, FAISS, LangChain/LangGraph pipelines, SQL + vector hybrid retrieval with a routing agent
3. **LLM Agents** — SQL tooling, MCP (Model Context Protocol)
4. **LLM Evals** — Accuracy/latency/cost, LLM-as-judge, golden sets

## Setup

```bash
pip install tiktoken sentence-transformers numpy pandas \
  langchain langchain-community langchain-openai langchain-core \
  langgraph openai faiss-cpu
```

Set your OpenAI API key:

```bash
export OPENAI_API_KEY="sk-..."
```

## Running

- **Slides:** `quarto render presentation.qmd` then open `presentation.html`
- **Notebook:** Open `presentation_code_along.ipynb` in Jupyter or VS Code

## Author

Ryan Singh
