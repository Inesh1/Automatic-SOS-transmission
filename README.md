# GenAI-powered passive distress detection system with intelligent emergency intent recognition and automatic SOS transmission

An AI-powered real-time emergency detection system that analyzes **voice, environmental sounds, motion, and contextual intent** to detect distress situations with high accuracy while minimizing false positives.

---

# 📌 Overview

Traditional emergency systems rely on **manual triggers or simple keyword detection**, which often fail in real-world scenarios.

This project introduces a **multi-signal fusion approach**, combining:

- 🎭 Emotion from voice  
- 🔊 Environmental sounds  
- 📱 Motion signals (simulated)  
- 🧠 Context-aware language understanding  

The system only triggers alerts when **multiple signals confirm danger**, making it **reliable, fast, and privacy-aware**.

---

# 🧠 Core Idea

# 🏗️ Architecture

## 🔁 Pipeline Flow
🎤 Audio Input
    ↓
Audio Preprocessing
    ↓
Parallel Detection:
    • Emotion Detection
    • Sound Event Detection
    • Motion Detection
    ↓
Fusion Engine (Risk Scoring)
    ↓
IF High Risk:
    → ASR (Speech to Text)
    → Keyword Engine (Intent Detection)
    → Evidence Recording
    → Emergency Alert


---

# 🤖 System Components (Agents)

## 🎭 Emotion Agent
- **Model:** Wav2Vec2  
- **Detects:**
  - Fear  
  - Panic  
  - Anger  

---

## 🔊 Sound Agent
- **Model:** AudioSet (AST)  
- **Detects:**
  - Screams  
  - Crashes  
  - Explosions  

---

## 📱 Motion Agent
- Simulated in prototype  
- Future: Phone accelerometer  

- **Detects:**
  - Sudden impact  
  - Abnormal movement  

---

## 🧠 Fusion Engine (Core Logic)
- Combines all signals  
- Assigns weighted risk score  
- Decides whether to trigger further analysis  

---

## 🎙️ ASR Agent
- **Model:** Whisper  
- Converts speech → text  
- Runs only when risk is high (optimized)  

---

## 🔑 Keyword Engine
- Context-aware scoring system  

- **Differentiates:**
  - “help me” → emergency  
  - “help me with homework” → safe  

---

## 📂 Evidence Module
- Records audio during emergencies  

- **Stores:**
  - Pre-buffer audio  
  - Post-trigger audio  

---

## 🌐 UI Layer
- Built using Gradio  

- **Provides:**
  - Live microphone input  
  - Detection output  
  - Evidence download  

---

# ⚙️ Tech Stack

- Python  
- Hugging Face Transformers  
- OpenAI Whisper  
- Librosa  
- Soundfile  
- NumPy  
- Gradio  
