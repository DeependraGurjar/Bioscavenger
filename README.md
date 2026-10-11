# 🌿 BioScavenger

**A screen-free, offline nature quest game. Listen, go outside, explore, and earn Nature Credits.**

Built for Hacktoberfest ("Touch the Grass" theme).

---

## 💡 What is it?

BioScavenger gives you a short scavenger quest as an **audio briefing**. You put your phone away, go outside to find things like leaves, bark, or flowers, then come back and upload a photo as proof.

Everything runs on your own computer. No internet, no accounts, no tracking.

---

## ✨ Features

| | |
|---|---|
| 🔌 **Fully offline** | Runs on a local AI model, with no cloud and no cost |
| 🎧 **Audio quests** | Calm voice narration, hands-free |
| 📸 **Photo proof** | Upload a picture to earn Nature Credits |
| 🔒 **Private** | No telemetry, no location tracking, no data sent anywhere |

---

## 🧰 Built With

| Part | Tool |
|---|---|
| AI model | [Qwen2.5-3B](https://ollama.com/library/qwen2.5) via [Ollama](https://ollama.com) |
| Voice | [Piper TTS](https://github.com/rhasspy/piper) |
| Interface | Streamlit (Python) |
| Data format | JSON, turned into game tasks |

---

## 🚀 Getting Started

### Before you begin
You need:
- [Python 3.10+](https://www.python.org/downloads/)
- [Ollama](https://ollama.com)

### Step 1: Download the project
```bash
git clone https://github.com/<your-username>/BioScavenger.git
cd BioScavenger
```

### Step 2: Install Python packages
```bash
pip install -r requirements.txt
```

### Step 3: Start the AI model
Open a **second terminal** and run:
```bash
ollama run qwen2.5:3b
```

### Step 4: Set up the voice (Windows)
1. Download the Windows release of [Piper TTS](https://github.com/rhasspy/piper).
2. Download the voice files `en_US-lessac-medium.onnx` and its `.json` file.
3. Put `piper.exe` and the voice files in the **main project folder**.

### Step 5: Run the app
```bash
python -m streamlit run app.py
```
Then open **http://localhost:8501** in your browser.

---

## 🎮 How to Play

1. Click **Generate Quest**.
2. Listen to the audio briefing.
3. Put your device away and go outside.
4. Find the items from the quest.
5. Upload a photo as proof.
6. Earn **Nature Credits**. 🌱

---

## 📁 Project Files

```
BioScavenger/
├── app.py            ← main app
├── requirements.txt  ← Python packages
├── piper.exe         ← voice engine (you download this)
└── *.onnx / *.json   ← voice model (you download this)
```

---

## 🤝 Contributing

Contributions are welcome, especially during Hacktoberfest!

1. Fork this repo
2. Create a branch
3. Make your changes
4. Open a pull request

**Ideas:** new quest themes, more voices, Linux/Mac setup instructions.
