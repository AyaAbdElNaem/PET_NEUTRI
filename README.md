# 🐾 PetNutri — AI-Powered Pet Nutrition & Health Companion

[![React](https://img.shields.io/badge/Frontend-React_18-blue?logo=react)](https://reactjs.org/)
[![Tailwind CSS](https://img.shields.io/badge/Styling-Tailwind_CSS-38B2AC?logo=tailwind-css)](https://tailwindcss.com/)

**PetNutri** is an end-to-end, science-backed pet nutrition and health web application designed to help pet parents optimize their pets' vitality, monitor daily hydration and diet goals, and receive instant, expert-validated nutritional guidance powered by a Retrieval-Augmented Generation (RAG) backend.

---

## ✨ Key Features

- 🥗 **Science-Backed Nutrition Advice:** Interactive AI Consultant providing ingredient safety, nutrient breakdowns (e.g., Antioxidants, Fiber), and recommended portion limits.
- 💬 **Interactive RAG Chatbot:** Real-time query system powered by a specialized veterinary knowledge base and hybrid retrieval mechanisms.
- 📊 **Daily Health Logging:** Visual progress tracking for pet hydration, activity, and dietary goals.
- 🔒 **Secure User Onboarding:** Seamless access management with email and social login flows.
- 📱 **Responsive UI:** Modern, clean, and intuitive UI built with Streamlit and CSS styling.

---

## 🏗️ System Architecture & Workflow

The architecture follows an end-to-end RAG data pipeline split into 6 distinct operational layers:

```mermaid
flowchart LR
    classDef data fill:#e1f5fe,stroke:#0288d1,stroke-width:2px,color:#01579b;
    classDef db fill:#fff3e0,stroke:#f57c00,stroke-width:2px,color:#e65100;
    classDef ai fill:#e8f5e9,stroke:#388e3c,stroke-width:2px,color:#1b5e20;
    classDef api fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px,color:#4a148c;
    classDef ui fill:#ffebee,stroke:#d32f2f,stroke-width:2px,color:#b71c1c;

    A[Data Sources: Veterinary Specs & Nutrition Docs]:::data --> B[(Preprocessing & Text Chunking)]:::db
    B --> C[Vectorization & ChromaDB Storage]:::ai
    C --> D[Context Retrieval & Prompt Engine]:::api
    D --> E[RAG Evaluation & Safety Scoring]:::ai
    E --> F[Interactive Streamlit Application & UI]:::ui

<p center="text-center">
  Crafted with ❤️ for pet health and longevity.
</p>
