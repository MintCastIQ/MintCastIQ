# MintCastIQ
- MintCastIQ is a **web‑first platform** designed for resilient, audit‑grade trading card workflows.  
- Originally prototyped as an Android app, MintCastIQ has shifted focus to the web, with a mobile companion planned for the future.
---
## 🚀 Vision
- Build contributor‑safe, forensic‑grade pipelines for trading card capture and validation.
- Empower contributors with ergonomic tooling, clear documentation, and audit‑ready workflows.
## 📂 Repository Contents
- `README.md` — overview and vision
- `CONTRIBUTING.md` — guidelines for safe and effective collaboration
- `PRIVACY.md` — transparency on data handling and contributor safety
- `DEVELOPMENT_GUIDE.md` — technical standards, workflows, and onboarding notes
---
## 🧩 Getting Started
Clone the repository:
```bash
git clone https://github.com/MintCastIQ/MintCastIQ.git
cd MintCastIQ
```
## ⚛️Part 1 - React Frontend Setup
### Install dependencies:
```bash
cd frontend
npm install
```
### Run the development server:
```bash
npm run dev
```
This will start the React app on http://localhost:3000. Make sure it’s configured to talk to the Flask backend (see .env or proxy settings).
---
## Part 2 — Flask Backend Setup
### Create a virtual environment:
```bash
cd backend
python3 -m venv venv
source venv/bin/activate
```
### Install dependencies:
```bash
pip install -r requirements.txt
```
### Run the Flask server:
```bash
flask run
```
This will start the backend on http://localhost:5000. You can configure routes, grading logic, and metadata indexing here.
---
## Part 3 — Docker Compose (Optional Unified Dev)
### 🐳 Unified Dev (Docker Compose)
To run both frontend and backend together:
```bash
docker-compose up --build
```
This will:
- Build and run the React frontend and Flask backend in separate containers.
- Expose ports 3000 (frontend) and 5000 (backend).
- Ensure audit-grade reproducibility across environments.
- Make sure your docker-compose.yml defines volumes, environment variables, and health checks for contributor safety.
---
### Part 4
## 🔒 Principles
- **Audit‑grade clarity**: Every workflow is documented and reproducible.
- **Contributor safety**: No secrets or personal data in commits.
- **Modularity**: Infrastructure and tooling are designed for scale and adaptability.
---
## 🤝 Community
- MintCastIQ thrives on collaboration.  
- Please read the [`CONTRIBUTING.md`](CONTRIBUTING.md) before submitting pull requests
- Join discussions to help shape the roadmap.
---
## 📜 License
This project will be released under an open‑source license (to be finalized).  
All contributions are subject to review for audit clarity and contributor safety.
