# 🪄 peak-genie: PDF Question-Answer tool

peak-genie is an AI-powered PDF QA tool that enables you to easily upload and analyze PDF documents with **advanced question-answering capabilities**. peak-genie goes beyond traditional keyword-based search and utilizes *vector embeddings* and *semantic search* to deliver precise and efficient results from your PDFs to improve your workflow efficiency.

## Installation

2. Navigate to the project directory by running `cd peak-genie`
3. Install the required packages using `pip install -r requirements.txt`

## Usage

To use peak-genie, simply run `python -m streamlit run folder-location/peak-genie/streamlit/main.py` in your terminal. This will start a local server that you can access through your web browser.
In the command, replace folder-location/ with the actual path to the peak-genie directory on your machine.



## Environment Variables

Before running the app, make sure to create a `.env` file in your local system and add the following environment variables:

```
OPENAI_API_KEY=<your openai api key>
PINECONE_API_KEY=<your pinecone api key>
PINECONE_API_ENV=<your pinecone api env>
USE_PINECONE=false
PINECONE_INDEX_NAME=<test>
TEMPERATURE=0
QA_WITH_SOURCE=false
```


For streamlit applications. Secrets management happens from a different file. See [this](https://docs.streamlit.io/streamlit-community-cloud/get-started/deploy-an-app/connect-to-data-sources/secrets-management) for more information.

Add a file called `secrets.toml` in a folder called `.streamlit` at the root of your app repo, and copy/paste your secrets into that file.
```
OPENAI_API_KEY="your openai api key"
PINECONE_API_KEY="your pinecone api key"
PINECONE_API_ENV="your pinecone api env"
USE_PINECONE="false"
PINECONE_INDEX_NAME="test"
TEMPERATURE="0"
QA_WITH_SOURCE="false"
```

## Architecture
![My Image](images/peak-genie.png "peak-genie Architecture")


