# LLM-Powered-PDF-Q-A-Assistant
Build a tool that ingests a set of PDF documents, indexes them in a vector database (e.g., FAISS or Pinecone), and lets users ask questions. The answer should be generated using RAG—retrieving relevant context chunks, then generating a response using an LLM (OpenAI API or open-source model).
# LLM-Powered PDF Q&A Assistant

🤖 A Streamlit web app that allows users to upload PDF documents and ask questions about their content using Large Language Models (LLMs) via OpenAI.

---

## Features

- Upload one or more PDF files via a web interface.
- Extract and index PDF text for semantic search.
- Answer user questions based on PDF content using OpenAI’s GPT models.
- Display retrieved relevant text passages alongside generated answers.
- Interactive and user-friendly Streamlit UI.

---

## Demo

*Add a link to a live demo here if available*

---

## Getting Started

### Prerequisites
- Python 3.8 or higher
- An OpenAI API key with available quota ([Get it here](https://platform.openai.com/account/api-keys))
- `pip` package manager

### Installation

1. Clone this repository:
    ```
    git clone https://github.com/yourusername/llm-pdf-qa.git
    cd llm-pdf-qa
    ```

2. Create and activate a virtual environment (optional but recommended):
    ```
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3. Install required packages:
    ```
    pip install -r requirements.txt
    ```

4. Create a `.env` file in the project root with your OpenAI API key:
    ```
    OPENAI_API_KEY=sk-your-openai-api-key
    ```
    
Open the local URL shown in your terminal (usually `http://localhost:8501`) to use the app. Upload PDFs and start asking questions!

---

## Project Structure

- `app.py`: Main Streamlit application script.
- `ingest.py`: Handles PDF ingestion and text extraction.
- `qa_chain.py`: Contains the logic for question answering using LLMs.
- `.env`: Stores environment variables such as OpenAI API key (not committed).
- `requirements.txt`: Python dependencies.
- Other helper modules & assets as needed.

---

## Troubleshooting

- **ModuleNotFoundError for some packages:**
  Ensure all dependencies are installed from `requirements.txt`.
  
- **OpenAI API key errors:**
  Make sure `.env` file is present **in the same folder as `app.py`** and contains a valid `OPENAI_API_KEY`.

- **Quota or rate limit exceeded:**
  Check your OpenAI dashboard for usage and billing status.

---

## License

MIT License.

---

## Acknowledgements

- Built with [Streamlit](https://streamlit.io/)
- Powered by [OpenAI GPT](https://openai.com/)
- Uses [python-dotenv](https://pypi.org/project/python-dotenv/) for environment variable management.

---

## Contact

Your Name – yamini.rc59@gmail.com  
Project Link: https://github.com/yamini-datascientist/llm-pdf-qa


---

### Running the App

Start the Streamlit app with this command:

