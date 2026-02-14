<div align="center">

# 🤖 Auto Reply Bot  
### AI-Powered WhatsApp Web Automation

![Python](https://img.shields.io/badge/Python-3.x-blue)
![OpenAI](https://img.shields.io/badge/OpenAI-GPT-green)
![Automation](https://img.shields.io/badge/Automation-pyautogui-orange)
![Status](https://img.shields.io/badge/Project-Experimental-red)

An intelligent auto-reply bot that reads WhatsApp Web chats  
and responds automatically using OpenAI.

</div>

---

## ✨ Overview

**Auto Reply Bot** is a Python automation tool that:

- 📖 Reads live chat messages from WhatsApp Web  
- 🧠 Analyzes conversation context using GPT  
- 💬 Generates dynamic AI responses  
- ⚡ Sends replies automatically  

It blends **screen automation + prompt engineering + API integration** into one clean pipeline.

---

## 🧠 How It Works

```
WhatsApp Web  →  Screen Selection  →  Clipboard Copy  
       ↓
   Chat History Extraction
       ↓
  OpenAI API (Context + Personality)
       ↓
   Generated Response
       ↓
   Auto Paste + Send
```

The bot continuously checks for new messages and replies only when required.

---

## 📂 Project Structure

```bash
auto-reply-bot/
│
├── bot.py          # Main automation logic
├── openai.py       # OpenAI response testing
├── get_cursor.py   # Utility for finding screen coordinates
└── README.md
```

---

## 🛠️ Tech Stack

- **Python 3.x**
- `pyautogui` – Screen automation
- `pyperclip` – Clipboard management
- `openai` – AI response generation
- WhatsApp Web (Chrome)

---

## ⚙️ Setup

### 1️⃣ Clone Repository

```bash
git clone https://github.com/SpartanOpJod/Auto-Reply-Bot
cd auto-reply-bot
```

### 2️⃣ Install Dependencies

```bash
pip install pyautogui pyperclip openai
```

### 3️⃣ Add Your OpenAI API Key

Replace this inside `bot.py` and `openai.py`:

```python
client = OpenAI(
    api_key="YOUR_API_KEY_HERE",
)
```

⚠️ Never commit your API key.

---

## 🖱️ Configure Screen Coordinates

Every system has different screen resolution.

Run:

```bash
python get_cursor.py
```

Hover your mouse over:
- Chrome icon
- Chat selection area
- Message input box

Update the coordinates inside `bot.py`.

---

## ▶️ Running the Bot

1. Open WhatsApp Web in Chrome  
2. Open the target chat  
3. Run:

```bash
python bot.py
```

The bot:
- Checks every 5 seconds
- Detects new messages
- Generates AI reply
- Sends automatically

---

## 🎭 Custom Personality

Inside `bot.py`:

```python
{"role": "system", "content": "You are Naruto... roast people in a funny way"}
```

Modify this to create:
- Professional assistant
- Motivational friend
- Sarcastic AI
- Study partner
- Meme generator

This is where prompt engineering shines.

---

## ⚠️ Limitations

- Depends on screen coordinates
- Breaks if UI layout changes
- Not using official WhatsApp API
- Requires visible browser window

---

## 🚀 Future Improvements

- Replace screen automation with WhatsApp Business API  
- Add GUI configuration panel  
- Add smarter message detection  
- Convert into background service  
- Docker support  

---

## 🎯 Why This Project Matters

This project demonstrates:

- API integration
- Prompt engineering
- System automation
- Real-world AI usage
- End-to-end workflow design

It’s more than a script — it’s an automation system.

---

<div align="center">

### ⭐ If you like this project, consider starring it!

</div>
