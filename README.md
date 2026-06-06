Speech-to-Indian Sign Language (ISL) Translator
An AI-powered communication accessibility tool that bridges the gap between spoken language and the Deaf and Hard of Hearing (DHH) community in India. This application converts real-time spoken audio into Indian Sign Language (ISL) sign sequences using advanced speech recognition, natural language processing, and a dynamic visual fallback mechanism.

🚀 Features
  1. Real-Time Speech-to-Text: Utilizes OpenAI's Whisper model for highly accurate, robust speech transcription.
  2. Smart Phrase-Level Mapping: Matches full words and common phrases using a custom JSON-based dictionary to ensure natural translation flow.
  3. Intelligent Alphabet Fallback: Automatically reverts to character-by-character fingerspelling for names, rare words, or terms not present in the phrase dictionary.
  4. Dynamic Sign Rendering: Displays corresponding ISL sign images sequentially, simulating a fluid video-like playback experience.
  5. Intuitive Web UI: Built with Gradio for a seamless, interactive, and user-friendly experience directly in the browser.

🔄 System Workflow
The translation pipeline operates in five core stages:
  1. Audio Capture: The user speaks into the microphone via the Gradio interface.
  2. Transcription: OpenAI Whisper processes the audio and outputs accurate text.
  3. NLP Preprocessing: Text is cleaned, normalized, and tokenized.
  4. Dictionary Lookup: The system attempts a phrase-level match. If unavailable, it seamlessly triggers an alphabet-level translation matrix.
  5. Visual Output: The application dynamically streams the correct sequence of ISL images to the user.

🛠️ Tech Stack
Language: Python
Speech Recognition: OpenAI Whisper
User Interface: Gradio
Data Structures: JSON-based Sign Language Mapping
Core Concepts: Natural Language Processing (NLP)
