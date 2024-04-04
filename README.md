# Chatbot Based on Internal Data (PDFs)

This project demonstrates the process of creating a chatbot that leverages internal data sources, specifically PDF documents and web pages, to generate responses. The chatbot utilizes a Retrieval-Augmented Generation (RAG) architecture, incorporating vector embeddings from documents to provide informative and contextually relevant answers.

## Getting Started

These instructions will guide you through setting up the project locally to run the chatbot.

### Prerequisites

Before you begin, ensure you have Python installed on your system. You will also need access to the required libraries and tools listed under the "Installation" section.

### Installation

Follow these steps to set up your development environment:

```bash
# Clone the repository
git clone https://github.com/yourgithubprofile/chatbot-pdf-data.git

# Navigate to the project directory
cd chatbot-pdf-data

# Install necessary Python packages
pip install -r requirements.txt
```

## Usage

To start the chatbot, run the Jupyter notebook:

```bash
jupyter notebook main.ipynb
```

Follow the instructions within the notebook to interact with the chatbot.

## Architecture

The project is structured around several key steps:

1. **Data Loading**: Utilizing `PyPDFDirectoryLoader` and `AsyncHtmlLoader` for reading PDFs and web pages.
2. **Data Transformation**: Applying `Html2TextTransformer` for converting HTML content to text.
3. **Text Splitting**: Chunking text using `RecursiveCharacterTextSplitter`.
4. **Vector Embedding**: Generating vector embeddings for the chunks using `CohereEmbeddings`.
5. **Chatbot Implementation**: Creating a chatbot that queries a Pinecone vector database to fetch relevant content.

### Tools and Libraries Used

- Jupyter Notebook: For interactive development and demonstrations.
- Python: The primary programming language.
- `langchain`, `langchain_community`, and `langchain_cohere`: For document processing, text splitting, and embedding generation.

### Implementation Details

The notebook includes detailed code cells for each step of the process, from loading and processing documents to initializing and querying the chatbot.


## Authors

- **Sandeep Polavarapu** - *Initial work* - [YourGitHubProfile](https://github.com/sandeeppvn)

See also the list of contributors who participated in this project.



