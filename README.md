# PDF Question Answering with Open-Source LLMs

This project demonstrates how to build a simple question-answering system for PDF documents using open-source Large Language Models (LLMs) and LangChain. It leverages the following libraries:

- **PyPDF2**: For extracting text from PDF files.
- **LangChain**: For building the question-answering chain and interacting with LLMs.
- **Hugging Face Transformers**: For utilizing pre-trained LLMs and generating text embeddings.
- **Sentence Transformers**: For creating high-quality sentence embeddings.
- **Chroma**: For creating a vector store to efficiently search for relevant information.

## Project Structure

- **your_script.py** (or your notebook file): Contains the Python code for PDF processing, embedding generation, vector store creation, and question-answering chain setup.
- **requirements.txt** (optional): Lists the required Python packages for easy environment setup.
- **your_pdf_file.pdf** (replace with your actual PDF): The PDF document you want to query.

## Getting Started

### Clone the Repository:


\`\`\`bash
git clone <your_github_repo_url>
\`\`\`


### Install Dependencies:

pip install -r requirements.txt  # If you have a requirements.txt file

Or install individual packages as mentioned in the code comments.

### Replace Placeholders:

- Update the \`repo_id\` in the code to point to the desired open-source LLM on Hugging Face.
- Replace \`'/content/Report_Summary (3)-2-4.pdf'\` with the actual path to your PDF file.

### Run the Code:

Execute the Python script or notebook to process the PDF, generate embeddings, create the vector store, and set up the question-answering chain.

### Ask Questions:

Use the \`qa_chain\` object to ask questions about the content of your PDF:


query = "What is the main conclusion of the report?"
result = qa_chain(query)
print(result['result'])

## Customization

- **Choose Your LLM**: Experiment with different open-source LLMs from Hugging Face by changing the \`repo_id\`.
- **Adjust Model Parameters**: Fine-tune the LLM's behavior by modifying the \`model_kwargs\` (e.g., temperature, max length).
- **Text Splitting**: Modify the \`chunk_size\` and \`chunk_overlap\` parameters in the \`RecursiveCharacterTextSplitter\` for different text chunking strategies.

## Contributing

Contributions are welcome! Feel free to open issues or pull requests for improvements, bug fixes, or new features.

## License

This project is licensed under the MIT License.

