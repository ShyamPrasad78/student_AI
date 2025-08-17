🎓 Student AI

An AI-powered student record and performance management system that helps manage student data, track progress, and provide insights using Machine Learning & modern web technologies.

🚀 Features

📂 Student Record Management – Store and manage personal, academic, and activity details.

🤖 AI Insights – Predict student performance, identify weak areas, and suggest improvements.

📊 Analytics Dashboard – Visualize performance trends across semesters, subjects, and activities.

🔐 Authentication System – Secure login for students, teachers, and admins.

🌐 Modern Web App – React frontend with responsive UI and smooth experience.

⚡ REST API – Backend with scalable APIs for student data and predictions.

🏗️ Tech Stack

Frontend

React.js (Vite + Tailwind CSS + shadcn/ui)

Axios for API requests

Backend

Django REST Framework / FastAPI (depending on version you built)

PostgreSQL / MySQL as DB

JWT Authentication

Machine Learning

Python (Pandas, NumPy, Scikit-learn, TensorFlow)

AI models for student performance prediction

Deployment

Dockerized services (Frontend + Backend + ML models)

AWS EC2 / Heroku (deployment-ready)

📂 Project Structure
student-ai/
│── backend/              
│   ├── models/           
│   ├── api/             
│   ├── ml/             
│   └── requirements.txt  
│
│── frontend/             
│   ├── src/components/   
│   ├── src/pages/       
│   └── package.json
│
│── docker-compose.yml  
│── README.md             

⚙️ Installation & Setup
🔹 Backend (Django/FastAPI)
cd backend
python -m venv venv
source venv/bin/activate   # (Linux/Mac)
venv\Scripts\activate      # (Windows)

pip install -r requirements.txt
python manage.py migrate   # Django (or uvicorn main:app --reload for FastAPI)


Run backend server:

python manage.py runserver  # Django
uvicorn main:app --reload   # FastAPI

🔹 Frontend (React)
cd frontend
npm install
npm run dev


Runs on http://localhost:5173 (Vite).

🔹 ML Model Training
cd backend/ml
python train_model.py


This generates a saved model used by the backend API.

🖼️ Screenshots

Dashboard with analytics

Student profile management

AI-powered performance prediction

📊 Example API Endpoints
Method	Endpoint	Description
GET	/api/students/	Get all students
POST	/api/students/	Add new student
GET	/api/predict/<id>	Predict performance for a student
POST	/api/auth/login/	Login & get JWT token
🤝 Contributing

Fork this repo

Create a new branch (feature-xyz)

Commit changes

Open a Pull Request

📜 License

This project is licensed under the MIT License.
