
# News Researcher Tool

# Overview

The News Researcher Tool is a powerful application designed to facilitate efficient research and information retrieval from news articles. By utilizing advanced natural language processing and machine learning techniques, this tool allows users to extract, process, and query information from a set of provided article links.

# Workflow
## Input Links:
Users can input up to three article links into the application.
## Text Extraction:
The application employs the LangChain library to extract text content from the provided article links.
## Preprocessing:
Text undergoes preprocessing steps to enhance the quality of information.
The processed text is then split into multiple chunks for further analysis.
## Embedding Generation:
Hugging Face embeddings are applied to the text chunks, providing rich contextual representations.
These embeddings capture semantic information crucial for downstream tasks.
## Vector Database (FAISS):
The generated embeddings are stored in a vector database called FAISS.
FAISS allows for efficient storage and retrieval of embeddings, forming a robust foundation for subsequent queries.
## Question Answering:
When a user posts a question related to the articles, the Hugging Face Language Model (LLM) utilizes the FAISS vector database.
LLM leverages the embeddings to find the most relevant information, providing accurate and contextually appropriate answers.
## Article Retrieval:
In addition to answering questions, the tool returns the article that contains the answer.
This feature aids users in gaining a comprehensive understanding of the context surrounding the query.
## Usage
To use the News Researcher Tool, follow these simple steps:

Paste up to three article links into the designated input area.
Submit the links to initiate the extraction and processing workflow.
Post questions related to the articles to receive accurate and informative answers.
Review the provided article that contains the answer to the posed question.
