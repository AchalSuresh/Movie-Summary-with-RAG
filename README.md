# Movie-Summary-with-RAG
Using Retrieval-Augmented Generation to Search a Movie Database Using Langchain, OpenAI and Pinecone

![Alt Text](https://framerusercontent.com/images/qtQMAzQadKJO9iaAe0MsjIcLNg.jpg)

**Overview**
This project implements Retrieval-Augmented Generation (RAG) to build a question-answering bot for movie-related queries. By leveraging large language models (LLMs) along with vector search, we enhance the ability of the model to provide factual responses without requiring fine-tuning or retraining.

Instead of relying solely on pre-trained knowledge, the model retrieves relevant movie descriptions from a vector database and uses them as context to generate more accurate and informative answers.

**Dataset Used**
Data containing 4900 top movies from IMDB

**How It Works 🚀**

1️) Extract & Process IMDB Data – Movie descriptions are extracted and preprocessed from IMDB.  
2️) Create Vector Embeddings – We generate vector embeddings using OpenAI's text-embedding-ada-002 model.  
3️) Store & Search in Pinecone – These embeddings are stored in Pinecone, a high-performance vector database, enabling semantic search.  
4️) Generate Answers with GPT-3.5 – When a user asks a movie-related question, the system retrieves relevant embeddings and provides them as context to OpenAI’s GPT-3.5-Turbo, enhancing the accuracy of responses.  
5️) Orchestrate with LangChain – LangChain facilitates seamless interaction between OpenAI, Pinecone, and the user query.  

**Tech Stack & Tools 🛠**  
* OpenAI GPT-3.5-Turbo – Generates natural language responses.  
* OpenAI text-embedding-ada-002 – Converts movie descriptions into vector embeddings.  
* Pinecone – Stores and retrieves embeddings for relevant context.  
* LangChain – Handles orchestration between the LLM, vector database, and retrieval pipeline.  
* Pandas & Python – For preprocessing and structuring the IMDB dataset.  

**Use Cases 🎯**  
✔ Find movie recommendations based on descriptions  
✔ Retrieve factual movie information with context  
✔ Answer questions about movie genres and storylines  

**Next Steps & Enhancements 🚀**
🔹 Expand the dataset with actor bios, movie reviews, and box office data  
🔹 Optimize retrieval mechanisms for faster and more accurate searches  

