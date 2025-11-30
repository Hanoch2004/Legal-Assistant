# Legal-Assistant ⚖️

A multi-purpose web application providing legal assistance via a chatbot, virtual-lawyer style interface — aiming to let users easily access government-law information, understand charges/punishments/acts, and get legal clarity without confusion.

## 🚀 Why this project

Many people find it difficult to understand legal jargon, act sections and implications. Legal-Assistant is built to:

- Provide instant legal awareness and clarity.  
- Extract and summarize relevant legal information (charges, punishments, corresponding legal acts/sections) from publicly available sources.  
- Offer a user-friendly interface (chatbot + web UI) so that even non-lawyers can navigate legal content easily.  
- Serve as a foundation for further customizing/adapting for state-specific laws or domain-specific legal assistance (e.g. labour laws, traffic rules, etc.)

## 🧰 Built With / Tech Stack

- **Python** — backend logic, scrapers & LLM integration  
- **FastAPI** — for building web API / backend server  
- **Vector store** (e.g. Chroma) — for storing and retrieving document embeddings (legal documents / acts)  
- **Scraper modules** — to fetch and parse legal information from websites (e.g. public legal-info sites)  
- **Frontend Web UI (HTML / CSS / JS)** — for user interaction (chat interface / website)  
- **SQLite** — for chat-history / session storage (optional, for persistence)  

_(You can mention exact versions here if you want — helpful for future reproducibility.)_

## 📂 Project Structure (at a glance)

/ # root directory
main.py # entry-point (or FastAPI server starter)
ollama_client.py # wrapper for LLM calls (if applicable)
scraper.py # modules/functions to scrape legal-info websites
prompt_builder.py # build and format prompts for LLM or logic
templates/ # HTML/CSS/JS templates for web UI
static/ # (optional) static assets like CSS, images
chat_history/ # (or database) for storing past user chats (if enabled)
README.md # this file
LICENSE # (if you want to open-source under a license)

bash
Copy code

*(Actual structure may vary — adapt accordingly.)*

## 💡 Features & What It Does

- Interactive chatbot interface: users ask legal questions in natural language.  
- Automatic legal-info retrieval: scrapes, parses and extracts relevant legal acts/sections.  
- Clear output: identifies charges, punishments, sections/acts relevant — avoids vague legalese for user readability.  
- Clean code structure: modular design (scraper, prompt builder, LLM wrapper, API layer) — easy to extend or plug-in additional modules (e.g. for state-specific laws).  
- (Future-ready) Ability to log chat history and support multiple user sessions.  

## 🛠️ Getting Started / How to Run Locally

### Prerequisites

- Python 3.x installed  
- (Optional) Virtual environment for isolation  
- Internet access (for scraping / API calls)  

### Setup

```bash
# 1. Clone the repo  
git clone https://github.com/Hanoch2004/Legal-Assistant.git  
cd Legal-Assistant

# 2. (Optional) create and activate venv  
python3 -m venv venv  
source venv/bin/activate   # On Windows: venv\\Scripts\\activate

# 3. Install dependencies (if you have a requirements.txt)  
pip install -r requirements.txt

# 4. Run the application  
python main.py   # or `uvicorn main:app --reload` if using FastAPI  
Usage
Open the web UI (probably at http://localhost:8000/ or configured port)

Ask legal-questions in natural language — e.g. “What punishment does Section X describe?”, “I was arrested under XYZ — what are my rights?”, etc.

The chatbot will respond by extracting relevant legal sections/acts and summarizing charges/punishments.

(Add screenshots or example interactions if available — this helps new users understand your app quickly.)

🤝 Contributing
Contributions, feature requests, bug-reports are welcome!
If you wish to contribute:

Fork the project

Create a new branch — e.g. feature/new-scraper or bugfix/…

Make your changes, test thoroughly

Submit a Pull Request — please describe what you changed / added in the PR description

You can also open an issue if you want to discuss a larger change or feature beforehand.

📄 License
Specify your license here (for example, MIT, GPL-3.0, or any other you choose).
If you don’t want to open-source it now, you can leave as “All rights reserved (private use)”.

🎯 Future Roadmap / Ideas
Add support for more legal domains (e.g. traffic laws, labour laws, family laws, cyber-laws)

Improve scraper/parser robustness to handle multiple legal-info websites and different formats

Add authentication / user accounts & history tracking

Build more friendly UI — with PDF output, download options, or shareable legal summaries

Add multilingual support (e.g. English + regional Indian languages)

🧑‍💻 Authors / Team
D. Hanoch Raj (22241A05U0)

K. Nishanth (22241A05V1)

Ratan (22241A05V1)

K. Koushik (22241A05U7)

(Add links to GitHub profiles if you like)

Thank you for checking out Legal-Assistant!
If you use or extend it — feel free to reach out or contribute.

pgsql
Copy code

---

### ✅ Why this structure works (based on best practices)

- It starts with a **clear overview**: what the project does and why. :contentReference[oaicite:4]{index=4}  
- It describes **how to run / install** so that others (or future you) can quickly get started. :contentReference[oaicite:5]{index=5}  
- It shows **features and usage**, which helps potential users understand the value. :contentReference[oaicite:6]{index=6}  
- It defines how **others can contribute**, which is useful if you plan to make it open-source or collaborate. :contentReference[oaicite:7]{index=7}  
- It includes **license / credit / authorship** to clarify usage, ownership and give you due credit. :contentReference[oaicite:8]{index=8}  

---

If you like — I can **generate a complete README.md** for your repo with this content (with Markdown formatting), which you can copy directly.  
Do you want me to prepare that now?
::contentReference[oaicite:9]{index=9}
