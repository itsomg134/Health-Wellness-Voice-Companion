# Health-Wellness-Voice-Companion


<div align="center">

![Version](https://img.shields.io/badge/Version-1.0.0-blue)
![Python](https://img.shields.io/badge/Python-3.11-yellow?logo=python)
![TypeScript](https://img.shields.io/badge/TypeScript-5.0-3178C6?logo=typescript)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-F7DF1E?logo=javascript)
![Shell](https://img.shields.io/badge/Shell-Bash-121011?logo=gnu-bash)
![Dockerfile](https://img.shields.io/badge/Dockerfile-Ready-0db7ed?logo=docker)
![License](https://img.shields.io/badge/License-MIT-green)

**A friendly AI Barista that takes your drink order through real-time voice interaction.
Built for the #MurfAIALAgentsChallenge.**

[Features](#-features) • [Project-Structure](#️-project-structure) • [Quick-Start](#-quick-start) • [Demo-Video](#-demo-video) • [Author](#-author)

</div>


# 🧘‍♂️ Health & Wellness Voice Companion

*A simple, supportive daily voice agent that checks in on your mood, energy, and goals — and remembers your progress over time.*


## 📌 Overview

This project is a **voice-based wellness companion** designed to support daily reflection.
It conducts short check-ins, listens to your mood and goals, provides grounded suggestions (non-medical), and stores each session in a JSON file so it can reference your previous days.

This agent is **not a clinician** — just a friendly, grounded voice that helps you stay mindful and consistent.

---
## 🎥 Live Demo

Watch the demo video here:
https://drive.google.com/file/d/1PwfpzJZSrQOFcGwoQ0cUO65RnV5F0yfv/view?usp=drive_link
## 🎯 Features

### **✔ Daily Voice Check-ins**

* Asks about mood, energy, stress, and intentions for the day.
* Example prompts:

  * “How are you feeling today?”
  * “What’s your energy like?”
  * “What are 1–3 things you'd like to get done today?”

### **✔ JSON Persistence**

All check-in data is stored in `wellness_log.json` including:

* Date & time
* Mood
* Energy level
* Daily objectives
* Summary sentence

### **✔ Personalized Follow-ups**

On the next session, the agent recalls past data:

* “Last time your energy was low — how is it today?”
* “Yesterday you planned 3 goals. How did they go?”

### **✔ Supportive, Grounded Responses**

* No medical advice
* No diagnosis
* Only small, realistic suggestions such as:

  * “Try breaking your task into smaller steps.”
  * “Maybe take a 5-minute walk to reset.”

---

## 🛠️ Tech Stack

* **Python**
* **SpeechRecognition** (STT)
* **pyttsx3** (TTS)
* **JSON**
* **Datetime**

---

## 📁 Project Structure

```
/Health-Wellness-Voice-Companion
│
├── main.py
├── wellness_log.json
├── requirements.txt
└── README.md
```

---

## 🧩 How It Works

### **1. Start the Companion**

```bash
python main.py
```

### **2. The Agent Will:**

* Speak a greeting
* Ask about mood, energy, stress
* Ask about 1–3 goals
* Provide a small reflection
* Recap your answers
* Save everything in JSON

### **3. Next Day**

It reads previous entries and gives personalized prompts:

```
"Yesterday you mentioned being tired. How is your energy today?"
```

---

## 🧪 Sample JSON Output

```json
[
    {
        "date": "2025-11-23T23:00:00",
        "mood": "tired",
        "energy": "low",
        "objectives": ["walk 10 mins", "finish report"],
        "summary": "User feels tired with low energy and set 2 small goals."
    }
]
```

---

## 🚀 Future Improvements

* Add sentiment analysis
* Dashboard to visualize mood trends
* Daily reminders
* Multi-language support
* Optional text-only mode

---

## 👨‍💻 Author

Om Gedam

GitHub: @itsomg134

Email: omgedam123098@gmail.com

Twitter (X): @omgedam

LinkedIn: Om Gedam

Portfolio: https://ogworks.lovable.app

Made with ❤️ using Python, TypeScript, JavaScript, Shell, and Docker.

