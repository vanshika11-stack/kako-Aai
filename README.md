# SIH26003 AI-based cognitive gaming &amp; memory assistance platform for elderly dementia patients in North Eastern Region (NER) – SIH 2026

Smart India Hackathon 2026 Category	Software
Theme	MedTech / BioTech / HealthTech Ministry -Ministry of Development of North Eastern Region (MDoNER)/ 
# Kako-Aai
**AI-based cognitive gaming & memory assistance platform for elderly dementia patients in North Eastern Region (NER)**  
Smart India Hackathon 2026 | Problem Statement ID: SIH26003 
Team: NEuroLife | SHARDA UNIVERSITY AGRA

🔗 Live demo / docs: https://gqjkk8cc4g.zite.so  
🎥 Demo video:  
📱 App: `/app` | 🖥 Backend: `/backend` | 🌐 Dashboard: `/dashboard`

---

## Problem

Elderly people in the North East face rising dementia and memory loss, but remote areas lack specialist care, cognitive therapy, and simple tools for daily mental stimulation. Families are distant or overburdened, and ASHA workers have no digital way to monitor or engage elders in local languages.

---

## Solution

Kako-Aai is a culturally familiar, voice-first AI companion that:
- Plays adaptive memory/recognition games using the elder’s own family photos and cultural images.
- Speaks in NER languages (Assamese, Hindi, Bengali, etc.) to greet, praise, encourage, and remind.
- Provides medicine, hydration, and routine reminders with voice + big on-screen messages.
- Works offline and syncs when connectivity is available.
- Connects to a family/ASHA dashboard for engagement monitoring, alerts, and follow-up.

---

## Features

- Elder mobile app (Flutter, Android, offline-first)
- Cognitive games: Same Photo Find, Who Is This?, Routine Sequence, Pattern/Object Recognition
- Voice AI companion (multilingual templates, Bhashini/device TTS fallback)
- Reminders: medicine, hydration, activities, appointments
- Family & ASHA dashboards (engagement, alerts, notes)
- Optional adaptive audio layer (regional music, ambient soundscapes; 40 Hz exploratory)

---

## Architecture

- **Mobile app:** Flutter + SQLite/Isar (offline) + local rule engine
- **Backend:** FastAPI (Python) + PostgreSQL/SQLite
- **Dashboards:** React/Next or Flutter Web
- **Language:** Bhashini APIs + device TTS/STT fallback
- **Sync:** Local queue → backend when online

See `docs/architecture.md` for detailed diagrams.

---

## Getting Started

### App (Flutter)

```bash
cd app
flutter pub get
flutter run
```

### Backend (FastAPI)

```bash
cd backend
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload
```

### Dashboard

```bash
cd dashboard
# install and run instructions based on your stack
```

---

## Research & Validation

- Caregiver interviews: [N]  
- Clinician/ASHA reviews: [N]  
- Usability tests: [N]  

See `research/` for interview guides, consent forms, and insights.

---

## Safety & Ethics

- Not a diagnostic or treatment tool.
- Consent-based data sharing.
- Role-based access (elder, family, ASHA).
- Clear disclaimers and human escalation for distress alerts.

See `docs/safety_ethics.md`.

---

## Team

- vanshika - team leader
-saniya
-anshika
-charu
-priyanshi
-priyanshu
Contact: vanshi13255@gmail.com

---

## License

MIT License (or your chosen license)
