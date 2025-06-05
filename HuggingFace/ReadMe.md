Description
This notebook demonstrates how to build and interact with intelligent retrieval-augmented generation (RAG) agents using the smolagents library. It focuses on automating the search for PhD research ideas in the field of Computational Linguistics using both live web searches and a custom semantic search over a knowledge base.

Features
✅ Integration with Hugging Face for model inference

🔍 Web search capability via DuckDuckGo for real-time results

📚 Custom semantic search over a curated list of PhD research ideas using BM25Retriever

🤖 Agent architecture combining external tools and model responses

🧠 Emphasis on combining external knowledge sources for contextual and relevant answers

Key Components
SmolAgents: Lightweight agents that use tools like search engines and custom retrievers

DuckDuckGoSearchTool: Enables real-time retrieval from the web

PhdIdeasRetrieverTool: A tool for semantic search through a static list of domain-specific ideas

LangChain & BM25Retriever: Powers vectorized and keyword-based document retrieval

Example Queries: Includes sample prompts for retrieving PhD research topics

Use Case
Ideal for students, researchers, or developers interested in:

Building smart assistants for academic or technical research

Experimenting with hybrid LLM agents that combine live search with static knowledge

Creating domain-specific agents for information retrieval
