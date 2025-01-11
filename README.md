




Gemma Model Document Q&A
Gemma Model Document Q&A is a Streamlit-based application that provides accurate and context-driven answers to user queries from document collections. It combines the power of LangChain, GROQ LLM, and Google Generative AI embeddings to process documents, build a vector database, and retrieve relevant information.

📝 Features
Upload and process PDF documents for embedding.
Create a vector database using Google Generative AI embeddings for efficient document search.
Generate accurate answers based on the provided document context using LangChain and GROQ LLM.
Perform document similarity searches to display the most relevant chunks.
📂 Folder Structure
bash
Copy code
project/
│
├── Gemma/
│   ├── main.py             # Main application script
│   ├── us_census/          # Directory containing PDF documents
│   ├── .env                # Environment variables (API keys)
│   └── requirements.txt    # Dependencies
│
└── README.md               # Project documentation
🛠️ Technologies Used
LangChain: For building LLM-powered question-answering chains.
FAISS: For vector-based document retrieval.
Streamlit: To create an interactive user interface.
Google Generative AI: For generating embeddings.
PyPDFLoader: For loading and processing PDF documents.
🔧 Installation
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/gemma-document-qa.git
cd gemma-document-qa
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
Set up the .env file: Create a .env file in the root directory and add your API keys:

makefile
Copy code
GROQ_API_KEY=your_groq_api_key
GOOGLE_API_KEY=your_google_api_key
Prepare your document directory: Place all PDF files in the us_census folder (or change the path in the script as needed).

▶️ Usage
Run the application:

bash
Copy code
streamlit run main.py
Embed documents:

Click the "Documents Embedding" button to process PDFs and create the vector database.
Ask questions:

Enter a question in the input field to retrieve answers based on document context.
View relevant document chunks in the "Document Similarity Search" section.
⚠️ Important Notes
Ensure your .env file is properly set up with the required API keys.
The us_census folder should contain all the documents you want to query.
Adjust the chunk_size and chunk_overlap parameters in the script for better document processing based on your dataset.
🛡️ License
This project is licensed under the MIT License.

🙋 Contact
For any questions or support, feel free to contact:

Ananya Midha
📧 midhaananya@gmail.com

This version improves formatting, organizes the content into clear sections, and provides proper code blocks for commands. Let me know if you'd like further adjustments!
