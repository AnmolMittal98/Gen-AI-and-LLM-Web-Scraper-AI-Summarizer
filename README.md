# Gen-AI and LLM Web Scraper & AI Summarizer

## Overview
This project is a Jupyter Notebook that demonstrates how to scrape website content and generate concise summaries using OpenAI's GPT models. It combines web scraping, text parsing, and AI-powered summarization in a single workflow.

## Features
- **Web Scraping:** Fetches and parses website content using `requests` and `BeautifulSoup`.
- **Content Cleaning:** Removes irrelevant elements (scripts, styles, images, inputs) for cleaner summaries.
- **OpenAI Integration:** Uses the OpenAI API to generate summaries of website content.
- **Markdown Output:** Displays AI-generated summaries in markdown format within the notebook.
- **Reusable Functions:** Includes helper functions for prompt creation, message formatting, and summary display.

## How It Works
1. **Setup:**
   - Loads environment variables from a `.env` file, including your OpenAI API key.
   - Checks for a valid API key and provides troubleshooting tips.
2. **Scraping:**
   - Defines a `Website` class to fetch and parse the target URL.
   - Cleans the HTML to extract readable text.
3. **Prompting & Summarization:**
   - Constructs prompts for the AI model, including system and user messages.
   - Sends requests to OpenAI's GPT model to generate a summary.
   - Displays the summary in markdown format for easy reading.

## Requirements
- Python
- Jupyter Notebook
- `requests`, `beautifulsoup4`, `python-dotenv`, `openai`, `IPython`

## Important Note
**OpenAI API tokens are paid.** You must have a valid, paid OpenAI API key to use the summarization features. Costs may apply based on your usage and OpenAI's pricing.

## Getting Started
1. Clone the repository.
2. Install required packages:
   ```bash
   pip install requests beautifulsoup4 python-dotenv openai IPython
   ```
3. Add your OpenAI API key to a `.env` file:
   ```env
   OPENAI_API_KEY=sk-proj-...
   ```
4. Open the notebook and follow the instructions to summarize any website by providing its URL.

## Disclaimer
- This notebook is for educational and demonstration purposes.
- Ensure you comply with website terms of service when scraping content.


## Additional Free Solution
A new notebook file, `ScraperPlusParserUsingOllama_free.ipynb`, has been added to this folder. It uses the open-source Ollama (llama3.2) model to perform website scraping and summarization for free, without requiring paid API tokens. This provides an alternative to the OpenAI-based workflow for users who prefer a local, no-cost solution.

