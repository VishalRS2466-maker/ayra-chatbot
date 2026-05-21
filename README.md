# 🤖 Ayra — AI Conversational Assistant

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![NLP](https://img.shields.io/badge/NLP-Intent%20Classification-0E7C7B?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active%20Development-brightgreen?style=for-the-badge)
![AI](https://img.shields.io/badge/AI-Conversational%20AI-0A2342?style=for-the-badge)

> **Ayra** is a Python-based AI conversational assistant built with a modular NLP pipeline. Designed to handle multi-turn conversations with intent detection, context tracking, and dynamic response generation — built entirely from scratch as a personal AI learning project.

---

## 🧠 What Is Ayra?

Ayra is a rule-and-ML-hybrid chatbot that demonstrates core conversational AI principles:

- **Intent Classification** — understands what the user is asking, not just what they typed
- **Multi-turn Context Tracking** — remembers conversation history within a session
- **Modular NLP Pipeline** — tokenisation → classification → response generation, each independently testable
- **Clean Architecture** — designed to be extensible with new intents and responses without touching core logic

Built to apply concepts from AI/ML research papers into a real, working system.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🎯 Intent Detection | Classifies user input into predefined intent categories |
| 🔄 Multi-turn Dialogue | Maintains context across multiple conversation turns |
| 🧩 Modular Pipeline | Tokeniser, classifier, and responder are independently swappable |
| ⚡ Lightweight | No heavy frameworks — built to run locally without GPU |
| 🛠️ Extensible | Add new intents and responses via simple config files |

---

## 🏗️ Architecture

```
User Input
    │
    ▼
┌─────────────────┐
│   Tokeniser     │  ← Preprocessing, normalisation, stopword removal
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ Intent Classifier│  ← Pattern matching + ML classification
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ Context Manager │  ← Tracks conversation state across turns
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│Response Generator│  ← Selects and formats the appropriate reply
└─────────────────┘
         │
         ▼
    Ayra's Reply
```

---

## 🚀 Getting Started

### Prerequisites
```bash
Python 3.10+
pip
```

### Installation
```bash
# Clone the repository
git clone https://github.com/VishalRS2466-maker/ayra-chatbot.git
cd ayra-chatbot

# Install dependencies
pip install -r requirements.txt

# Run Ayra
python main.py
```

### Example Conversation
```
You  : Hello!
Ayra : Hi there! I'm Ayra. How can I help you today?

You  : What can you do?
Ayra : I can answer questions, have a conversation, and assist with tasks.
       What would you like to explore?

You  : Tell me something interesting.
Ayra : Did you know? The word "robot" comes from the Czech word "robota",
       meaning forced labour — first used in a 1920 play.
```

---

## 🛠️ Tech Stack

- **Language:** Python 3.10+
- **NLP:** Custom tokenisation pipeline, intent classification
- **Architecture:** Modular, component-based design
- **Storage:** JSON-based intent and response configuration

---

## 📁 Project Structure

```
ayra-chatbot/
│
├── main.py              # Entry point — starts the conversation loop
├── chatbot/
│   ├── tokeniser.py     # Text preprocessing and tokenisation
│   ├── classifier.py    # Intent classification engine
│   ├── context.py       # Conversation state and context manager
│   └── responder.py     # Response selection and generation
├── data/
│   └── intents.json     # Intent definitions and training patterns
├── requirements.txt
└── README.md
```

---

## 🌱 What I Learned Building Ayra

- How to design a **modular NLP pipeline** where each component is independently testable
- How **intent classification** works in practice — the gap between theory (papers) and implementation
- Importance of **context management** in multi-turn dialogue — stateless responses feel broken
- How to structure a Python AI project for **readability and extensibility**

---

## 🗺️ Roadmap

- [ ] Add machine learning-based intent classifier (scikit-learn / TF-IDF)
- [ ] Voice input support via SpeechRecognition library
- [ ] Web interface using Flask
- [ ] Tamil language support (regional NLP)
- [ ] Integration with Mithran rural chatbot for unified assistant platform

---

## 👨‍💻 About the Developer

**Vishal R S** — AI/ML Engineering Student at VSB College of Engineering, Karur.
Building AI projects daily as part of a 1% compounding growth discipline.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin)](https://linkedin.com/in/vishal-r-s-875002390)
[![GitHub](https://img.shields.io/badge/GitHub-Portfolio-181717?style=flat&logo=github)](https://github.com/VishalRS2466-maker)

---

## 📄 License

MIT License — free to use, learn from, and build upon.

---

*Built with curiosity, persistence, and the belief that the best way to learn AI is to build AI.*
