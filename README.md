## What it does

  - Collects leads from two channels: **Telegram bot** and **Google Forms**
  - Normalizes data from both sources into a unified format
  - Uses **AI to qualify leads** and assign a temperature score (hot / warm / cold)
  - Saves all leads to **Google Sheets CRM** with score and reason
  - Instantly notifies the manager in **Telegram** when a hot lead comes in

  ## Tech stack

  - n8n (workflow automation)
  - OpenAI GPT (lead qualification)
  - Google Forms + Google Sheets (data collection and CRM)
  - Telegram Bot API (notifications and lead intake)

  ## How it works

  1. Lead submits a form or sends a message to the Telegram bot
  2. AI parser extracts structured data (name, phone, budget, urgency)
  3. AI qualifier evaluates the lead and assigns hot / warm / cold
  4. Hot leads trigger an immediate Telegram notification to the manager
  5. All leads are saved to Google Sheets with full details and score

  ## Setup

  1. Import the workflow JSON into your n8n instance
  2. Set up credentials: Telegram Bot, OpenAI, Google Sheets, Google Forms
  3. Replace `YOUR_TELEGRAM_CHAT_ID` with your manager's Telegram chat ID
  4. Activate the workflow
