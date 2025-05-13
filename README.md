# StoryToVideo AI

StoryToVideo AI is a web application that allows users to upload written stories and automatically generates narrated videos with text overlays. The final video can be uploaded to YouTube directly via the platform.

## Features

- Upload a story or script
- AI voiceover generation using Text-to-Speech
- Automatic text overlay and video rendering
- Ready for YouTube upload via YouTube Data API

## Technologies Used

- **FastAPI** for backend API
- **MoviePy** for video rendering
- **gTTS** for text-to-speech voiceover
- **FFmpeg** (under the hood) for video processing
- **YouTube API** (planned) for auto-upload

## Getting Started

### Prerequisites

Make sure you have Python 3.8+ installed. Then install dependencies:

```bash
pip install -r backend/requirements.txt
