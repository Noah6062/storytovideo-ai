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
```

### Running the Server

```bash
cd backend
uvicorn main:app --reload
```

The API will be available at: `http://localhost:8000`

### Example API Usage

Send a POST request to `/generate-video/` with `story` as form data.

Or test directly via the interactive Swagger UI:

```
http://localhost:8000/docs
```

### Output

The generated `.mp4` file will be downloadable after the API processes the story.

## TODO

- [ ] Integrate ElevenLabs for high-quality voice
- [ ] Add AI video or image generation for scenes
- [ ] Connect to YouTube API for auto-upload
- [ ] Build frontend UI

## License

MIT License

## Author

Built by Noah Anderson
