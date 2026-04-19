# Personalized News Agent

## Overview
This project builds an end-to-end personalized news retrieval and summarization system using LLM-based agents. It combines user interest data from a SQL database with web search, credibility filtering, and summarization to deliver relevant and trustworthy news updates.

## Features
- Fetches user interests from a SQL database
- Expands interests into time-sensitive search queries
- Retrieves recent news using DuckDuckGo search
- Filters results based on credibility
- Summarizes top news articles into concise insights
- Supports personalized query-based news retrieval

## Workflow
1. Retrieve user interests from the customer database  
2. Expand interests into search queries using the LLM  
3. Search for recent news articles  
4. Filter search results based on credibility  
5. Summarize the most relevant and credible news  
6. Return a final personalized response  

## Tech Stack
- Python
- LangChain
- SQLDatabase / SQLite
- DuckDuckGo Search
- Hugging Face / Groq LLM integrations
- Pydantic

## Project Structure
.
├── customer.db
├── notebook.ipynb
├── README.md
└── requirements.txt

## Installation
git clone <your-repo-url>
cd <your-repo-folder>
pip install -r requirements.txt

## Environment Setup
Create a `.env` file and add the required API keys:

HF_HUB_API_TOKEN=your_huggingface_token  
GROQ_API_KEY=your_groq_api_key  

## Usage
Run the notebook or Python script and call the main function:

query_response(email="alice.d56e53b6-1@gmail.com", user_query="current events")

## Business Value
- Personalized content delivery
- Improved trust through credibility filtering
- Reduced manual effort through AI automation
- Potential for enterprise and premium use cases

## Challenges Faced
- Tool input and output alignment in agent workflows
- Parsing errors with older LangChain agent setups
- Environment and package version compatibility
- Handling structured and unstructured data together

## Conclusion
This project demonstrates how LLMs, search tools, and databases can be combined to build a scalable and intelligent personalized news assistant.

## Future Enhancements
- Improve credibility scoring with domain ranking
- Introduce user feedback loop
- Add multilingual support
- Deploy as a web application
