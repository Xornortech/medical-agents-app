# 🧠 Medical Multi-Agent AI System

This project allows you to:
- 📤 Upload PDFs
- 🧠 Extract and embed medical content into a vector DB (Chroma)
- 🤖 Generate presentations using agents (Markdown + JSON)
- 📎 Export to PowerPoint using an external API

## 🛠 Features
- LangChain-style agent system (Extractor, Interpreter, Synthesizer)
- OpenAI GPT-4 + Chroma RAG
- REST API with Express.js
- Dockerized setup
- Frontend UI (HTML + JS)

## 🚀 Getting Started

### 1. Clone the project
```bash
git clone https://github.com/Xornortech/medical-agents-app.git
cd medical-agents-app
```

### 2. Configure Environment
Copy the example env file:
```bash
cp .env.example .env
```
Edit .env and set:
- `OPENAI_API_KEY=...`
- `SLIDE_API_URL=https://...`

### 3. Run with Docker
```bash
docker-compose up --build
```

Access app at http://localhost:3000

## 📂 Folder Structure
```
├── server.js
├── routes/
├── controllers/
├── services/
├── utils/
├── public/
│   ├── index.html
│   ├── css/
│   └── js/
├── uploads/
├── .env.example
├── Dockerfile
└── docker-compose.yml
```

## 🧪 API Endpoints
| Endpoint               | Description                                |
|------------------------|--------------------------------------------|
| POST /upload-pdf       | Upload a medical PDF and store in Chroma  |
| POST /generate-presentation | Create presentation in Markdown, JSON, and .pptx |
| POST /analyze          | Analyze medical text using agents         |
| POST /ingest           | Manually ingest documents into vector DB  |

## 📄 License
MIT

