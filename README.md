# Multi-PDF Chatbot using LangChain and Gemmini AI

This project showcases a multi-PDF chatbot built using [LangChain](https://langchain.com/) and the Gemmini AI API. The chatbot leverages LangChain’s capabilities to parse multiple PDF documents and answer questions based on their content, making it ideal for handling extensive documentation or multi-file references.

## Table of Contents
- [Features](#features)
- [Setup and Installation](#setup-and-installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [API Key Management](#api-key-management)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

---

## Features
- **Multi-PDF Parsing**: Processes multiple PDFs at once.
- **Question-Answering**: Answers queries based on parsed PDF content.
- **Contextual Memory**: Remembers conversation context for a better user experience.
- **Gemmini AI Integration**: Uses the Gemmini API for language model capabilities.
  
## Setup and Installation

### Prerequisites
- Python 3.8 or higher
- Gemmini AI API Key (available on [Gemmini AI](https://gemmini.com))
- [LangChain](https://python.langchain.com/en/latest/) library
- PDF processing libraries (e.g., `PyMuPDF`)

### Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/multi-pdf-chatbot.git
    cd multi-pdf-chatbot
    ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Install additional tools for PDF processing if needed:
    ```bash
    pip install pymupdf
    ```

## Configuration

1. **API Key**: Create a `.env` file in the root directory and add your Gemmini AI API key:
    ```plaintext
    GEMMINI_API_KEY=your_gemmini_api_key
    ```

2. **LangChain Configuration**: Adjust LangChain settings in `config.py` as per your model and memory requirements.

3. **PDF Storage**: Place the PDF files to be parsed in the `pdf_files` directory or adjust the script to point to your preferred folder.

## Usage

1. **Run the Chatbot**:
    ```bash
    python app.py
    ```

2. **Interacting with the Chatbot**: Ask questions based on the PDF content. The chatbot will parse PDFs and respond based on the information extracted.

3. **Sample Query**:
    - **User**: "What is the main topic of Document A?"
    - **Bot**: "Document A primarily discusses..."

## API Key Management

The API key for Gemmini AI should be kept secure. Avoid sharing or hardcoding it in files. Use environment variables to securely store your API key.

## Technologies Used
- **LangChain**: Framework for building language model applications.
- **Gemmini AI**: For natural language processing capabilities.
- **PyMuPDF**: For efficient PDF parsing.
- **Flask** (optional): For a web interface to access the chatbot.
  
## Contributing

Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature: `git checkout -b feature-name`.
3. Commit your changes: `git commit -m "Added new feature"`.
4. Push to the branch: `git push origin feature-name`.
5. Submit a pull request.

## License
This project is licensed under the MIT License.
