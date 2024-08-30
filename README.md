# Custom Chatbot Using Langchain
This repository contains the code for a custom chatbot that extracts data from a specific website, creates embeddings, stores them in a vector store, and interacts with users through a Flask RESTful API.

## Features
### Web Scraping: 
Extracts course data from Brainlox Technical Courses using BeautifulSoup.
### Embeddings: 
Uses OpenAI embeddings via Langchain to generate vector embeddings for the course data.
### Vector Store: 
Stores the embeddings in FAISS, a vector store for efficient similarity search.
### Conversational API: 
Provides a RESTful API to handle conversation inputs and generate context-aware responses.

## Setup
### Extract Data: 
Run the script to scrape course data from the specified URL.


### Create Embeddings: 
Generate embeddings and store them in the vector store.


### Run the Flask API: 
Start the Flask server to interact with the chatbot.


## Usage
Once the Flask server is running, you can interact with the chatbot by sending POST requests to the /chat endpoint.

## Example Request

curl -X POST http://127.0.0.1:5000/chat -H "Content-Type: application/json" -d '{"message": "Tell me about the courses available?"}'
## Example Response
json
Copy code
{
  "response": "Here are some courses available: Course A, Course B, Course C..."
}

## Contributing
Feel free to submit issues or pull requests if you want to improve the project.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgements
Langchain
OpenAI
BeautifulSoup
