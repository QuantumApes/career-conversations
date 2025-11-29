# 🚀 Career Conversations — Personal Digital Twin  
**AI-powered interactive career assistant that recruiters can chat with.**  
This project creates a **digital twin** of me that recruiters and hiring managers can interact with directly.  
It dynamically incorporates my **latest résumé, LinkedIn PDF, experience summaries, and ongoing updates**—all synced automatically through GitHub → Hugging Face CI/CD.

---

## 🎯 Purpose  
Recruiters often want to understand a candidate quickly without scheduling a call.  
This app allows them to:

- Ask me questions about my experience  
- Explore my background interactively  
- Get customized insights about my roles, achievements, and projects  
- Understand how I think, communicate, and solve problems  
- Explore my résumé in a conversational format  

It’s like having a **24/7 AI version of me** available for Q&A.

---

## 🧠 How It Works  
This project builds and deploys an AI “digital twin” using:

- **Gradio** → interactive chat interface  
- **OpenAI API** → LLM-powered conversation engine  
- **Hugging Face Spaces** → publicly accessible web app  
- **GitHub Actions** → automatic deployment pipeline  
- **Résumé + Summary Files** → dynamic background knowledge  

Whenever I update my résumé, add new internships, or change my summary,  
the digital twin updates automatically.

---

## 🔄 Automatic Sync Pipeline  
This repo contains a GitHub Action that syncs:

- `app.py` (the full application logic)  
- `requirements.txt`  
- `/me` folder (resume PDF, summary text, etc.)  

…into my Hugging Face Space:

➡️ **https://huggingface.co/spaces/Quantumplayer/career_conversations**

Every time I push to `main`, Hugging Face rebuilds and deploys the latest version.

No manual uploads.  
No outdated info.  

---

## 📁 Project Structure

```
career-conversations/
│
├── app.py                # Digital Twin chatbot + app logic
├── requirements.txt      # Python dependencies
│
├── me/
│   ├── linkedin.pdf      # My latest résumé (auto-synced)
│   ├── summary.txt       # My updated summary / bio
│
├── .github/workflows/
│       └── hf-sync.yml   # CI/CD pipeline → Hugging Face
│
└── README.md             # (You are here)
```

---

## 💡 Features  
### ✅ AI Digital Twin  
Answers recruiter questions about my background using LLM reasoning.

### ✅ Résumé-Aware  
Reads my LinkedIn PDF and summary files to give accurate, grounded answers.

### ✅ Interactive Chat Interface  
Built using Gradio’s clean, modern ChatInterface.

### ✅ Fully Automated Deployment  
GitHub → Hugging Face syncing ensures the app is always up to date.

### ✅ Secure API Key Handling  
Uses environment variables and HF Secrets (no exposed keys).

---

## 🛠️ Tech Stack  
| Component | Technology |
|----------|------------|
| UI | Gradio ChatInterface |
| LLM | OpenAI API |
| Hosting | Hugging Face Spaces |
| Automation | GitHub Actions |
| Data | Résumé / LinkedIn export + summary.txt |

---

## 🔐 Secrets & Security  
This project uses Hugging Face Space Secrets to store:

- `OPENAI_API_KEY`

No secrets are stored in the repo.

---

## 📬 For Recruiters  
If you're a recruiter exploring this repository—welcome!  
The live demo below lets you chat with an AI-powered version of me:

👉 **https://huggingface.co/spaces/Quantumplayer/career_conversations**

Feel free to ask about:

- My technical skills  
- My most recent project  
- My resume highlights  
- My internships  
- Why I'm a fit for your role  
- Any specific competency questions  

The AI is grounded in my real experience.

---

## 🧩 Future Improvements  
- Add vector search over all past projects  
- Add voice-enabled conversation  
- Add interactive portfolio cards  
- Add analytics for common recruiter questions

---

## 🤝 Contributions  
This is a personal showcase project, but feedback or suggestions are always welcome.

---

## ⭐ If you like this project  
Give the repo a star! It helps others discover this work and supports the project’s visibility.
