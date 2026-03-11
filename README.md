# Babel Fish — Voice Translation Assistant with Watsonx

## Introduction

This project is a voice translation assistant built using **Watsonx** and **IBM Watson Speech Libraries for Embed**. Inspired by the fictional Babel Fish from Douglas Adams' *The Hitchhiker's Guide to the Galaxy*, the assistant takes voice input, converts it to text, sends it to an LLM for translation, and plays back the response as speech.

The app features a responsive frontend built with HTML, CSS, and JavaScript, and a reliable backend powered by Python and Flask.

Try the [demo app](https://ai-personal-assistant.xs6r134s1i6.us-east.codeengine.appdomain.cloud/) to see the final application in action.

---

## Features

- 🎙️ **Speech-to-Text** — converts voice input to text using IBM Watson STT
- 🤖 **LLM Translation** — processes and translates text using Watsonx's `mistralai/mistral-medium-2505`
- 🔊 **Text-to-Speech** — converts translated text back to audio using IBM Watson TTS
- 🌐 **Web Interface** — responsive UI with light/dark mode support

---

## Tech Stack

- **Backend:** Python, Flask
- **Frontend:** HTML, CSS, JavaScript, Bootstrap, Font Awesome, jQuery
- **AI/ML:** IBM Watsonx, IBM Watson Speech Libraries for Embed

---

## UI Preview

### Light Mode
> The base interface before the assistant is fully configured — returns `null` as a response.

![Light Mode UI](assets/ui-light-mode.png)

### Dark Mode
> The completed assistant giving clear translation responses.

![Dark Mode UI](assets/ui-dark-mode.png)

---

## Setup & Installation

### 1. Clone the repository
```bash
git clone https://github.com/ibm-developer-skills-network/translator-with-voice-and-watsonx
cd translator-with-voice-and-watsonx
```

### 2. Create and activate a virtual environment
```bash
python3.11 -m venv my_env
source my_env/bin/activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```
> This may take 5–10 minutes.

### 4. Run the server
```bash
python3 server.py
```

---

## Project Structure

| File | Description |
|---|---|
| `server.py` | Flask backend — handles routing and API requests |
| `worker.py` | Core logic — speech-to-text, text-to-speech, Watsonx integration |
| `templates/index.html` | Frontend layout and structure |
| `static/style.css` | Custom styling and loading animations |
| `static/script.js` | Frontend interactivity — voice recording, messaging, light/dark mode |

---

## Learning Objectives

By completing this project, you will be able to:

- Explain the basics of voice assistants and their applications
- Set up a Python/Flask development environment
- Implement speech-to-text functionality for voice input
- Integrate with Watsonx LLM for intelligent translation
- Implement text-to-speech for voice output
- Build and deploy a full-stack AI-powered web application

---

## API Keys

This project uses IBM Watsonx and IBM Watson Speech Services. See [DEV_NOTES.md](DEV_NOTES.md) for instructions on setting up API keys and switching to a HuggingFace backend if needed.
