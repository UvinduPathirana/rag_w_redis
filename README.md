# Build a RAG Application with Langchain and Redis

This repository serves as a beginner-friendly guide for building a RAG application using Lanchain and Redis.
The vector database used here is Redis since it is a very lightweight, fast and popular vector database nowadays.

We use Jupyter Notebook as the code notebook since it is a free open source popular notebook. Also better to have docker 
installed on the developer's computer.

## Requirements

To get started with this project, you will need:

- **Docker**: Recommended for easy deployment of RedisStack.
- **Jupyter Notebook**: For running the provided code snippets and tutorials.
- **Langchain Libraries**: For building the RAG model and managing various NLP components.

## Components

1. **RedisStack**: RedisStack provides vector similarity search capabilities that are crucial for managing embeddings and vector-based queries.
2. **Jupyter Notebook**: Used for experimentation, code execution, and interaction with the Redis database.
3. **Langchain**: A powerful library for creating language models and integrating with external knowledge sources like vector databases.

## Folder Structure

- **Vector_db_tut/**: This folder contains a comprehensive tutorial on how to use Redis as a vector database, including:
  - **Working with Redis-Stack Functions**: A deep dive into the RedisStack commands and operations relevant for vector storage and similarity search.
  - **Encoding and Storing JSON Data to Redis VDB**: Demonstrates how to encode and vectorize JSON datasets, then store them as vectors in Redis.
  - **Querying Redis for Vector Similarity**: Guides on vectorizing user queries and performing k-nearest neighbor (KNN) searches within Redis.
  - **Building a Query Table**: Details on building a query system to retrieve the most relevant data from the vectorized dataset using similarity search.

## What is a RAG Model?

A **Retrieval-Augmented Generation (RAG)** model combines traditional language models (LLMs) with an external knowledge source (like Redis) to enhance the model’s ability to provide factually accurate information. Here's how it works:

1. **Retrieval**: The system retrieves relevant information from the vector database based on a user query. In this case, Redis is used to store and retrieve embeddings (vectorized data points).
2. **Augmentation**: The retrieved data is used to "augment" the language model’s response, ensuring it’s grounded in real-world data.
3. **Generation**: The final step involves the language model generating a response based on the user query and the retrieved context.

By storing embeddings in Redis, this model can perform **vector similarity searches** to retrieve relevant context or information before generating an answer.

