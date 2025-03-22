# **Termi-Vision – Terminal Audio & Screen Recorder with AI Transcription**

Termi-Vision is a terminal-based application designed for seamless audio and screen recording with AI-driven transcription using Gemini AI. It supports global shortcuts, real-time status notifications, and automatic clipboard integration.

## **Features**

- **Minimalist Terminal UI** – Simple and efficient command-line interface.
- **Global Shortcuts** – Quick access for audio (⇧⌥X) and screen+audio recording (⇧⌥Z).
- **Dual Recording Modes** – Record either audio-only or screen with audio.
- **AI-Powered Transcription** – Automates conversion of recordings into text.
- **Auto Cleanup** – Deletes recordings upon successful transcription.
- **Clipboard Integration** – Automatically copies transcribed text.
- **Live Status Updates** – Real-time notifications for recording and transcription.

## **Setup & Usage**

1. **Clone the Repository & Create Virtual Environment**

   ```bash
   git clone https://github.com/haiderali780/Termi-Vision.git
   cd Termi-Vision
   python -m venv venv
   ```

2. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **For macOS Users:** Install `portaudio` (required for PyAudio)

   ```bash
   brew install portaudio
   ```

4. **Start the Application**
   ```bash
   bash run.sh
   ```
   Or manually activate the environment:
   ```bash
   source activate_env.sh
   python terminal_video_voice_recorder.py
   ```

## **Keyboard Shortcuts**

- **⇧⌥X (Shift+Alt+X)** – Toggle audio-only recording.
- **⇧⌥Z (Shift+Alt+Z)** – Toggle screen+audio recording.
- **Ctrl+C** – Exit the application.

## **Permission Requirements**

- **Accessibility Access** – Required for keyboard shortcuts and text entry.
  - Navigate to **System Settings → Privacy & Security → Accessibility**.
  - Add your terminal application (e.g., Terminal, iTerm2, VS Code).

## **Project Structure**

### **Core Files**

- `terminal_video_voice_recorder.py` – Main application entry point.
- `keyboard_handler.py` – Manages global keyboard shortcuts.
- `terminal_ui.py` – Handles terminal UI components.

### **Recording Components**

- `recorders/recording_handler.py` – Controls recording sessions.
- `recorders/recorder.py` – Core recording functionality.
- `audio_recorder.py` – Audio capture logic.
- `screen_audio_recorder.py` – Screen and audio recording.

### **Transcription Components**

- `transcription_handler.py` – Manages the transcription process.
- `audio_transcription.py` – Handles audio transcription with Gemini AI.
- `video_transcription.py` – Processes video transcriptions.

### **Utilities**

- `type_text.py` – Automatically types transcribed text at the cursor position.

---

For any issues or contributions, feel free to submit a pull request or open an issue.

```

```
