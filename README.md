# LangChain RAG (Retrieval-Augmented Generation) Project

This project, **LangChain RAG**, is a Python-based implementation of Retrieval-Augmented Generation (RAG) using a vector database. It leverages LangChain, a framework for building applications powered by language models, to create a system that can retrieve relevant information from a database and generate responses based on the retrieved data.

## Project Structure

- `chroma/`: Contains database files and metadata for the vector database.
- `compare_embeddings.py`: Script for comparing embeddings to analyze similarity between text documents.
- `create_database.py`: Script for creating and populating the vector database with text embeddings.
- `data/`: Contains the text data used in the project.
  - `books/`: Contains the text files of the books.
    - `alice_in_wonderland.md`: "Alice's Adventures in Wonderland" by Lewis Carroll.
    - `animal_farm.md`: "Animal Farm" by George Orwell.
- `LICENSE`: License file for the project (MIT License).
- `query_data.py`: Script for querying data from the vector database and generating responses using LangChain.

## Tech Stack

- **Python**: The primary programming language used for this project.
- **LangChain**: A framework for building applications with language models, enabling retrieval-augmented generation.
- **Vector Database**: A database optimized for storing and querying vector embeddings (e.g., Chroma).
- **Embeddings**: Text embeddings are used to represent text data in a high-dimensional vector space, enabling semantic search and similarity comparisons.

## Getting Started

### Prerequisites

- Python 3.x
- Required Python packages (listed in `requirements.txt`)

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/phonethantzaw/langchain-rag.git
    cd langchain-rag
    ```

2. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

### Usage

1. **Create the Database**:
   Run the `create_database.py` script to generate embeddings for the text data and store them in the vector database.
    ```sh
    python create_database.py
    ```

2. **Compare Embeddings**:
   Use the `compare_embeddings.py` script to compare embeddings and analyze the similarity between different text documents.
    ```sh
    python compare_embeddings.py
    ```

3. **Query Data**:
   Use the `query_data.py` script to query the vector database and generate responses using LangChain's retrieval-augmented generation capabilities.
    ```sh
    python query_data.py 'ADD_YOUR_QUESTION_HERE?'
    ```

## How It Works

1. **Data Preparation**:
   - The text data (e.g., books) is stored in the `data/books/` directory.
   - The `create_database.py` script processes the text files, generates embeddings, and stores them in the vector database (`chroma/`).

2. **Embedding Comparison**:
   - The `compare_embeddings.py` script calculates the similarity between embeddings, allowing you to analyze how closely related different texts are.

3. **Querying and Generation**:
   - The `query_data.py` script retrieves relevant information from the vector database based on a query and uses LangChain to generate a response.

## License

This project is licensed under the **Apache License 2.0**. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- **"Animal Farm" by George Orwell**: A classic novel used as sample data in this project.
- **"Alice's Adventures in Wonderland" by Lewis Carroll**: Another classic novel used as sample data.
- **Project Gutenberg**: For providing the text data used in this project.
- **LangChain**: For providing the framework to build retrieval-augmented generation applications.
- **Chroma**: For providing the vector database used to store and query embeddings.

## Future Enhancements

- Add support for more text data sources (e.g., PDFs, web scraping).
- Implement a user-friendly interface for querying and generating responses.
- Optimize the vector database for larger datasets.
- Explore advanced retrieval techniques, such as hybrid search (combining keyword and vector search).

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Commit your changes.
4. Submit a pull request.

