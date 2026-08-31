# PET_NEUTRI
# 🐾 PetNutri — AI-Powered Pet Nutrition & Health Companion

[![React](https://img.shields.io/badge/Frontend-React_18-blue?logo=react)](https://reactjs.org/)
[![Tailwind CSS](https://img.shields.io/badge/Styling-Tailwind_CSS-38B2AC?logo=tailwind-css)](https://tailwindcss.com/)
[![RAG Architecture](https://img.shields.io/badge/Backend-RAG System-green?logo=python)](https://python.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**PetNutri** is an end-to-end, science-backed pet nutrition and health web application designed to help pet parents optimize their pets' vitality, monitor daily hydration and diet goals, and receive instant, expert-validated nutritional guidance powered by a Retrieval-Augmented Generation (RAG) backend.

---

## ✨ Key Features

- 🥗 **Science-Backed Nutrition Advice:** Interactive AI Consultant providing ingredient safety, nutrient breakdowns (e.g., Antioxidants, Fiber), and recommended portion limits.
- 💬 **Interactive RAG Chatbot:** Real-time query system powered by a specialized veterinary knowledge base and hybrid retrieval mechanisms.
- 📊 **Daily Health Logging:** Visual progress tracking for pet hydration, activity, and dietary goals.
- 🔒 **Secure User Onboarding:** Seamless access management with email and social login flows.
- 📱 **Mobile-First Responsive UI:** Modern, clean, and intuitive UI built with React, Tailwind CSS, and Lucide React.

---

## 🏗️ System Architecture

```text
[ React Frontend ] ──(HTTP/JSON)──> [ FastAPI / Python Backend ] ──> [ Vector DB / RAG Pipeline ] ──> [ LLM Engine ]
```

1. **Frontend Layer:** Built with React, Vite, and Tailwind CSS. Communicates asynchronously with the backend via Axios.
2. **Backend RAG Pipeline:** Contextual vector retrieval powered by semantic similarity search over domain-specific pet nutrition knowledge sources.

---

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher)
- Python 3.10+
- Git

### 1. Clone the Repository
```bash
git clone [https://github.com/YOUR_USERNAME/petnutri-app.git](https://github.com/YOUR_USERNAME/petnutri-app.git)
cd petnutri-app
```

### 2. Frontend Setup
```bash
cd frontend
npm install
npm run dev
```

### 3. Backend Setup
```bash
cd ../backend
python -m venv venv
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate

pip install -r requirements.txt
python app.py
```

---

## 🛠️ Tech Stack

- **Frontend:** React, Vite, Tailwind CSS, Lucide Icons, Axios
- **Backend & RAG:** Python, FastAPI / Streamlit, LangChain, ChromaDB / FAISS, Gemini API / Groq API
- **Deployment:** Vercel (Frontend), Render / Streamlit Cloud (Backend)

---

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.

---

<p center="text-center">
  Crafted with ❤️ for pet health and longevity.
</p>
