# Sentiment-Analysis
# Speech-to-Text Sentiment Analysis using Whisper and DistilBERT

## Project Overview

This project implements an end-to-end speech processing pipeline that converts audio into text, analyzes the sentiment of the extracted text, and generates an audio response based on the sentiment result.

The system combines OpenAI Whisper for speech recognition, DistilBERT for sentiment analysis, and Google Text-to-Speech (gTTS) for audio generation.

## Features

* Speech-to-Text Conversion using Whisper
* Sentiment Analysis using DistilBERT
* Automatic Text-to-Speech Response Generation
* Supports MP3 and WAV audio files
* Easy deployment on Google Colab
* End-to-End AI Pipeline

## Architecture

```text
Input Audio
     │
     ▼
OpenAI Whisper
(Speech-to-Text)
     │
     ▼
Extracted Text
     │
     ▼
DistilBERT
(Sentiment Analysis)
     │
     ▼
Sentiment Result
(Positive/Negative)
     │
     ▼
Google Text-to-Speech
     │
     ▼
Output Audio File
```

## Technologies Used

* Python
* OpenAI Whisper
* DistilBERT
* Hugging Face Transformers
* PyTorch
* Google Text-to-Speech (gTTS)
* Google Colab

## Installation

Install the required dependencies:

```bash
pip install openai-whisper transformers torch gtts
```

Install FFmpeg:

```bash
apt-get install ffmpeg
```

## Usage

### Step 1: Upload or Record Audio

Provide an audio file in MP3 or WAV format.

### Step 2: Convert Speech to Text

Whisper transcribes the audio and extracts the spoken text.

### Step 3: Perform Sentiment Analysis

DistilBERT analyzes the extracted text and predicts:

* POSITIVE
* NEGATIVE

### Step 4: Generate Audio Response

The sentiment result is converted into speech using gTTS.

## Example

### Input Audio

```text
I am very happy with the service and support.
```

### Transcribed Text

```text
I am very happy with the service and support.
```

### Sentiment Analysis Result

```text
Label: POSITIVE
Confidence: 0.9987
```

### Generated Response

```text
The sentiment of the given audio is POSITIVE. The confidence score is 1.00.
```

### Output

```text
output_audio.mp3
```

## Project Structure

```text
Speech-To-Text-Sentiment-Analysis/
│
├── sample_audio.mp3
├── output_audio.mp3
├── main.py
├── requirements.txt
└── README.md
```

## Applications

* Customer Feedback Analysis
* Voice-Based Review Systems
* Call Center Analytics
* Social Media Monitoring
* Virtual Assistants
* Speech Intelligence Systems

## Future Enhancements

* Real-Time Microphone Input
* Multi-Language Support
* Emotion Detection
* Web Application Deployment
* Dashboard Visualization
* Live Sentiment Monitoring

## Results

The project successfully converts speech into text, classifies the sentiment using DistilBERT, and generates an audio response, demonstrating the integration of speech recognition, natural language processing, and speech synthesis in a single workflow.

## Author

Developed as an AI and Natural Language Processing project using Whisper and DistilBERT.
