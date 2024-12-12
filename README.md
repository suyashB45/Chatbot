# Chat with PDF using Gemini 💁  

This project enables users to interact with PDF documents through a conversational interface powered by Google Generative AI and FAISS vector stores. By uploading PDF files, users can ask questions and receive detailed responses based on the document content.  

## Features  

- **PDF Upload and Processing**: Extract text from uploaded PDF files.
- **Text Chunking**: Split large text into manageable chunks for better processing.
- **Embedding and Indexing**: Use Google Generative AI embeddings to create a searchable vector store.
- **Conversational Chain**: Answer user queries using Google Gemini Pro with custom prompts.
- **Streamlit Interface**: User-friendly web interface for uploading files and interacting with the model.

## Demo  

![LangChain Logo](https://media.licdn.com/dms/image/D4D12AQHR6_vWjjNyPQ/article-cover_image-shrink_720_1280/0/1684226004055?e=2147483647&v=beta&t=NqJ6P94aqLjACBX7FZzLsotcUlR35WJgq4FQn96AMN8)  
![Google Gemini AI](https://s.yimg.com/ny/api/res/1.2/FWWVOW6s2MUFV_yLq9E36g--/YXBwaWQ9aGlnaGxhbmRlcjt3PTEyMDA7aD02NzU-/https://s.yimg.com/os/creatr-uploaded-images/2023-12/5f7be670-943f-11ee-af7f-41b7060d20ba)  

Check out this video demonstration of the app in action:  

[![Chat with PDF Demo](https://img.youtube.com/vi/PRnsPYJ8I2E/0.jpg)](https://youtu.be/PRnsPYJ8I2E?si=qXK64rFUNh4jUY2g)  

## Technologies Used  

- **Python**  
- **Streamlit**: For building the web interface.  
- **PyPDF2**: For reading text from PDF files.  
- **LangChain**: For text splitting and managing conversational AI chains.  
- **Google Generative AI (Gemini)**: For embeddings and conversational responses.  
- **FAISS**: For efficient similarity search on vectorized text.  
- **dotenv**: For managing API keys securely.  

## How It Works  

1. **Upload PDF Files**: Use the sidebar to upload one or more PDF documents.  
2. **Process PDF Files**: Extract and split text into smaller chunks for processing.  
3. **Generate Embeddings**: Create vector embeddings using Google Generative AI.  
4. **Ask Questions**: Input questions based on the uploaded content to receive detailed answers.  

## Setup  

1. Clone the repository:  
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```  

2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```  

3. Add your Google API key to a `.env` file:  
   ```env
   GOOGLE_API_KEY=your_google_api_key
   ```  

4. Run the Streamlit app:  
   ```bash
   streamlit run app.py
   ```  

## Usage  

- Navigate to the app in your browser.  
- Upload PDF files via the sidebar.  
- Ask questions about the uploaded documents using the input field.  

## Notes  

- Ensure that the Google API key has access to Google Generative AI services.  
- If the FAISS index is not found, re-upload and process the PDF files.  

## Future Enhancements  

- Add support for additional file formats (e.g., Word, TXT).  
- Implement multi-language support for PDFs.  
- Optimize response time for large documents.  

## License  

This project is licensed under the MIT License.  

## Acknowledgments  

- [Streamlit](https://streamlit.io/)  
- [LangChain](https://www.langchain.com/)  
- [FAISS](https://github.com/facebookresearch/faiss)  
- [Google Generative AI](https://ai.google/)  
```  

Let me know if you need further adjustments!
