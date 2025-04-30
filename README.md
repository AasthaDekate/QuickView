# QuickView

QuickView is a Flask web application that allows users to input a YouTube video URL and get a summarized version of the video's transcript. It leverages the YouTube Transcript API to fetch video transcripts and uses a pre-trained BART model from Hugging Face Transformers to generate concise summaries.

## Features

- Input any valid YouTube video URL
- Automatically extract the video transcript
- Summarize long transcripts in manageable chunks
- Display the summarized text on the web page
- Simple and clean user interface

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. Create and activate a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. Install the required dependencies:
   ```bash
   pip install flask transformers sentence-transformers youtube-transcript-api
   ```

## Usage

1. Run the Flask application:
   ```bash
   python app.py
   ```

2. Open your web browser and navigate to:
   ```
   http://127.0.0.1:5000/
   ```

3. Enter a YouTube video URL in the input box and click "Summarize".

4. View the summarized transcript on the page.

## Project Structure

```
.
├── app.py                  # Main Flask application
├── templates/
│   └── index.html          # HTML template for the web interface
├── static/
│   └── back.jpg            # Background image for the web page
└── README.md               # Project documentation
```

## Dependencies

- Flask
- transformers
- sentence-transformers
- youtube-transcript-api

## Future Scope

- Enhance the summarization model to support multiple languages.
- Add user authentication to save and manage summaries.
- Integrate with other video platforms beyond YouTube.
- Improve UI/UX with more interactive features.
- Deploy the application on cloud platforms for wider accessibility.
