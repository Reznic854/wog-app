# Whisper Translate API

A simple Express.js API that uses OpenAI Whisper for speech transcription and GPT-4 for translation.

## How to use

1. Install dependencies  
   ```bash
   npm install
   ```

2. Create a `.env` file and add your OpenAI key:
   ```
   OPENAI_API_KEY=sk-xxxxxx
   ```

3. Start the server  
   ```bash
   node index.js
   ```

API will run at `http://localhost:3000/translate`

Use `POST /translate` with form-data:
- `file`: your `.webm` audio
- `inputLang`: source language (e.g. `en`)
- `outputLang`: target language (e.g. `hr`)
