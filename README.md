# UIS Hackathon — Smart Marks Manager

An **AI-powered teacher dashboard** built for the **GEMS United Indian School (UIS) Hackathon**. Smart Marks Manager helps teachers record, analyze, and report student marks in one place — replacing scattered spreadsheets with a fast, modern web app.

**Author:** [Farhan Mohammed R](https://github.com/FARHANMOHAMMED-R)  
**Repository:** [github.com/FARHANMOHAMMED-R/UIS-Hackathon](https://github.com/FARHANMOHAMMED-R/UIS-Hackathon)

---

## Problem

Teachers spend hours juggling Excel sheets, manual grade calculations, and handwritten report cards. Marks get lost, trends are hard to spot, and generating parent-ready reports takes too long.

## Solution

Smart Marks Manager gives teachers a single dashboard to:

- Manage **students**, **classes**, and **subjects**
- Enter and update **marks** by exam type (Unit Test, Midterm, Practical, Final Exam)
- View **analytics** — class averages, pass/fail rates, and performance charts
- Generate **AI-assisted remarks** and insights for students
- Export **PDF reports** and **Excel spreadsheets**
- Work **offline** with built-in demo data, or connect **Firebase** for real-time cloud sync

---

## Features

| Feature | Description |
|--------|-------------|
| **Student management** | Add, edit, and search students by class, section, and roll number |
| **Marks entry** | Bulk entry with validation against max/pass marks per subject |
| **Dashboard & charts** | Visual overview of class performance using interactive charts |
| **AI insights** | Smart remark suggestions powered by OpenAI (optional) |
| **Reports** | Export marksheets to PDF and Excel |
| **Dark / light theme** | Comfortable UI for long grading sessions |
| **Offline demo mode** | Pre-loaded seed data — no setup required to explore the app |
| **Firebase integration** | Optional Auth + Firestore for production use |

---

## Tech Stack

| Layer | Technology |
|-------|------------|
| Frontend | React 18, Vite 6 |
| Styling | Tailwind CSS, Framer Motion |
| Routing | React Router v7 |
| Charts | Recharts |
| Backend (optional) | Firebase Auth & Firestore |
| AI (optional) | OpenAI API |
| Export | jsPDF, xlsx |
| Notifications | React Hot Toast |

---

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) 18 or later
- npm (comes with Node.js)

### Installation

```bash
git clone https://github.com/FARHANMOHAMMED-R/UIS-Hackathon.git
cd UIS-Hackathon
npm install
```

### Run locally

```bash
npm run dev
```

Open the URL shown in the terminal (usually `http://localhost:5173`).

### Environment variables (optional)

Copy `.env.example` to `.env` and fill in your credentials to enable Firebase and AI features:

```bash
cp .env.example .env
```

| Variable | Purpose |
|----------|---------|
| `VITE_FIREBASE_*` | Firebase web app config for auth and database |
| `VITE_OPENAI_API_KEY` | Enables real AI remark generation |

Without these keys, the app runs in **demo mode** with local seed data and built-in placeholder AI responses.

### Build for production

```bash
npm run build
npm run preview
```

---

## Project Structure

```
UIS-Hackathon/
├── src/
│   ├── components/     # UI components (dashboard, forms, charts)
│   ├── context/        # React context (auth, theme, data)
│   ├── firebase/       # Firebase configuration
│   ├── services/       # Data layer and seed data
│   └── utils/          # Shared helpers
├── public/             # Static assets
├── index.html
├── package.json
└── README.md
```

---

## Hackathon Context

This project was created for the **UIS Hackathon** — a school innovation challenge focused on building practical tools that improve everyday teaching and learning at GEMS United Indian School.

**Target users:** Teachers and school administrators  
**Goal:** Reduce grading overhead and give educators actionable insights about student performance

---

## Roadmap

- [ ] Complete core UI components and routing
- [ ] Firebase authentication and cloud sync
- [ ] Parent portal (read-only marks view)
- [ ] SMS/email notifications for low-performing students
- [ ] Mobile-responsive layout polish

---

## License

This project is open source and available for educational and hackathon use.

---

## Contact

**Farhan Mohammed R**  
GitHub: [@FARHANMOHAMMED-R](https://github.com/FARHANMOHAMMED-R)
