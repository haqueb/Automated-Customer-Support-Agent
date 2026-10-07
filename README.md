# Automated-Customer-Support-Agent
AI-Powered Conversational Agent for Facebook Messenger, Designed and deployed a fully automated customer support chatbot integrating Facebook Messenger with OpenAI's Large Language Models (LLMs) via Make.com.

# 🤖 AI-Powered Facebook Messenger Chatbot

An intelligent, fully automated conversational agent for Facebook Messenger. This project integrates Meta's Graph API with OpenAI's Large Language Models (ChatGPT) using Make.com to provide instant, context-aware customer support 24/7.

## 🚀 Overview

This repository documents the architecture and setup of a webhook-based automation system that listens to incoming messages on a Facebook Business Page, processes the text using OpenAI, and sends the AI-generated response back to the user seamlessly.

**Key Features:**
- **Instant Auto-Reply:** Zero wait time for customer inquiries.
- **LLM Integration:** Utilizes OpenAI to understand context and generate human-like responses.
- **No-Code/Low-Code Architecture:** Built entirely on Make.com for scalable and easily maintainable workflow automation.
- **Webhook Security:** Verified data transmission using Meta Developer payload tokens.

## 🛠️ Architecture & Workflow

1. **Trigger:** A user sends a message to the Facebook Business Page.
2. **Webhook Event:** Meta Graph API triggers a webhook, sending the message payload to Make.com.
3. **Processing:** Make.com routes the extracted text to the OpenAI API (ChatGPT/Whisper module).
4. **Action:** The generated response from OpenAI is mapped back to the Facebook Messenger module in Make.com and sent directly to the user's inbox.

*(Note: Upload your architecture diagram image here and update the path)*
`![Architecture Diagram](path/to/your/diagram.png)`

## ⚙️ Prerequisites

To deploy this automation, you will need:
- A Facebook Business Page.
- A Meta for Developers account with a configured Business App (Messenger API enabled).
- An active [Make.com](https://www.make.com/) account.
- An OpenAI API Key with available credits.

## 📥 Installation & Setup

### 1. Import the Blueprint
- Download the `messenger_ai_bot_blueprint.json` file from this repository.
- Go to Make.com, create a new scenario, click on the **More** (three dots) menu, and select **Import Blueprint**.
- Upload the `.json` file to instantly load the workflow structure.

### 2. Configure Meta Webhooks
- Go to [Meta for Developers](https://developers.facebook.com/apps/).
- Under **Messenger > Messenger API Settings**, add your callback URL (provided by the first Make.com module) and verify the token.
- Generate a Page Access Token and subscribe the webhook to `messages` and `messaging_postbacks`.

### 3. Connect OpenAI
- Open the OpenAI module in Make.com and establish a connection using your OpenAI API key.
- Customize the system prompt to define the persona and rules for your AI assistant.

### 4. Finalize & Activate
- Map the output `Result` from the OpenAI module to the `Text` field in the final Facebook Messenger module.
- Run a test to verify the data flow, then toggle the scenario to **Active**.

## 🎥 Live Demonstration

*(Note: Upload a GIF demonstrating the chatbot in action and update the path)*
`![Demo](path/to/your/demo.gif)`

## 👨‍💻 Author

**[Md Badeul Haq ]**
- LinkedIn: [[Link to your LinkedIn Profile]](https://bd.linkedin.com/in/haqueb)

