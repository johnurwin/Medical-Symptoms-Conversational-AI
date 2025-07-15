# Medical-Symptoms-Conversational-AI

An AI-powered conversational assistant designed to collect user symptoms, suggest possible conditions, and provide basic healthcare advice using retrieval-augmented generation (RAG) and slot-filling.

---

## 🛠 Stack
- **LangChain** for flow and LLM integration
- **OpenAI GPT-4o** (or Claude/Gemini)
- **Chroma** for vector search
- **FastAPI**
- **Regex + API mocks** for intent and data lookups

---

---

## 🧠 Core Features
- Intent detection (symptom, appointment, fallback)
- Retrieval-Augmented Generation using embedded docs
- Symptom slot-filling and mock condition lookup
- Modular chatbot logic, easily extendable
- Optional backend (FastAPI or Flask)

---

## 📁 Project Structure
```
symptom-checker-bot/
├── app.py                # Entry point (CLI or API)
├── chatbot.py            # Conversational flow logic
├── intents.py            # Intent recognition (regex-based)
├── retrieval.py          # Chroma + embedding setup
├── api_integration.py    # Symptom-to-condition mock API
├── memory.py             # Optional memory management
├── data/
│   └── knowledge_base/   # Text files for vector search
├── tests/
│   └── test_flows.py     # Unit and functional tests
└── requirements.txt
```

---

## ✅ TODO / Improvements
- Add frontend (Streamlit or React)
- Support multilingual input
- Integrate real medical APIs (e.g. Infermedica, HealthTap)
- Expand entity recognition and dialogue tree depth

---

## 🧪 Example Prompt
```
User: I’ve had a fever and sore throat for 2 days
Bot: That sounds uncomfortable. Based on your symptoms, possible conditions include the flu or a throat infection. Stay hydrated and monitor your temperature. Would you like to schedule a virtual consult?
