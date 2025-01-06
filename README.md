# Gen-AI-Hackathon-Text-to-Data-
A robust and intelligent query resolution system leveraging Vector Databases, Large Language Models (LLMs), and Relational Database Services (RDS).


# Optimized Query Resolution System

## Overview
The Optimized Query Resolution System is a scalable and intelligent framework for efficiently resolving user queries. It combines the power of Vector Databases, large language models (LLMs), and Relational Database Services (RDS) to deliver accurate and relevant results with insightful summaries.

## Key Features
- **Vector Search**: Stores and retrieves commonly used queries from a Vector Database for high-speed semantic matching.
- **Query Re-Ranking**: Utilizes LLMs to rank queries based on similarity and relevance.
- **Automated Query Refinement**: Finalizes user queries for execution using LLMs to ensure correctness and clarity.
- **RDS Integration**: Executes refined queries on an RDS for data retrieval.
- **Data Summarization**: Summarizes results using LLMs for better understanding.
- **Scalable Architecture**: Designed to handle large-scale queries efficiently.
- **Security**: Implements input sanitization and access control to ensure data safety.

---

## Workflow
1. **Store General Queries**  
   - Save 20-30 commonly used queries as vector embeddings in a Vector Database.

2. **Retrieve Relevant Queries**  
   - Fetch the top-N relevant queries from the Vector Database based on the user's input.

3. **Re-Rank Queries**  
   - Use an LLM to re-rank the queries based on semantic similarity and contextual relevance.

4. **Select Top Queries**  
   - Extract the top-K most relevant queries from the ranked list.

5. **Finalize Query**  
   - Refine and finalize the query with the help of an LLM.

6. **Execute Query**  
   - Execute the refined query on the RDS server to fetch the desired data.

7. **Deliver Results**  
   - Summarize and present the retrieved data to the user in an easy-to-understand format.

---

## Prerequisites
- **Python 3.8+**
- Libraries:
  - sentence-transformers (for embeddings)
  - pinecone, weaviate, or `milvus` (for Vector Database operations)
  - openai or similar (for LLM integration)
- A configured **RDS Server** (MySQL, PostgreSQL, etc.)
- API keys for your Vector Database and LLM provider (e.g., OpenAI).
