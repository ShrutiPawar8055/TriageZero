# 🏥 Triage AI - Intelligent Healthcare Management & Diagnostics

A state-of-the-art healthcare triage application combining a **Neumorphic UI** with **Real-time AI Diagnostics**. This platform enables healthcare providers to manage patients, perform AI-assisted triage, and interact with an AI Voice Assistant for symptom assessment.

---

## ✨ Key Features

- **🗣️ AI Voice Assistant**: Real-time conversational interface powered by **LiveKit** for hands-free symptom assessment.
- **🎙️ Cough Analysis**: Deep learning-based cough classification (Sick vs. Healthy) using **TensorFlow**.
- **👁️ Eye Scan (Anemia Detection)**: Computer vision-based analysis for detecting signs of anemia from eye scans.
- **📊 Interactive Analytics**: Comprehensive dashboard for tracking patient trends and diagnostic outcomes.
- **🌐 Multi-language Support**: Fully localized in **English**, **Hindi**, and **Bengali** to serve diverse patient populations.
- **📱 Neumorphic UI**: A modern, soft-UI design system built with **Tailwind CSS** for a superior user experience.
- **📄 Triage Reports**: Automated PDF generation for diagnostic summaries and patient records.

---

## 🛠️ Tech Stack

### Frontend
- **React.js** (Vite)
- **Tailwind CSS** (Neumorphic Design System)
- **Framer Motion** (Smooth Page Transitions)
- **LiveKit Client** (WebRTC Voice Interaction)
- **Lucide React** (Modern Iconography)
- **i18next** (Localization)

### Backend & ML
- **FastAPI** (Python High-Performance API)
- **TensorFlow / Keras** (Deep Learning Models)
- **SQLite** (Persistent Patient Records)
- **Librosa** (Audio Processing for Cough Analysis)
- **OpenCV / PIL** (Image Processing for Eye Scans)

---

## 🚀 Getting Started

### 1. Prerequisites
- **Node.js** (v18+)
- **Python** (3.9+)
- **npm** or **yarn**

### 2. Installation

#### Clone the Repository
```bash
git clone https://github.com/Ommali8421/Triage.git
cd Triage
```

#### Frontend Setup
```bash
npm install
```

#### Backend Setup
```bash
pip install -r "ML models/requirements.txt"
```

### 3. Environment Configuration
Create a `.env` file in the root and another in the `src/` directory (refer to `.env.example`):
```env
# Backend API Keys
LIVEKIT_API_KEY=your_key
LIVEKIT_API_SECRET=your_secret
LIVEKIT_URL=your_url

# Frontend
VITE_API_URL=http://localhost:8000
VITE_LIVEKIT_URL=wss://your_url
```

### 4. Running the Application

#### Start All Servers (Recommended)
We provide a convenient PowerShell script to launch both servers:
```powershell
./start.ps1
```

#### Manual Start
**Backend:**
```bash
python app.py
```

**Frontend:**
```bash
npm run dev
```

---

## 📁 Project Structure

```text
├── ML models/          # TensorFlow models and Python triage logic
├── src/
│   ├── components/     # Reusable Neumorphic UI & Layout components
│   ├── pages/          # Application views (Home, Triage, Voice, etc.)
│   ├── voice-agent/    # LiveKit integration & Voice UI logic
│   ├── utils/          # PDF generation & disease knowledge base
│   └── translations.js # Localization strings (EN, HI, BN)
├── app.py              # Main FastAPI application
├── triage_records.db   # SQLite database (auto-generated)
└── start.ps1           # Automated startup script
```

---

## 🔒 Security & Privacy
- **API Security**: Environment variables are strictly ignored in Git.
- **Data Privacy**: Local-first processing for diagnostic data.

---

## 🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

---

