# Campus Event Management System

A full-stack application for organizing, approving, and managing university events with smart resource recommendations and reporting.

---

## 📦 Project Structure

```
.
├── tester.py                # Automated API event booking tester
├── backend/                 # Node.js Express backend
│   ├── index.js             # Main server entry
│   ├── routes/              # API routes (event, user, venue)
│   ├── models/              # Mongoose models (Event, Approver, User, Venue, etc.)
│   ├── utils/               # Utility modules (AI, Supabase)
│   ├── data/                # University data
│   ├── .env                 # Environment variables
│   └── package.json         # Backend dependencies
├── frontend/                # React frontend
│   ├── src/                 # Source code (Dashboard, ReportPage, etc.)
│   ├── public/              # Static assets
│   └── package.json         # Frontend dependencies
└── HF_v2/                   # Gemini NLP event scheduler (Python)
```

---

## 🚀 Features

- **Multi-level Approval Workflow:** Automatic routing to approvers based on event type.
- **Unified Calendar:** Visualize all events, statuses, and details.
- **Smart Resource Recommendation:** AI suggests resources post-approval.
- **Resource Allocation & Email Status:** Confirm allocations and track email notifications.
- **Event Reports:** Downloadable PDF reports for each event.
- **Automated API Testing:** [`tester.py`](tester.py) script for bulk event booking.

---

## 🛠️ Setup Instructions

### 1. Clone the Repository

```bash
git clone <your-repo-url>
cd <your-repo-folder>
```

### 2. Backend Setup

```bash
cd backend
npm install
cp .env.example .env   # Edit with your MongoDB URI and other secrets
node index.js
```
- The API will be available at `http://localhost:5100`.

### 3. Frontend Setup

```bash
cd frontend
npm install
npm start
```
- Open [http://localhost:3000](http://localhost:3000) in your browser.

### 4. Automated Event Booking Test

```bash
python tester.py
```
- Sends 50 randomized event bookings to the backend API.

### 5. Gemini NLP Event Scheduler (Optional)

See [HF_v2/README.md](HF_v2/README.md) for instructions on running the Gemini-powered event scheduler.

---

## 📑 Usage

- Organizers can create events, view approval status, and confirm resources.
- Approvers receive event requests and can approve/reject.
- Reports are generated for each event and can be downloaded as PDF.

---

## 📚 Documentation

- Frontend: [frontend/README.md](frontend/README.md)
- Gemini NLP Scheduler: [HF_v2/README.md](HF_v2/README.md)
- Event Prioritizer: [HF_v2/backend/event_prioritizer/README.md](HF_v2/backend/event_prioritizer/README.md)

---

## ✨ Credits

**Institution** : Kumaraguru College of Technology,Coimbatore

**Members** :
1. Adarsh J
2. Akshayaa US
3. Deebak Balaji M

---

## 📝 License

MIT License (see LICENSE file)
