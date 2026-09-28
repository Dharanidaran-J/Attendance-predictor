# 🎓 AttendIQ – Student Attendance Predictor

A responsive attendance management web app that helps students track attendance, simulate OD / medical leave, and ask an Attendance Advisor chatbot whether they can safely take leave, all against the **75% minimum** requirement.

🔗 **Live demo:** https://YOUR-USERNAME.github.io/attendance-predictor/

## ✨ Features
- Dashboard with student profile, overall and subject-wise attendance
- Colour-coded status: 🟢 Safe (80%+), 🟡 Warning (75–79.99%), 🔴 Critical (below 75%)
- Donut, bar and trend charts that update automatically
- OD / Medical Leave Simulator with a configurable policy (present, excluded or absent)
- Attendance Advisor chatbot that answers using live dashboard data
- Risk analysis: classes you can miss, and classes needed to reach 75% / 80%
- Mark Present / Absent, edit or add subjects, edit profile
- Light / dark mode, mobile responsive, saved in localStorage

## 🧮 Calculation Logic
- Attendance % = Attended / Total × 100
- After missing n classes = Attended / (Total + n) × 100
- Max classes you can miss = floor(Attended × 100 / Required − Total)
- Classes needed to reach T% = ceil((T × Total − 100 × Attended) / (100 − T))

The dashboard, simulator and chatbot all use the same calculation functions and the same data.

## 🛠️ Tech Stack
HTML, CSS, JavaScript (single file) · Chart.js · localStorage

## 🚀 Run Locally
Download or clone the repo and open `index.html` in any browser.

## 🌐 Deploy
Settings → Pages → Branch `main` → `/ (root)` → Save.

## 🔮 Future Improvements
- Real LLM integration for open-ended questions
- Timetable-based prediction
- CSV import and multi-student login
- Alerts when attendance nears 75%

## 👥 Team
YOUR TEAM NAME (add member names)
