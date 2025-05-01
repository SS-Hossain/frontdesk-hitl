# 🧠 Frontdesk HITL AI Supervisor

A simple, modular Flask-based simulation of a human-in-the-loop (HITL) AI receptionist system.

This project was built as part of Frontdesk's engineering assessment and demonstrates how an AI receptionist can escalate unknown questions to a human supervisor, follow up with customers, and update its internal knowledge base.

---

## 🚀 Features

- 📞 Simulated AI agent that receives questions via `/call`
- 🤖 Answers known questions from a local knowledge base
- ❓ Escalates unknown questions by creating a help request
- 🧑 Supervisor Panel (admin UI) to:
  - View and resolve help requests
  - Mark unanswered ones as unresolved after 10 mins
- 💾 Automatically learns new Q&As from supervisor input
- 📚 Viewable Knowledge Base section
- ✅ Clean request lifecycle: `Pending → Resolved / Unresolved`

---

## 🧰 Tech Stack

- Python 3
- Flask
- HTML + Bootstrap 5
- JSON (as a lightweight DB)
- Postman (to simulate customer calls)

---

## 🛠️ Setup Instructions

1. **Clone the repo**  
   ```bash
   git clone https://github.com/yourusername/frontdesk-hitl.git
   cd frontdesk-hitl
   
## Set up virtual environment
    ```python -m venv venv
       venv\Scripts\activate  # (Windows) or source venv/bin/activate (Linux/macOS)
       pip install flask
