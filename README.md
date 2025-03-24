# VisionVoice AI 

This is an AI-powered chatbot designed to improve communication between patients and doctors by combining speech recognition and image analysis.

## Project Overview

This chatbot helps bridge gaps in healthcare by:

- **Listening & Understanding:**: Uses OpenAI’s Whisper to convert speech into text.

- **Analyzing Medical Images:**: Uses Meta’s Llama 3.2 to interpret images and provide insights.

- **Responding Naturally**: Generating human-like, empathetic responses to patient inquiries.

## Features

- **Speech-to-Text (STT)**:Converts spoken words into text using Whisper.
- **Medical Image Analysis**: Processes images with Llama 3.2 for insights.
- **Text-to-Speech (TTS)**: Replies with natural-sounding speech via gTTS & ElevenLabs.
- **User-Friendly Interface**: Built with Gradio for a smooth experience.

## Getting Started

### Prerequisites

- **Python 3.8+**: Ensure Python is installed on your system.
- **Virtual Environment**: It's recommended to use a virtual environment to manage dependencies.

### Installation

1. **Clone the Repository**:

   ```bash
   git clone git@github.com:jamesoyanna/voice_vision_ai.git
   cd vision_voice_ai
   ```

2. **Set Up Virtual Environment**:

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up Environment Variables**:

   Create a `.env` file in the project root directory with the following content:

   ```bash
   GROQ_API_KEY=your_groq_api_key
   ELEVENLABS_API_KEY=your_elevenlabs_api_key
   ```

5. **Install FFmpeg**:

   - **Windows**: Download from [FFmpeg Official Website](https://ffmpeg.org/download.html) and add to system PATH.
   - **macOS**: Install via Homebrew: `brew install ffmpeg`.
   - **Linux**: Use the package manager: `sudo apt-get install ffmpeg`.

### Running the Application

After completing the installation steps:

```bash
python gradio_app.py
```

Open your browser and navigate to `http://localhost:7860` to interact with the chatbot.


## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- **OpenAI**: For the Whisper model.
- **Meta**: For the Llama 3.2 model.
- **Gradio**: For the user interface framework.

