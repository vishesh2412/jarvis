# Jarvis - A Voice Assistant in Python

Jarvis is a simple AI-powered voice assistant built with Python. It listens to your voice commands and performs tasks such as searching Wikipedia, opening websites, playing music, and sending emails.

## Features

- **Voice-Based Interaction** - Uses speech recognition and text-to-speech.
- **Wikipedia Search** - Fetches summaries from Wikipedia.
- **Web Navigation** - Opens Google, YouTube, and Stack Overflow.
- **Music Playback** - Plays music from a specified directory.
- **Time Retrieval** - Tells the current time.
- **Application Launching** - Opens VS Code or other apps.
- **Email Sending** - Sends emails via Gmail.
- **Exit Command** - Ends execution when "exit" is spoken.

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/jarvis.git
   ```
2. Install dependencies:
   ```sh
   pip install pyttsx3 speechRecognition wikipedia
   ```
3. Run the script:
   ```sh
   python jarvis.py
   ```

## Configuration

### **1. Updating File Paths**
- Modify `music_dir` in `play music` to your actual music folder.
- Update `codePath` if VS Code is installed at a different location.

### **2. Secure Email Credentials**
The current script contains hardcoded credentials, which is insecure. **Do not use your real password directly in the script.** Instead:

- Store credentials in environment variables:
  ```python
  import os
  email_user = os.getenv("EMAIL_USER")
  email_pass = os.getenv("EMAIL_PASS")
  ```
- Use an App Password for Gmail instead of your real password.

## Usage

1. Run the script.
2. Speak your command when prompted.
3. Jarvis will execute the requested task.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
This project is open-source and available under the MIT License.

