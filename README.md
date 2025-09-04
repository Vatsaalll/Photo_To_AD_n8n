# AI Ad Creator - Telegram Bot Workflow



This n8n workflow automates the creation of professional ad videos from simple product photos using AI. Just send a photo of any product to your Telegram bot with a creative brief, and receive a complete AI-generated ad video within minutes.

## 🚀 Key Features

- **Zero-Code Implementation**: Build a complete AI ad creation system without programming knowledge
- **Telegram Integration**: Trigger the workflow by simply sending a photo to your Telegram bot
- **AI-Powered Creative Generation**: Uses GPT-4o for image analysis and prompt engineering + Google VEO3 for video generation
- **Human-in-the-Loop Approval**: Review and approve/reject AI-generated prompts before video creation
- **Cost-Effective Production**: Creates professional ad videos for ~$0.40 each (90%+ profit margins)
- **Multi-Platform Output**: Final videos delivered directly to Telegram (easily extendable to other platforms)

## 💰 Business Value

This workflow transforms how creative agencies operate:
- Reduces ad production costs from hundreds to less than $1 per video
- Cuts production time from hours to minutes
- Enables solo creators to operate as "one-person creative agencies"
- Creates 90-99% gross margins on ad creation services
- Scales content production without additional staff

## ⚙️ Technical Architecture

![Workflow Architecture](architecture.png)

The workflow consists of three main sections:

1. **Input Section**
   - Telegram trigger to receive product photos and creative briefs
   - Image analysis using GPT-4o to understand product details

2. **AI Creative Factory**
   - Dual AI agent system for prompt engineering
   - GPT-4o Image model for scene generation
   - Google VEO3 for video creation
   - Human approval step before final generation

3. **Output Delivery**
   - Telegram integration for final video delivery
   - (Easily extendable to Instagram, Dropbox, etc.)

## 🛠️ Requirements

- [n8n](https://n8n.io/) account (free tier available)
- [Telegram Bot](https://core.telegram.org/bots#6-botfather) 
- [OpenAI API](https://platform.openai.com/) account
- [Key.AI](https://keyai.com/) account (for VEO3 access)

## 📦 Setup Instructions

1. **Create Required Accounts**
   - Set up Telegram Bot via BotFather
   - Create OpenAI API key
   - Sign up for Key.AI and add credits

2. **Configure n8n Credentials**
   ```plaintext
   Telegram Bot Token → n8n Telegram API credential
   OpenAI API Key → n8n OpenAI API credential
   Key.AI API Key → n8n Header Auth credential (Authorization: Bearer YOUR_KEY)
