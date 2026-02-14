🤖 Auto Reply Bot (WhatsApp Web Automation)

An AI-powered auto-reply bot that reads chat messages from WhatsApp Web and generates contextual replies using OpenAI.

This bot:

📖 Reads chat messages directly from the screen

🧠 Analyzes conversation history using GPT

💬 Replies automatically in a defined personality

⚡ Runs in real time

🚀 Features

Automated chat reading using pyautogui

Clipboard-based message extraction with pyperclip

AI-generated contextual responses via OpenAI API

Customizable personality (Hindi + English coder roast mode 😏)

Fully automated message sending

🛠️ Tech Stack

Python 3.x

pyautogui

pyperclip

openai

WhatsApp Web (Chrome)

📂 Project Structure
auto-reply-bot/
│
├── bot.py          # Main automation script
├── openai.py       # OpenAI response testing script
├── get_cursor.py   # Utility to get screen coordinates
└── README.md

⚙️ How It Works
1️⃣ Screen Automation

The bot:

Clicks on Chrome

Selects chat area

Copies entire conversation

Checks if the last message is from a specific sender

2️⃣ AI Processing

The conversation history is sent to GPT with:

A defined personality

Response constraints

Context-aware instructions

3️⃣ Auto Reply

If the last message matches the target sender:

The AI generates a response

The bot pastes it into chat

Sends it automatically

🧪 Setup Instructions
Step 1: Clone the Repository
git clone https://github.com/your-username/auto-reply-bot.git
cd auto-reply-bot

Step 2: Install Dependencies
pip install pyautogui pyperclip openai

Step 3: Add Your OpenAI API Key

Replace this in both bot.py and openai.py:

api_key="<Your Key Here>"


⚠️ Never push your API key to GitHub.

🖱️ Configure Screen Coordinates

Every screen resolution is different.

Use:

python get_cursor.py


Move your mouse over:

Chrome icon

Chat selection area

Message input box

Update coordinates inside bot.py.

▶️ Running the Bot

Open WhatsApp Web in Chrome

Open the target chat

Run:

python bot.py


The bot will:

Check every 5 seconds

Detect new messages

Reply automatically

🧠 Customizing Personality

Inside bot.py:

{"role": "system", "content": "You are a person named Naruto... roast people in a funny way"}


Change this prompt to:

Professional assistant

Flirty friend

Motivational coach

Savage roast king

Study buddy

Literally anything.

⚠️ Important Notes

This bot relies on screen coordinates (not official WhatsApp API)

Works only when:

Browser window is visible

Screen resolution matches configured coordinates

Do NOT use for spam

Educational purposes only

📌 Limitations

Breaks if UI layout changes

Hardcoded sender detection

Depends on exact chat format

Not optimized for background execution

🔮 Future Improvements

Use WhatsApp Business API instead of screen automation

Add GUI for configuration

Add message filtering logic

Dockerize the project

Deploy as a background service

🎯 Why This Project Is Cool

Combines automation + AI

Shows real-world API integration

Demonstrates prompt engineering

Practical use of system-level automation

This is not just a script — it’s a proper automation pipeline.
