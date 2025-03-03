# 💬 RAG-based InterviewBot with Neo4j, LangChain & LlamaIndex

This project is a **Retrieval-Augmented Generation (RAG)** based chatbot that leverages **Neo4j**, **LangChain**, and **LlamaIndex** to perform advanced knowledge retrieval over a graph database. By combining graph data with language models, it allows for intelligent, context-aware conversations powered by structured knowledge.

---

## 🚀 Features

- ✅ **RAG-based Chatbot**: Answers user queries by retrieving relevant graph context and enhancing responses using an LLM.
- ✅ Loads and parses data from a **Neo4j graph database**.
- ✅ Converts nodes and relationships into documents for **LlamaIndex**.
- ✅ Builds a `VectorStoreIndex` for semantic search over the graph.
- ✅ Retrieves accurate, contextually relevant information with **custom retrievers**.
- ✅ Supports natural language queries using **LangChain** and **OpenAI GPT**.
- ✅ Executes **Cypher queries** and combines results with LLM output.

---

## 🏗️ Tech Stack

| Technology         | Purpose                                |
|--------------------|----------------------------------------|
| **Python**        | Backend logic                         |
| **Neo4j**         | Graph database                        |
| **LlamaIndex**    | Document indexing & retrieval         |
| **LangChain**     | LLM orchestration & pipelines         |
| **OpenAI GPT**    | Text generation & augmentation        |
| **Neo4jGraph**    | Cypher query interface                |
| **RAG**           | Combines retrieved context with LLMs  |

---

## 🗂️ Project Structure
. ├── graph_loader.py # Loads and processes graph data from Neo4j ├── retriever.py # Custom retriever for RAG pipeline ├── query_engine.py # LLM-based query handling ├── app.py # Example chatbot interface ├── requirements.txt # Dependencies └── README.md # Documentation


---

## ⚙️ Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/rag-graph-chatbot.git
   cd rag-graph-chatbot
2. **Set up the environment:**
   ```bash
    python3 -m venv venv
    source venv/bin/activate
    pip install -r requirements.txt

3. **Configure environment variables:**
   ```bash
    OPENAI_API_KEY=your_openai_key
    NEO4J_URI=bolt://localhost:7687
    NEO4J_USERNAME=neo4j
    NEO4J_PASSWORD=your_password

## 🏃 🧠 How the RAG Chatbot Works
🔹 Step 1: User asks a natural language question. <br>
🔹 Step 2: Relevant nodes and relationships are retrieved from Neo4j.<br>
🔹 Step 3: Data is transformed into documents for LlamaIndex indexing.<br>
🔹 Step 4: Semantic search finds the most relevant pieces of information.<br>
🔹 Step 5: The selected context is passed to OpenAI GPT.<br>
🔹 Step 6: GPT generates an enriched, context-aware response.<br>
🔹 Step 7: The answer is returned to the user.<br>

## 💡 Acknowledgements
- LangChain
- LlamaIndex
- Neo4j
- OpenAI GPT
