# Dairy--pro-
It is a SaaS based final year group project done by group of 2 people - me and my friend


# Structure
Dairy Pro Connect is a comprehensive dairy management system built with React (Vite) for the frontend and Flask for the backend.

🏗️ Architecture
Frontend: React + TypeScript + Vite + Shadcn UI (Hosted on Vercel)
Backend: Flask (Python) (Hosted on Railway)
Database: PostgreSQL (Hosted on Neon)
Emailing: Flask-Mail via Gmail SMTP
🚀 Deployment Instructions
1. Database (Neon)
Create a project on Neon.tech.
Copy the Connection String (DATABASE_URL).
2. Backend (Railway)
Create a new project on Railway.app.
Connect your GitHub repository.
Root Directory: / (Railway will automatically detect the Procfile).
Add the following Environment Variables:
DATABASE_URL: (Your Neon connection string)
MAIL_SERVER: smtp.gmail.com
MAIL_PORT: 587
MAIL_USE_TLS: True
MAIL_USERNAME: (Your Gmail)
MAIL_PASSWORD: (Your App Password)
Deploy. You will get a Public URL (e.g., https://your-backend.up.railway.app).
3. Frontend (Vercel)
Create a new project on Vercel.
Connect your GitHub repository.
Add the following Environment Variable:
VITE_API_URL: (Your Railway Backend URL)
Deploy.
🛠️ Local Development
Prerequisites
Node.js & npm
Python 3.10+
Setup
Clone the Repo:

git clone <your-repo-link>
cd dairy-pro-connect
Frontend Setup:

npm install
npm run dev
Backend Setup:

cd backend
python -m venv venv
source venv/bin/activate  # Or venv\Scripts\activate on Windows
pip install -r requirements.txt
python app.py
📂 Project Structure
/src: Frontend source code.
/backend: Flask backend logic.
Procfile: Railway configuration.
vercel.json: Vercel configuration.
requirements.txt: Python dependencies.
