# Prompt Optimizer API

A simple Node.js + Express backend API to optimize prompts using OpenAI GPT-4. Designed for use with prompt generation tools for AI image creation.

## 🔧 Features

- Accepts prompt input via `/optimize` endpoint (POST).
- Uses OpenAI's GPT-4 model to rewrite and enhance prompts.
- Configurable via `.env` file.
- CORS enabled for frontend access.

## 🚀 How to Deploy on Railway

1. Fork or upload this repository to your own GitHub account.
2. Go to [Railway.app](https://railway.app) and create a new project.
3. Choose **Deploy from GitHub Repo** and select this repo.
4. In the Railway dashboard, go to the **Variables** tab and add:
   - `OPENAI_API_KEY`: your OpenAI API key.

5. Railway will auto-detect and start your backend server.

## 🛠️ Local Development

```bash
git clone https://github.com/your-username/prompt-api.git
cd prompt-api
npm install
touch .env  # Add your API key inside
npm start
```

`.env` file format:
```
OPENAI_API_KEY=your_openai_api_key_here
```

## 📫 API Endpoint

`POST /optimize`

**Request body:**
```json
{
  "prompt": "cinematic, Indonesian man, neon city"
}
```

**Response:**
```json
{
  "optimized": "Cinematic portrait of a light-skinned Indonesian man standing in a neon-lit futuristic city..."
}
```

## 📄 License

MIT

---

**Credit:**  
Developed by [Madeci](https://madeci.web.id)  
