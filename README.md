# 🎬 AI-Powered Script Writing Assistant for Content Creators (Built in n8n)

🚀 This project helps **content creators generate professional video scripts** using AI automation — entirely built with **n8n** and **free public APIs** (Perplexity, Wikipedia, and Email).

![UI Screenshot](assets/ui-screenshot.png)

---

## 🧠 Use Case
Many creators struggle to write high-quality video scripts quickly. This assistant:
- Accepts input like **topic**, **audience**, **tone**, **length**
- Fetches real-time context (Wikipedia, Google, etc.)
- Uses **Perplexity AI** to generate detailed, recent, engaging scripts
- Sends the final result to user’s email automatically

---

## 🔧 Tech Stack
- [n8n](https://n8n.io/) (Low-code workflow automation)
- Perplexity AI API (GPT-powered research and generation)
- Wikipedia API (/summary)
- Email (SMTP or Gmail node)

---

## 🛠️ Workflow Architecture

```mermaid
graph TD
    A[Webhook Input] --> B[Fetch Wikipedia / News Context]
    B --> C[Send to Perplexity API]
    C --> D[Format Script + Citations]
    D --> E[Send via Email]
