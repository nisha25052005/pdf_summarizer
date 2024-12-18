# PDF Summarization Tool

This is a Python-based project that extracts and summarizes text from uploaded PDF files using Streamlit for the user interface, PyPDF2 for PDF text extraction, SpaCy for sentence segmentation, and the BERT Extractive Summarizer for text summarization.

## Features
- Upload a PDF file through a user-friendly interface.
- Extract and display the full text from the PDF.
- Summarize the extracted text using a pre-trained BERT model.

---

## Prerequisites

1. **Python**: Ensure Python 3.8 or higher is installed on your system.
   - [Download Python](https://www.python.org/downloads/)

2. **Pip**: Install `pip` (Python's package installer) if not already available.
   ```bash
   python -m ensurepip --upgrade
   ```

3. **Visual Studio Code (VS Code)**: A code editor for running and modifying the project.
   - [Download VS Code](https://code.visualstudio.com/)

---

## Setup Instructions

### Step 1: Clone or Download the Project
1. If you have downloaded the ZIP file, extract it to your desired location.

---

### Step 2: Create a Virtual Environment (Optional but Recommended)
1. Open your terminal and navigate to the project directory.
2. Create a virtual environment:
   ```bash
   python -m venv venv
   ```
3. Activate the virtual environment:
   - **Windows**:
     ```bash
     venv\Scripts\activate
     ```
   - **Mac/Linux**:
     ```bash
     source venv/bin/activate
     ```

---

### Step 3: Install Dependencies
Install the required Python packages listed in `requirements.txt`:

1. Navigate to the project directory in your terminal.
2. Run the following command:
   ```bash
   pip install -r requirements.txt
   ```

If `requirements.txt` is not available, manually install the following packages:
```bash
pip install streamlit PyPDF2 bert-extractive-summarizer spacy
python -m spacy download en_core_web_md
```

---

### Step 4: Run the Application
1. In the terminal, navigate to the project directory.
2. Start the Streamlit app:
   ```bash
   streamlit run mainapp.py
   ```
3. The application will open in your default web browser. If it does not, copy the URL displayed in the terminal (e.g., `http://localhost:8501`) and paste it into your browser.

---

## Project Structure
```
project-directory/
|-- mainapp.py              # Main application file
|-- requirements.txt        # List of required dependencies
|-- README.md               # Project documentation
```

---

## Troubleshooting
- **Error: ModuleNotFoundError**: Ensure all dependencies are installed.
- **Error during summarization**: Ensure the `en_core_web_md` model is downloaded for SpaCy.
- **Browser does not open**: Check the terminal output for the local URL and manually open it in your browser.

---

## Notes
- This tool works best with English-language PDFs.
- Ensure the PDF contains selectable text (i.e., not scanned images). For scanned PDFs, integrate OCR tools like Tesseract for text extraction.

---

## Future Enhancements
- Add support for multilingual text summarization.
- Improve the UI with advanced customization options.
- Integrate OCR capabilities for scanned PDFs.



