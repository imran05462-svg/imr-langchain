
# What is LangChain?

LangChain is a framework for building applications with LLMs (Large Language Models) like GPT.
It helps you:

Connect LLMs with data (files, APIs, databases).

Manage chains of prompts → responses → actions.

Build agents that can use tools (search, calculators, etc.).

# Step 1: Install LangChain
pip install langchain openai
pip install faiss-cpu tiktoken

# Step 2: Setup OpenAI API Key
export OPENAI_API_KEY="your_api_key_here"
import os
os.environ["OPENAI_API_KEY"] = "your_api_key_here"

# Step 3: First “Hello World” with LangChain
from langchain_openai import ChatOpenAI

# Create LLM instance
llm = ChatOpenAI(model="gpt-3.5-turbo")

# Ask something
response = llm.invoke("Write a haiku about LangChain")
print(response.content)

# Step 4: Use a Prompt Template

<img width="395" height="182" alt="image" src="https://github.com/user-attachments/assets/b50636d2-dc2f-4abb-86b1-9b568a68555c" />
