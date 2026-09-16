# Development Guide
This is an interactive Jupyter Notebook that serves as a tutorial on Retrieval-Augmented Generation (RAG).

## Important Notes
- The main tutorial file is rag_tutorial.ipynb
- Never install packages. Update the pyproject.toml file instead and run "uv sync".
- Do not create any other external python (.py) files unless they are just temporary scripts.
- All sample code should be in a Jupyter Notebook code cell so that the user can run it interactively. Only sample code to demonstrate the concepts should be created. Code to setup or prepare the sample code is also okay.
- The user must be able to run sample codes that are OpenAI or Ollama compatible.
- Environment variables are expected to be in the .env file.
- The tutorial outline is in rag_tutorial_outline.ipynb
- Create tables, charts, or diagrams if necessary to facilitate learning. Consider these parts of the lecture or lesson material.
- Tables, diagrams, or charts that are part of the lecture should be shown in markdown cells or raw cells, whichever suits best. Do not ask the user to run a code cell just to see a diagram, chart, or table of a lecture. Tables, diagrams, or chart output via code cell execution is permitted as an output of a sample code.
- Check for JSON parsing errors after each change to rag_tutorial.ipynb with: `python -m json.tool rag_tutorial.ipynb`
- Facilitate the learning process by adding snippets of runnable python code in code cells. Include explanations as comments in the code and print statements for demonstration.
- **CRITICAL: Maintain valid JSON structure in Jupyter notebooks** - every string must end with `,` except the last one in an array, and all JSON objects must have proper comma separation
- **Always use UTF-8 encoding** when reading or writing files to prevent character encoding issues
- When running Python scripts, ensure you specify `encoding='utf-8'` in file open operations
- Keep all notebook files as UTF-8 encoded JSON
- Environment variables should be set in the `.env` file using UTF-8 encoding

## Environment Variables

BASE_URL
LLM_MODEL
EMBEDDING_MODEL
API_KEY

## Specific Package Versions for pyproject.toml

- Python 3.11.9
- LangChain:
  - Core: >=0.3.0
  - langchain: >=0.3.0
  - langchain-community: >=0.3.0
  - langchain-text-splitters: >=0.3.0
  - langchain-ollama>=0.2.0
  - langchain-openai>=0.2.0

