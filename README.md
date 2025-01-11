

#Gemma Model Document Q&A
Gemma Model Document Q&A is a Streamlit-based application designed to provide accurate and context-driven answers to user queries from document collections. It leverages advanced language models and vector embeddings for document processing, retrieval, and question answering.

📝 Features
Upload and process PDF documents for embedding.
Use Google Generative AI embeddings to create a vector database for efficient document search.
Answer user queries based on the provided documents using LangChain and GROQ LLM.
Perform document similarity searches to display relevant chunks of text.
📂 Folder Structure
graphql
Copy code
project/
│
├── Gemma/
│   ├── main.py           
│   ├── us_census/        # Directory containing PDF documents
│   ├── .env              
│   └── requirements.txt  # Dependencies
│
└── README.md             
🛠️ Technologies Used
LangChain: For building LLM-powered question-answering chains.
FAISS: For vector-based document retrieval.
Streamlit: For building an interactive user interface.
Google Generative AI: To generate embeddings for document processing.
PyPDFLoader: For loading and processing PDFs.
🔧 Installation
Clone the repository:

bash
Copy code

Set up a virtual environment:

bash
Copy code
python -m venv venv
source venv/bin/activate    # macOS/Linux
.\venv\Scripts\activate     # Windows
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Create a .env file: Add your API keys in a .env file in the following format:

makefile
Copy code
GROQ_API_KEY=your_groq_api_key
GOOGLE_API_KEY=your_google_api_key
Prepare your document directory: Add all your PDF files to the us_census folder (or change the path in the script accordingly).

▶️ Usage
Run the application:

bash
Copy code
streamlit run main.py
Embed documents:

Click the "Documents Embedding" button to create the vector database.
Ask questions:

Enter your question in the text input field and get answers based on the embedded documents.
Expand "Document Similarity Search" to view relevant document chunks.
⚠️ Important Notes
Ensure your .env file is properly set up with the required API keys.
The us_census folder should contain all the documents you want to query.
Adjust the chunk_size and chunk_overlap parameters for better performance based on your document structure.
🛡️ License
This project is licensed under the MIT License.

🙋 Contact
For questions or support, reach out to Ananya Midha at midhaananya@gmail.com.

