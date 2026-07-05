# AI Video Assistant

An AI-powered assistant for turning videos or audio into structured meeting insights. It can process a YouTube link or local media file, transcribe the content, generate a summary, extract action items, capture key decisions, and support follow-up Q&A over the transcript using a retrieval-augmented generation (RAG) workflow.

## Features

- Upload or provide a YouTube URL or local media file
- Transcribe audio/video using Whisper-style processing
- Generate:
  - Titles
  - Executive summaries
  - Action items
  - Key decisions
  - Open questions
- Chat with the processed content using a retrieval-based assistant
- Modern Streamlit web interface

## Tech Stack

- Python
- Streamlit
- Whisper / speech-to-text processing
- LangChain + Mistral AI
- Chroma vector store
- Sentence-transformers / Hugging Face embeddings

## Project Structure

- app.py — Streamlit UI
- main.py — CLI pipeline runner
- core/ — transcription, summarization, extraction, and RAG logic
- utils/ — audio preprocessing utilities
- test.py — example end-to-end test script

## Setup

1. Clone the repository
2. Create and activate a virtual environment
3. Install dependencies:

```bash
pip install -r Requirements.txt
```

4. Create a .env file using the provided template
5. Run the app:

```bash
streamlit run app.py
```

## Environment Variables

Create a .env file with values such as:

```bash
MISTRAL_API_KEY=your_mistral_api_key
SARVAM_API_KEY=your_sarvam_api_key
WHISPER_MODEL=small
SARVAM_STT_MODEL=saaras:v2.5
```

## Resume-Friendly Project Notes

This project demonstrates:

- End-to-end AI pipeline design
- LLM orchestration and prompt-based workflows
- RAG-based question answering
- Working with speech-to-text and structured output generation
- A complete user-facing application

## Example Usage

You can run the example script with:

```bash
python test.py
```

## What I Learned

Through this project, I learned how to:

- Build an end-to-end AI pipeline using Python
- Integrate speech-to-text, summarization, and extraction workflows
- Use LLMs and retrieval-augmented generation for intelligent question answering
- Connect AI models with a Streamlit-based user interface
- Structure a project in a way that is suitable for GitHub and resume presentation

## Future Scope

Possible improvements for the project include:

- Adding support for multi-language transcription and translation
- Improving the UI with better file upload and result visualization
- Adding user authentication and saved project history
- Integrating with cloud storage or a database
- Expanding the system for meeting analytics, speaker detection, and summaries by topic

## Author
Karthikeyan Jain
