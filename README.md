# pustiAI-maternal-health
Dialect-aware, voice-first Bangla AI screening platform translating maternal nutrition science into local kitchen units and early anemia detection.



# PustiAI (পুষ্টি AI) — Voice-First AI Companion for Rural Maternal Nutrition

PustiAI is an AI-powered, dialect-aware voice companion designed to eliminate maternal malnutrition and enable early anemia screening for low-literacy rural mothers in Bangladesh.

Built for the **Grameenphone FutureMakers 2026** competition under the **Healthcare & Mental Wellbeing** track.

---

## Key Features

- **Voice-First Interaction:** Allows rural users to speak naturally in local Bangla dialects without requiring text literacy.
- **Semantic Symptom Screening:** Utilizes multilingual vector embeddings to map spoken symptoms to clinical severity tiers.
- **Kitchen Unit Translations:** Translates metric dietary targets into measurable household utensils (*e.g., 1 cup lentils + 1 spoon lemon juice*).
- **Smart Plant-Protein Synergy:** Recommends affordable, complete-protein plant pairings (*grain + legume*) when animal protein is unaffordable.
- **Offline-First Clinic Routing:** Directs high-risk cases to nearby Upazila Health Complexes using localized clinic lookup tables.

---

## Tech Stack & Architecture

- **Language & Core Logic:** Python 3.10+
- **Speech-to-Text (ASR):** OpenAI Whisper / Fine-Tuned Bangla Speech Models
- **Vector Embeddings:** `sentence-transformers` (`paraphrase-multilingual-MiniLM-L12-v2`)
- **Classifier:** Cosine Similarity Intent Matching Engine
- **Delivery Channels:** Telegram Bot API & Streamlit Web Interface

---

## Quickstart & Local Setup

### 1. Clone Repository & Install Dependencies
```bash
git clone [https://github.com/YOUR_USERNAME/pusti-ai-maternal-health.git](https://github.com/YOUR_USERNAME/pusti-ai-maternal-health.git)
cd pusti-ai-maternal-health
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
