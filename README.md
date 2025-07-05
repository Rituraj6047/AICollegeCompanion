# 🧠 AI College Companion 📚

An intelligent academic assistant that generates **personalized daily study plans** using Generative AI. It analyzes your **academic calendar**, **timetable**, and **syllabus** to suggest what you should study each day — all displayed on a modern, student-friendly dashboard.

---

## 🚀 Features

- ✅ Upload Academic Calendar, Timetable, and Subject-wise Syllabus (PDFs)
- 🤖 AI-generated daily To-Do list using Gemini API
- 📊 Progress tracking and weekly summary
- 🗓️ Upcoming deadlines panel
- 🧼 Clean, responsive UI with React.js
- ⚙️ Backend powered by Node.js + Express

---

## 🧠 How It Works

1. **Upload Documents**:
   - Academic calendar
   - Time-table
   - Subject-wise syllabus

2. **AI Processing**:
   - Gemini API (Google Generative AI) analyzes all documents
   - It understands semester timelines, subject schedule, and syllabus scope

3. **Smart To-Do List**:
   - You get a personalized study plan for **today**
   - Based on your actual subjects and upcoming exams

---

## 🧱 Tech Stack

| Frontend  | Backend       | AI Layer             | Others            |
|-----------|----------------|----------------------|--------------------|
| React.js  | Node.js + Express | Gemini Pro Vision API | Multer (file upload), Axios |

---

## 📦 Setup Instructions

### 1. Clone the repo

```bash
git clone https://github.com/your-username/ai-college-companion.git
cd ai-college-companion
```

### 2. Start the backend server

```bash
cd server
npm install
touch .env
```

Inside `.env`, add:
```
GEMINI_API_KEY=your_google_generative_ai_key_here
```

Then:
```bash
npm start
```

### 3. Start the frontend

```bash
cd ../client
npm install
npm start
```

Frontend will run on: `http://localhost:3000`  
Backend will run on: `http://localhost:5000`

---

## 📂 Project Structure

```
study-sync-app/
├── client/         # React frontend
│   ├── components/
│   └── App.js, index.js
├── server/         # Node.js backend
│   ├── routes/
│   ├── uploads/
│   ├── gemini.js   # AI logic here
│   └── server.js
```

---

## 📅 To-Do Plan Format (AI Output Example)

```json
[
  {
    "subject": "DBMS",
    "topic": "Normalization",
    "duration": "1.5h"
  },
  {
    "subject": "Math",
    "topic": "Partial Derivatives",
    "duration": "2h"
  }
]
```

---

## 🔮 Future Features

- ✅ Save task progress in MongoDB
- ✅ Login / signup for multiple students
- ⏰ Study reminder notifications
- 🎤 Voice command support
- 📈 Weekly and monthly planning insights

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you’d like to change or add.

---

## 📄 License

This project is licensed under the MIT License.

---

## 🙌 Acknowledgements

- [Google Generative AI](https://ai.google.dev/)
- [React](https://reactjs.org)
- [Node.js](https://nodejs.org)
- Inspired by the real needs of college students struggling to plan smartly.
