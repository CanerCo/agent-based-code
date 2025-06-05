# 📘 ntb1_rag_agents_recap.ipynb

## Description

This notebook demonstrates how to build and interact with intelligent retrieval-augmented generation (RAG) agents using the `smolagents` library. It focuses on automating the search for PhD research ideas in the field of Computational Linguistics using both live web searches and a custom semantic search over a knowledge base.

## Features

- ✅ Integration with Hugging Face for model inference
- 🔍 Web search capability via DuckDuckGo for real-time results
- 📚 Custom semantic search over a curated list of PhD research ideas using `BM25Retriever`
- 🤖 Agent architecture combining external tools and model responses
- 🧠 Emphasis on combining external knowledge sources for contextual and relevant answers

## Key Components

- **SmolAgents**: Lightweight agents that use tools like search engines and custom retrievers  
- **DuckDuckGoSearchTool**: Enables real-time retrieval from the web  
- **PhdIdeasRetrieverTool**: A tool for semantic search through a static list of domain-specific ideas  
- **LangChain & BM25Retriever**: Powers vectorized and keyword-based document retrieval  
- **Example Queries**: Includes sample prompts for retrieving PhD research topics  


# ntb2-tool-calling-agents

This Python script demonstrates how to create, use, and share custom AI-powered tools using the [`smolagents`](https://pypi.org/project/smolagents/) framework in conjunction with Hugging Face services. It includes several examples of defining, deploying, and importing tools and agents for tasks like restaurant recommendations, PhD topic generation, and image generation.

---

## 🚀 Features

- **🔧 Tool Definition using Decorators**  
  Use the `@tool` decorator to define simple tools (e.g., highest-rated restaurant finder).

- **📦 Class-Based Tool Creation**  
  Create structured tools like `PhdIdeasTopicTool` for generating research topics.

- **🤗 Hugging Face Integration**  
  - Authenticate and access the Hugging Face Inference API.
  - Push custom tools to the Hub.
  - Load tools from the community.

- **🌐 Advanced Tool Loading**
  - Load tools from Hugging Face Spaces (`Tool.from_space()`).
  - Use LangChain tools with `Tool.from_langchain()` (requires SERPAPI key).
  - Load tools from MCP servers for advanced applications.

---

## 🛠️ Requirements

- Python 3.8+
- `smolagents`
- `huggingface_hub`
- `gradio_client`
- `langchain-community`
- `google-search-results`
- `mcp` (optional, for MCP integration)

Install all dependencies with:

```bash
pip install smolagents gradio_client langchain-community google-search-results "smolagents[mcp]"

## Use Case

Ideal for students, researchers, or developers interested in:
- Building smart assistants for academic or technical research
- Experimenting with hybrid LLM agents that combine live search with static knowledge
- Creating domain-specific agents for information retrieval
