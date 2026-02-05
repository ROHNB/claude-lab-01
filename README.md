# Claude Lab 01

A Python project for experimenting with the Anthropic Claude API.

## Project Overview

This project provides an interactive command-line interface for chatting with Claude, demonstrating basic API usage and conversation management.

## Project Structure

```
claude-lab-01/
├── test.py                 # Main interactive chat application
├── requirements.txt        # Python dependencies
├── .env.example           # Environment variable template
├── .env                   # Environment variables (local, not in git)
├── .gitignore            # Git ignore rules
├── claude-lab-01-env/    # Python virtual environment
└── README.md             # This file
```

## Setup Instructions

### Prerequisites
- Python 3.8+
- Anthropic API key from https://console.anthropic.com

### Installation

1. Create environment variables file:
```bash
Copy-Item .env.example .env
```

2. Edit `.env` and add your API key:
```
ANTHROPIC_API_KEY=sk-ant-...your-key-here...
```

3. Activate virtual environment:
```bash
.\claude-lab-01-env\Scripts\Activate.ps1
```

4. Install dependencies (if not already installed):
```bash
pip install -r requirements.txt
```

## Usage

Run the interactive chat:
```bash
python test.py
```

Then type messages to chat with Claude. Enter `exit` to quit.

## Dependencies

- `anthropic>=0.77.1` - Anthropic API client
- `python-dotenv>=1.0.0` - Environment variable management

## Features

- Interactive command-line chat interface
- Environment variable configuration for API key security
- Clean separation of concerns
- Ready for extensibility

## Development

This project is configured with:
- Virtual environment (`claude-lab-01-env`)
- `.gitignore` for security (protects .env and `__pycache__`)
- `requirements.txt` for dependency management

## Notes

- API keys are stored in `.env` (not committed to git)
- Virtual environment is local and not committed
- The project uses Claude 3.5 Sonnet model by default
