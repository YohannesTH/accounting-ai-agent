# 🧾 Accounting AI Agent — n8n + Google Gemini + Telegram

An intelligent **AI-powered accounting assistant** built using **n8n**, **Google Gemini**, and **Telegram**.  
This automation streamlines bookkeeping by processing **audio, image, and document inputs**, analyzing their content with **AI agents**, and logging extracted accounting data directly into **Google Sheets**.

---

## 🚀 Features

- 🤖 **AI-Powered Workflow** — Integrates Google Gemini for intelligent text, image, and document analysis.  
- 📱 **Telegram Integration** — Users send audio, images, or documents directly to a Telegram bot.  
- 🔊 **Audio Transcription** — Automatically transcribes voice messages into text.  
- 🧾 **Invoice & Document Analysis** — Extracts key financial details such as dates, amounts, and descriptions.  
- 📊 **Google Sheets Logging** — Automatically appends processed data into structured spreadsheets.  
- ⚙️ **Fully Automated with n8n** — Zero manual intervention once set up.  
- 💬 **Instant Responses** — Returns results or confirmations directly in Telegram.

---

## 🧠 Workflow Overview

1. **Telegram Trigger:** Listens for new messages (audio, image, or document).  
2. **Switch Node:** Routes input based on type.  
3. **Processing Path:**
   - Audio → Download → Transcribe → AI Agent → Append to Google Sheets  
   - Image → Download → Analyze Image → AI Agent → Append to Google Sheets  
   - Document → Download → Analyze Document → AI Agent → Append to Google Sheets
   - Text → AI Agent → Append to Google Sheets   
4. **Response:** Sends confirmation or summary message back via Telegram.

---

## 🧩 Tech Stack

| Category | Tools |
|-----------|--------|
| Automation | [n8n](https://n8n.io/) |
| AI Models | Google Gemini / OpenAI API |
| Messaging | Telegram Bot API |
| Storage | Google Sheets |
| Logic | JavaScript (Custom Code Nodes) |

---

## ⚙️ Setup Instructions

1. **Clone this repo**
   ```bash
   git clone https://github.com/yourusername/accounting-ai-agent.git
   cd accounting-ai-agent

2. **Set up n8n**
   - Install n8n locally or use [n8n Cloud](https://n8n.io).  
   - Import the workflow JSON file (if provided).  

3. **Create environment variables**
   ```bash
   TELEGRAM_API_TOKEN=your_telegram_bot_token
   GOOGLE_API_CREDENTIALS=your_google_credentials.json
   GEMINI_API_KEY=your_gemini_api_key
4. **Connect integrations**
   - Link your Telegram bot to n8n.  
   - Configure Google Sheets API credentials.  
   - Add your Gemini API key for AI processing.  

5. **Run the workflow**
   - Execute the workflow in n8n.  
   - Send an audio, image, or document to your Telegram bot.  
   - Processed data will appear automatically in Google Sheets.
