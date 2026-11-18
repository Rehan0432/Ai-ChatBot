# Nova AI — Groq Chatbot (Fixed Ports)

Gemini-inspired light UI chatbot powered by Groq `llama-3.3-70b-versatile`.

## Fixed ports
- Frontend: http://localhost:5188
- Backend: http://localhost:5189

These ports are fixed. Vite will stop with an error if 5174 is already occupied instead of silently switching to another port.

## Setup on Windows

1. Extract this ZIP.
2. Open PowerShell/CMD inside this folder.
3. Install dependencies:

   ```bash
   npm install
   ```

4. Create `.env`:

   PowerShell:
   ```powershell
   Copy-Item .env.example .env
   ```

   CMD:
   ```cmd
   copy .env.example .env
   ```

5. Open `.env` and add your Groq API key:

   ```env
   GROQ_API_KEY=your_actual_groq_api_key
   PORT=5001
   ```

6. Start both frontend and backend:

   ```bash
   npm run dev
   ```

7. Open http://localhost:5188

## Features
- Groq streaming chat using Llama 3.3 70B
- Browser localStorage chat history
- Search conversations by title or message
- Rename and delete chats
- New chat
- Microphone voice-to-text where supported by the browser
- Plus menu with Images / PDF / Videos choices (menu only; upload is not enabled)
- Express backend and try/catch error handling

Keep your `.env` file private. Do not paste your API key into chat or frontend code.


## Fixed ports
- Frontend: http://localhost:5188
- Backend: http://localhost:5189

Copy `.env.example` to `.env` and add your Groq API key. Then run `npm install` and `npm run dev` from this project folder.
