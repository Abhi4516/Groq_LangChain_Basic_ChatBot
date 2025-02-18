## Building a Basic Chatbot

This project demonstrates:

* Setting up a basic chatbot using a Groq-backed LLM.
* Using LangChain’s message types (`HumanMessage`, `AIMessage`, etc.) to interact with the model.
* Implementing a conversation history with session management.
* Utilizing prompt templates to customize LLM interactions.
* Incorporating a message trimmer to manage context window sizes.

### Features

* **Chat Model Initialization:** Instantiate and interact with a Groq model.
* **Message History:** Save and retrieve conversation messages using a custom history store.
* **Prompt Templates:** Create custom prompt templates that adjust language or system behavior.
* **Conversation Management:** Limit messages sent to the LLM by trimming the conversation history.

---

## Vector Stores and Retrievers

This project illustrates how to:

* Represent documents with metadata using LangChain’s `Document` class.
* Generate vector embeddings with HuggingFace models.
* Index documents in a vector store using Chroma.
* Perform similarity search (both synchronously and asynchronously).
* Build a custom retriever using LangChain’s Runnable interface.
* Assemble a Retrieval-Augmented Generation (RAG) chain that answers questions using retrieved context.

### Features

* **Document Creation:** Define sample documents with content and metadata.
* **Vector Store Setup:** Use Chroma to create a vector index from documents.
* **Similarity Search:** Query the vector store for related documents using similarity metrics.
* **Retriever Wrapping:** Create Runnable retrievers for seamless integration in LCEL chains.
* **RAG Chain:** Build a chain that fetches relevant context and uses an LLM (via Groq) to answer questions.
