![image](https://github.com/user-attachments/assets/c3ff69ac-de3a-449c-b35e-07ef4c8d8438)

## Business Use Case

**Problem Statement:**

Finsights Grey Inc. is an innovative financial technology firm that specializes in providing advanced analytics and insights for investment management and financial planning. The company handles an extensive collection of 10-K reports from various industry players, which contain detailed information about financial performance, risk factors, market trends, and strategic initiatives. Despite the richness of these documents, Finsights Grey's financial analysts struggle with extracting actionable insights efficiently in a short span due to the manual and labor-intensive nature of the analysis. Going through the document to find the exact information needed at the moment takes too long. This bottleneck hampers the company's ability to deliver timely and accurate recommendations to its clients. To overcome these challenges, Finsights Grey Inc. aims to implement a Retrieval-Augmented Generation (RAG) model to automate the extraction, summarization, and analysis of information from the 10-K reports, thereby enhancing the accuracy and speed of their investment insights.

**Objective:**

As a Gen AI Data Scientist hired by Finsights Grey Inc., the objective is to develop an advanced RAG-based system to streamline the extraction and analysis of key information from 10-K reports.

The project will involve testing the RAG system on a current business problem. The Financial analysts are asked to research major cloud and AI platforms such as Amazon AWS, Google Cloud, Microsoft Azure, Meta AI, and IBM Watson to determine the most effective platform for this application. The primary goals include improving the efficiency of data extraction. Once the project is deployed, the system will be tested by a financial analyst with the following questions. Accurate text retrieval for these questions will imply the project's success.

**Questions:**

1. Has the company made any significant acquisitions in the AI space, and how are these acquisitions being integrated into the company's strategy?

2. How much capital has been allocated towards AI research and development?

3. What initiatives has the company implemented to address ethical concerns surrounding AI, such as fairness, accountability, and privacy?

4. How does the company plan to differentiate itself in the AI space relative to competitors?

Each Question must be asked for each of the five companies.

By successfully developing this project, we aim to:

Improve the productivity of financial analysts by providing a competent tool.

Provide timely insights to improve client recommendations.

Strengthen FinTech Insights Inc.’s competitive edge by delivering more reliable and faster insights to clients.

Steps involved in this Sample RAG implementation use case.

Setup - 
  # Import the necessary Libraries
Implementing RAG
Prepare Data - 
  # Upload Dataset-10k.zip and unzip it dataset folder using -d option
Chunking - 
  # Provide pdf_folder_location
  # Load the directory to pdf_loader
  # Create text_splitter
  # Create chunks
  # Check the total number of chunks
  # Check the first object in report_chunks and print it
Database Creation
  # Create a Collection Name
  # Initiate the embedding momdel 'thenlper/gte-large'
  # Create the vector Database
  # Persist the DB
  # Mount the Google Drive
  # Copy the persisted database to your drive
Test your RAG Application
  # Install the required packages
  # Import the necessary Libraries
Authentication
Mount Google Drive
Load Vector DB from Google Drive
  # Initialise the embedding model
  # Load the persisted DB
  # Create a Colelction Name
  # Load the persisted DB
test our database with a sample question
RAG Q&A
Prompt Design
  # Create a system message for the LLM
  # Create a message template
  # Create a variable company to store the source of the context so that you can filter the similarity search
  # Create context for query by joining page_content and page number of the retrieved docs
  # Craft the messages to pass to chat.completions.create
  # Get a response from the LLM
Evaluation
  # Create a prompt for the rater LLM to check the groundedness of the response
  # Create a prompt for the rater LLM to check the relevance of the response
  # Create user message template such that question, answer and context can be provided through it
  # Create messages for groundness
  # Print the response of the rater LLM on groundedness
  # Print the response of the rater LLM on relevance
Evaluation on multiple QUeries

  
  
  

