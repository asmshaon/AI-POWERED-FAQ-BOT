# AI-Powered FAQ Bot

An intelligent FAQ chatbot powered by Groq's LLM and LangChain, designed to answer questions about Electronic Voting Machines (EVM) based on a curated FAQ dataset.

## Features

- Interactive command-line chatbot interface
- Powered by Groq's LLM (llama-3.1-8b-instant and GPT-OSS-20B)
- Built with LangChain for prompt management and chain creation
- Secure API key handling with getpass prompt

## Prerequisites

- Python 3.12+
- Groq API Key - Get one from [Groq Console](https://console.groq.com)

## Installation

1. Clone the repository:

```bash
git clone git@github.com:asmshaon/AI-POWERED-FAQ-BOT.git
cd AI-Powered-FQA-Bot
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Set up environment variables:

Create a `.env` file in the project root:

```env
GROQ_API_KEY=your_groq_api_key_here
```

Alternatively, the notebook will prompt you to enter the API key at runtime if not found in the `.env` file.

## Usage

### Running the Jupyter Notebook

1. Start Jupyter:

```bash
jupyter notebook
```

2. Open `faq-bot.ipynb`

3. Run all cells to initialize the chatbot

4. Interact with the chatbot in the final cell

### Sample Questions

- "What is EVM?"
- "How does an EVM work?"
- "Is EVM secure?"
- "Who uses EVM?"
- "Can an EVM be tampered with?"

Type `exit` to end the conversation.

## Project Structure

```
AI-Powered-FQA-Bot/
├── faq-bot.ipynb          # Main Jupyter notebook with chatbot implementation
├── requirements.txt        # Python dependencies
├── .env                   # Environment variables (not tracked in git)
├── .env.example           # Example environment file
├── .gitignore            # Git ignore rules
└── README.md             # Project documentation
```

## Technologies Used

- **LangChain** - Framework for building LLM applications
- **Groq** - Fast LLM inference API
- **Python-dotenv** - Environment variable management

## How It Works

1. **Environment Setup**: Loads API keys from `.env` file or prompts user input with getpass
2. **FAQ Data**: Stores predefined questions and answers about Electronic Voting Machines
3. **LLM Chain**: Uses LangChain's PromptTemplate and ChatGroq for response generation
4. **Interactive Loop**: Continuously accepts user questions and generates AI-powered responses
5. **Context-Aware**: Uses the FAQ dataset to provide accurate, contextual answers

## Security Note

Never commit your `.env` file containing API keys to version control. The `.gitignore` file is configured to prevent this.

## Contact

Abu Saleh Muhammad Shaon
Email: srabon.php@gmail.com
GitHub: [@asmshaon](https://github.com/asmshaon)
