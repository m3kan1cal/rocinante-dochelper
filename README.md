# Welcome to rocinante-dochelper

Simple repository demoing how to train OpenAI LLM using LangChain, embeddings, vector DBs, RetrievalQA, and memory on text documents for querying.

## Getting Started

A pre-requisite for this project is to have Python 3.11 installed on your machine, and to have some basic familiarity
with the language. You can find the installation instructions for Python [here](https://www.python.org/downloads/).

1. Clone this repository.
2. Install dependencies.

    ```bash
    pip install -r requirements.txt
    ```

3. Create a trial account on [Pinecone](https://pinecone.io).
4. Create a new index on Pinecone called `langchain-docs-index`. Use `euclidean` as the index type and `1536` as the dimension.
5. Copy your Pinecone API key from the Pinecone console. 
6. Create an environment variable with the key `PINECONE_API_KEY` and the value of the copied API key.
7. Copy the environment name from the Pinecone console.
8. Create an environment variable with the key `PINECONE_ENVIRONMENT_REGION` and the value of the copied environment name.
9. Create an account on [OpenAI](https://platform.openai.com/).
10. Copy your OpenAI API key from the OpenAI console.
11. Create an environment variable with the key `OPENAI_API_KEY` and the value of the copied API key.
12. Run the script, but replace the `PATH_TO_PYTHON_INTERPRETTER` with the path to your Python interpreter.

    ```bash
    /{PATH_TO_PYTHON_INTERPRETER}/bin/streamlit run main.py
    ```

13. Go to `http://localhost:8501` in your browser to see the app and use the prompt.

This is intended to give a general idea on how you can simply use Pinecone and OpenAI to build a simple search engine for text documents.
