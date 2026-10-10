# 🕵️‍♂️ AI Agent with Function Calling
A command-line AI agent built in Python using the OpenAI SDK. The agent can understand natural language prompts and autonomously call functions (tools) to interact with a local file system — reading files, listing directories, writing files, and executing Python scripts.

## Features
- Conversational interface powered by an LLM
- Custom system prompt to guide agent behavior
- Function calling / tool use, allowing the agent to:
  - List files and directories
  - Read file contents
  - Write to files
  - Execute Python files
- Iterative agent loop supporting multi-step reasoning

## Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/georlia/AI-agent.git
   cd AI-agent

2. Install dependencies using uv:
   ```bash
    uv sync
3. Create a .env file in the root directory with your API key:
   ```bash
   API_KEY=your_key_here

## Usage
Run the agent with a prompt:
 ```bash
   uv run main.py "your prompt here"
 ```
Example:
 ```bash
   uv run main.py "What is the square root of 4?"
 ```

## Project Structure
```text
.
├── functions/        # Tool functions the agent can call
├── main.py           # Entry point
├── prompts.py        # System prompt definition
├── config.py         # Configuration values
└── tests/            # Unit tests
```

## Built With
* Python
* OpenAI SDK
* uv for dependency management
