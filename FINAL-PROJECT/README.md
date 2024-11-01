
# Dhiwise Selection Task - Recruitment Process Automation Tool

This project is part of the Dhiwise 2nd round selection process, designed to automate key aspects of the recruitment workflow by aligning resumes with job descriptions and analyzing interview content.

## Project Overview

This tool is developed to streamline the recruitment process by:
1. Matching resumes with job descriptions for optimal candidate alignment.
2. Analyzing interview video content to summarize and extract insights.

## Installation

### Requirements

Ensure you have **Python 3** installed. This project also requires the following libraries:

- `streamlit`
- `langchain`
- `langchain-openai`
- `langchain-google-genai`
- `faiss-cpu`
- `tiktoken`
- `python-dotenv`
- `pdfminer`
- `markdown`

All dependencies are listed in `requirements.txt`.

### Installation Steps

1. **Clone the Repository**

   ```bash
   git clone <repository_url>
   cd <repository_name>
   ```

2. **Set Up a Virtual Environment**

   ```bash
   python -m venv virtualenv
   ```

3. **Activate the Virtual Environment**

   - **Windows**: 
     ```bash
     .\virtualenv\Scripts\activate
     ```
   - **Linux/Mac**: 
     ```bash
     source virtualenv/bin/activate
     ```

4. **Install Required Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

5. **Configure API Keys**

   Add your API keys (`LANGCHAIN_API_KEY`, `PINECONE_API_KEY`, `GOOGLE_GEMINI_API_KEY`, `ASSEMBLY_AI_API_KEY`) to `keys.env`. Obtain these keys from their respective provider websites.

## Running the Application

1. **Start the App**

   ```bash
   streamlit run ./Streamlit_App/app.py
   ```

2. **Upload Files for Analysis**


   - **For Job Matching**: Upload your resume (PDF/DOCX) and job description (TXT/JSON) files.
   - **For Video Analysis**: Upload your interview video (MP4, MPEG4).

3. **Analyze Content**

   - For job matching, simply click the 'Match' button and wait for the result.
   - For video analysis, upload your video and wait for the summarized output.

## How to Use the Project

### Using Job Matching System
1. Upload your resume (in PDF/DOCX format) and job description (in TXT/JSON format).
2. Click the Match button to start the alignment analysis.
3. View the results to understand how well the resume aligns with the job description.

### Using Video Analyzer
1. Upload the interview video file (MP4, MPEG4 formats are supported).
2. Wait for the tool to generate a summary and analysis of the interview content.

```