# Dialogue Dataset Generator for Text-to-SQL Agents

A framework for automatically generating dialogue datasets specifically designed for Text-to-SQL agents. This tool helps create realistic conversations that explore various SQL join combinations and query scenarios.

## Overview

The Dialogue Dataset Generator is designed to create high-quality data for Text-to-SQL agents by:
- Automatically identifying and exploring join combinations within database schemas
- Generating natural language dialogues that correspond to complex SQL queries
- Ensuring balanced representation of different join types and table combinations
- Creating realistic user-agent interactions for SQL query generation

## Features

- **Join Combination Analysis**: Automatically identifies and analyzes possible join combinations within database schemas
- **Balanced Dataset Generation**: Ensures equitable representation of tables and join types
- **Natural Language Generation**: Creates realistic dialogues using LLMs
- **Configurable**: Supports customization of dialogue generation parameters

## Requirements

- Python 3.11+
- Dependencies listed in `requirements.txt`:
  - LangChain and LangGraph for LLM integration
  - Pandas and NumPy for data manipulation
  - NetworkX for graph operations
  - Jupyter Notebook for development and analysis

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/dialogue-dataset-generator.git
cd dialogue-dataset-generator
```

2. Create and activate a virtual environment:
```bash
python3.11 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Set up environment variables:
Create a `.env` file with your configuration:
```
AZURE_OPENAI_BASE_URL=...
AZURE_OPENAI_API_KEY=...
OPENAI_API_VERSION=...
```

## Usage

The framework consists of two main components:

1. **Join Combination Analysis** (`part-1-join_combinations.ipynb`):
   - Analyzes database schema
   - Identifies possible join combinations
   - Generates balanced join scenarios

2. **Dialogue Generation** (`part-2-creating-dialogues.ipynb`):
   - Creates natural language dialogues
   - Generates corresponding SQL queries
   - Ensures realistic user-agent interactions

## Project Structure

```
dialogue-dataset-generator/
├── mondial/              # mondial data
├── part-1-join_combinations.ipynb
├── part-2-creating-dialogues.ipynb
├── llm_config.py        # LLM configuration
├── requirements.txt     # Project dependencies
└── .env                 # Environment variables
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. Or send me an e-mail: matheusolivsilv.ai@gmail.com
