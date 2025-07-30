# UdaPlay - AI Game Research Agent Project

This repo is my solution to project 3 of the Agentic AI Nanodegree Program from Udacity.   
Completion date: July 30, 2025  

## Project Overview
UdaPlay is an AI-powered research agent for the video game industry. 

## Project Structure

### Part 1: Offline RAG (Retrieval-Augmented Generation)
Uses a Vector Database (ChromaDB) to store and retrieve video game information efficiently.

### Part 2: AI Agent Development
Builds an intelligent agent that combines local knowledge with web search capabilities.

The agent has the following capabilities:
1. Answer questions using internal knowledge (RAG)
2. Search the web when needed
3. Maintain conversation state
4. Return structured outputs


### Directory Structure
```
root/
├── games/           # JSON files with game data
├── lib/             # Custom library implementations
│   ├── llm.py       # LLM abstractions
│   ├── messages.py  # Message handling
│   ├── ...
│   └── tooling.py   # Tool implementations
├── Udaplay_01_starter_project.ipynb  # Part 1 implementation
└── Udaplay_02_starter_project.ipynb  # Part 2 implementation
```

## Requirements

### Environment Setup
Create an `.env` file with the following entries:
```
OPENAI_API_KEY="YOUR_KEY"
OPENAI_BASE_URL="https://api.openai.com/v1"
CHROMA_OPENAI_API_KEY="YOUR_KEY"
TAVILY_API_KEY="YOUR_KEY"
VOCAREUM_OPENAI_API_KEY="YOUR_KEY"   # Can be the same as OPENAI_API_KEY, as long as VOCAREUM_BASE_URL is then also the same as OPENAI_BASE_URL
VOCAREUM_BASE_URL="https://openai.vocareum.com/v1"
```

### Project Dependencies
- Python 3.11+
- ChromaDB
- OpenAI
- Tavily
- dotenv


## License
MIT License see [here](./LICENSE.md). 

Chosen based on [this mentor answer](https://knowledge.udacity.com/questions/155958).

## Udacity Honor Code
See [Udacity Honor Code](https://support.udacity.com/hc/en-us/articles/210667103-Udacity-Honor-Code).

I confirm that this submission is my own work. I have not used code from any other Udacity student's or graduate's submission of the same project. I have correctly attributed all code I have obtained from other sources, such as websites, books, forums, blogs, GitHub repos, etc. I understand that Udacity will check my submission for plagiarism, and that failure to adhere to the Udacity Honor Code may result in the cancellation of my enrollment.