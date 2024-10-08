GoogleTTS

GoogleTTS is a Python-based project that utilizes Google Cloud's Text-to-Speech API to convert text into speech. This project allows users to input text and generate audio files with customizable voice options.

Features:
- Convert text to speech using Google Cloud Text-to-Speech API
- Choose from a variety of available languages and voices
- Generate MP3 audio files from input text
- List available voices for each supported language

Prerequisites:
Before you begin, ensure you have met the following requirements:
- Python 3.7 or higher
- A Google Cloud Platform account with Text-to-Speech API enabled
- Google Cloud credentials (JSON key file)

Installation:
1. Clone this repository:
   git clone https://github.com/yourusername/GoogleTTS.git
   cd GoogleTTS

2. Create a virtual environment and activate it:
   python -m venv tts_env
   source tts_env/bin/activate  # On Windows, use `tts_env\Scripts\activate`

3. Install the required packages:
   pip install google-cloud-texttospeech

4. Place your Google Cloud credentials JSON file in the project directory and name it `credentials.json`.

Usage:
1. Prepare your input text in a file named `input.txt` in the project directory.

2. Run the script:
   python text_to_speech.py

3. Follow the prompts to select your desired language and voice.

4. The script will generate an `output.mp3` file containing the synthesized speech.

Code Structure:
The main functionality is implemented in the `text_to_speech.py` file.

Key functions:
- text_to_speech: Converts text to speech using the Google Cloud TTS API
- get_available_voices: Retrieves available voices from the API
- choose_language: Allows user to select a language
- choose_voice: Allows user to select a voice for the chosen language
- read_text_file: Reads input text from a file

License:
This project is licensed under the Apache License 2.0. See the LICENSE file for details.

Acknowledgements:
This project uses the Google Cloud Text-to-Speech API. Please refer to Google's documentation for API usage and limitations.