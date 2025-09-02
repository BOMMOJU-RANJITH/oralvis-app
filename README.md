# OralVis Monorepo

This repository contains:

- backend/ - Node/Express backend
- frontend/ - React frontend


# Project Overview

OralVis is a web application designed for dental clinics to manage and visualize patient scans efficiently.

Technicians can easily upload patient scans.

Dentists can securely view and analyze uploaded scans.

The system uses role-based access control to ensure that each user only has access to their respective functionality.

# Technology Stack

Frontend: React (Vite)

Backend: Node.js

Database: SQLite

Authentication: JWT (JSON Web Tokens)

Cloud Storage: Cloudinary for storing images

Deployment: Backend hosted on Render, Frontend on Netlify

# Screenshots
Login Page

<img width="1920" height="1080" alt="Screenshot 2025-09-02 120737" src="https://github.com/user-attachments/assets/c5f4ae21-18e7-4136-aa11-a2d3f18e8232" />

<img width="1920" height="1080" alt="Screenshot 2025-09-02 120821" src="https://github.com/user-attachments/assets/1d4b664a-16d6-4ea4-ab5b-d432e82d3e99" />

Technician Upload Page

<img width="1920" height="1080" alt="Screenshot 2025-09-02 120836" src="https://github.com/user-attachments/assets/d1982a5c-c577-49b2-a093-9ca8b5ec1516" />

<img width="1920" height="1080" alt="Screenshot 2025-09-02 120906" src="https://github.com/user-attachments/assets/fd7a306b-bd9e-44b3-872a-c1c951b5d847" />

Dentist Viewer Page

<img width="1920" height="1080" alt="Screenshot 2025-09-02 121200" src="https://github.com/user-attachments/assets/422e02b0-05a6-45b5-b740-bdd478a3ba3a" />

# Live Demo

(https://charming-sunburst-5796b3.netlify.app/)

ensure backend running(only if it is sleeping) by reloading https://oralvis-backened-6.onrender.com/ 

# Follow these steps to set up the project on your local machine.

1. Clone the repository
   
git clone https://github.com/BOMMOJU-RANJITH/oralvis-app.git

cd oralvis-app

2. Install dependencies
   
* Backend

cd backend

npm install

*Frontend

cd ../frontend

npm install

3. Set up environment variables

Create a .env file in both backend and frontend folders using the .env.example template.

backend/.env.example

PORT=5000
JWT_SECRET=your_jwt_secret_key
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
DB_URL=your_database_url

frontend/.env.example

VITE_API_BASE_URL=http://localhost:5000


Rename .env.example to .env and fill in your actual values.

4. Start the servers
* Backend

cd backend

* node index.js

Frontend

cd frontend

npm run dev


Backend will run on http://localhost:5000

Frontend will run on http://localhost:5173 (default for Vite)

# Login Credentials
Role	Email	Password

Technician	technician@example.com	tech123

Dentist	dentist@example.com	dentist123
