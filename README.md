# Building Your Own Database Agent

Learn how to build your own AI agent to interact with SQL data and tabular data using the Langchain agent framework and Azure Open AI.

## Overview

This guide will walk you through the steps to deploy a Language Model (LLM) using an AI agent, implement Retrieval-Augmented Generation (RAG) with tabular data, develop your database agent, build a function-calling system, and integrate the Azure Open AI Assistant API.

## Steps

1. **Deploy an LLM Using an AI Agent**
2. **Implement RAG with Tabular Data**
3. **Develop Your Database Agent**
4. **Build a Function Calling System**
5. **Integrate Azure Open AI Assistant API**

## 1. Building an AI Agent

Start by experimenting with Azure Open AI to create a simple agent for language translation.

## 2. Interact with CSV Data

To build a database agent that connects to a database, we use a baseline GPT model with robust prompt capabilities. For handling SQL tasks, you can customize a model by fine-tuning it. However, we will use a RAG pattern with a database or dataset as the data source. Here, we focus on CSV files, utilizing Langchain Agents to connect to the CSV file as our starting point.

![Screenshot 2024-06-17 164520](https://github.com/Lekhansh-cmd/Building-a-Database-Agent-Using-Azure-Open-AI/assets/78807364/30c3c44b-4868-4997-8698-827ac11caf0c)


## 3. Connect to a SQL Database

After successfully connecting a CSV file to a Langchain agent, proceed to connect directly to a database. We will use a SQLite Database, a local instance of a relational database, accessed via API.

![Screenshot 2024-06-17 165915](https://github.com/Lekhansh-cmd/Building-a-Database-Agent-Using-Azure-Open-AI/assets/78807364/1e282b62-6213-4901-89c1-4dd1d0622c2f)


## 4. Azure OpenAI Function Calling

The Function Calling feature is beneficial for several reasons:

- Provides specific instructions for finding information.
- Prioritizes queries for precise results and desired format.
- Adds control and encapsulates queries for better structure and predictability.

## 5. Leverage Assistants API for SQL Databases

In the final step, combine the previous configurations using the Azure Open AI Assistants API, which offers features such as:

- Maintains conversation context dynamically.
- Stateful, keeping track of interactions, useful for scenarios like e-commerce.
- Enables function calling.
- Supports Code Interpreter, allowing it to handle and modify Python code iteratively, adjusting code until successful, and enabling autonomous code modification.

**Run the Script Locally**
To run the script locally, follow these steps:

1. **Clone the Repository**: Start by cloning the repository to your local machine.
   git clone https://github.com/Lekhansh-cmd/Building-a-Database-Agent-Using-Azure-Open-AI.git
   cd your-repository

2. **Set Up a Virtual Environment**: It's recommended to use a virtual environment to manage dependencies.
   python -m venv venv
   source venv/bin/activate   # On Windows use `venv\Scripts\activate`

3. **Generate .env File:** Create a .env file in the root directory to store your Azure Open AI key.
   touch .env

  Add the following line to the .env file:
  AZURE_OPENAI_KEY=your_azure_openai_key

4. **Install Required Libraries:** Use requirements.txt to install the necessary libraries.
   pip install -r requirements.txt

5. **Run Your Script:** Execute your Python script.
   python your_script.py



