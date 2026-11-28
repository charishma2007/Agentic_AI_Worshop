# LangGraph – AI Chatbots and Multi-Agent Systems

## Project Overview

This project demonstrates the development of intelligent AI chatbots and multi-agent systems using LangGraph, LangChain, and Groq LLM. It explores tool calling, structured output, intent classification, state management, conditional routing, and agent-based workflows.

A Flower Shop business is used as a practical example to demonstrate automated customer support and order management.

## Objectives

- Build intelligent AI chatbots using LangGraph.
- Integrate external tools with Large Language Models.
- Classify customer queries using structured output.
- Implement state-based workflows and conditional routing.
- Develop specialized agents for customer support and order management.
- Visualize graph workflows and monitor execution using streaming.

## Notebooks Included

### 1. LangGraph_AI_Chatbot.ipynb

Implements a tool-enabled AI chatbot using LangGraph.

**Key Features:**

- Groq LLM integration
- Wikipedia tool integration
- Arxiv tool initialization
- Dynamic tool calling
- Message state management
- ToolNode and conditional edges
- Graph visualization
- Real-time response streaming

### 2. LangGraph_Intent_Classification.ipynb

Demonstrates structured output and customer intent classification for a Flower Shop business.

**Key Features:**

- Structured output using Pydantic
- Customer intent classification
- TypedDict-based state management
- StateGraph implementation
- Basic FAQ workflow demonstration
- Graph visualization and execution streaming

Customer queries are classified into three categories:

| Intent | Description |
|---|---|
| Order | Purchase flowers or book bouquets |
| FAQ | Ask about prices, availability, timings, or policies |
| Other | General or unrelated queries |

### 3. LangGraph_Multi_Agent_System.ipynb

Implements a multi-agent customer support and order management system for a Flower Shop.

**Key Features:**

- FAQ Agent for customer queries
- Order Agent for flower and bouquet bookings
- Intent-based conditional routing
- Custom business tools
- Price retrieval and shop timings
- Customer order collection and confirmation
- Graph visualization
- Step-by-step execution streaming

## Custom Business Tools

| Tool | Functionality |
|---|---|
| search_faq | Answers frequently asked customer questions |
| get_price | Retrieves flower and bouquet prices |
| is_open | Provides shop opening timings |
| log_order | Records customer order details |

## System Workflow

1. The customer enters a message.
2. The LLM identifies the customer's intent.
3. LangGraph routes the message to the appropriate node.
4. The FAQ Agent or Order Agent uses the required tools.
5. The system generates a relevant response.
6. The execution workflow can be monitored using graph streaming.

## Technologies Used

- Python
- LangGraph
- LangChain
- Groq API
- OpenAI GPT-OSS-120B
- Pydantic
- Wikipedia API
- Arxiv API
- Google Colab
- Mermaid Graph Visualization

## Sample Customer Queries

- Do you deliver flowers to my area?
- What is the price of a rose?
- Do you provide customized bouquets?
- What are your shop opening timings?
- I'm Ravi, book 2 bouquets for 24 Dec 2026.
- Good morning!

## How to Run

1. Open the required notebook in Google Colab.
2. Install the required dependencies.
3. Generate a Groq API key.
4. Add the API key to Google Colab Secrets with the name `GROK_API_KEY`.
5. Enable notebook access to the secret.
6. Run all cells sequentially.
7. Enter sample queries and observe the generated responses and graph execution.

## Current Limitations

- The intent classification notebook demonstrates a basic FAQ workflow with a placeholder response.
- The Arxiv tool is initialized but not connected to the chatbot workflow.
- Business prices, timings, and policies are sample data.
- Customer orders are stored temporarily in a Python list.
- Multi-turn conversation persistence is not implemented in the Flower Shop multi-agent workflow.

## Learning Outcomes

- Understanding LangGraph architecture and state management.
- Integrating LLMs with external and custom tools.
- Implementing structured output and intent classification.
- Developing conditional agent workflows.
- Building specialized AI agents for business applications.
- Visualizing and monitoring graph execution.

## Conclusion

This project demonstrates how LangGraph and LangChain can be used to develop intelligent, modular, and tool-enabled AI applications. The Flower Shop multi-agent system illustrates how AI agents can automate customer interactions and business operations through structured workflows.
