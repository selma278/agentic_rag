   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/selma278/agentic_rag/blob/main/agentic_rag.ipynb)
# Agentic RAG with LlamaIndex + Groq

An agent that decides when to query a document (RAG) and when to call a calculator tool.

## Stack
- LlamaIndex (FunctionAgent)
- Local embeddings: all-MiniLM-L6-v2
- LLM: openai/gpt-oss-120b on Groq

## How to run
1. Get a Groq API key from console.groq.com
2. Open the notebook in Colab
3. Add the key as a secret named GROQ_API_KEY
4. Run all cells

## Example
Q: "What is the neural radiance number plus 32432584?"
The agent retrieves 1200 from the document, then calls the `add` tool → 32433784
