# 🎁 GiftLink – Fullstack Gift Sharing Web Application
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Platform](https://img.shields.io/badge/platform-IBM%20Cloud%20%7C%20Render-blue.svg)
![Dockerized](https://img.shields.io/badge/Docker-Supported-blue.svg)

sharegiftweb is a fullstack gift-sharing web application that allows users to share, browse, and search for gifts based on specific filters like name, age range, category, and condition. It promotes a culture of giving and reuse.

The application is fully containerized using Docker and deployed to [Render](https://render.com). It consists of a React frontend and a Node.js/Express backend connected to MongoDB Atlas.

---

## 📸 Live Demo

- **Frontend:** [https://sharegiftweb.onrender.com](https://sharegiftweb.onrender.com)
- **Backend API:** [https://sharegift-backend.onrender.com/api/gifts](https://sharegift-backend.onrender.com/api/gifts)

---

## 📌 Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [API Endpoints](#api-endpoints)
- [Docker Reference](#docker-reference)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)

---

## ✨ Features
- 🎁 Gift creation and listing
- 🔍 Advanced search by name, age range, condition, and category
- ⚙️ RESTful API backend
- 🧑 User registration and management
- 🌍 Cloud deployment using Render
- 🧑 User registration and management
- 🐳 Full Docker containerization (frontend + backend)
- 🌐 CORS-enabled secure API
- 🔄 Real-time data syncing from MongoDB Atlas
- 🌐 Uses MongoDB Atlas for cloud data storage
---

## 🛠️ Tech Stack

| Area         | Technology                        |
|--------------|------------------------------------|
| Frontend     | React, HTML, CSS, JavaScript       |
| Backend      | Node.js, Express.js                |
| Database     | MongoDB Atlas                      |
| Deployment   | Render (Frontend + Backend)        |
| Containerization | Docker, Docker Compose         |
| Version Control | Git & GitHub                    |
| CICD            | GitHub Action                   |
---

## 📁 Project Structure

```bash
Fullstack-capstone-project/
│
├── giftlink-frontend/       # React frontend
│   ├── public/
│   ├── src/
│   └── Dockerfile
│
├── giftlink-backend/        # Express backend
│   ├── routes/
│   ├── models/
│   ├── util/
│   └── Dockerfile
│
├── docker-compose.yml
└── README.md


⚙️ Getting Started
Prerequisites
Node.js & npm

Docker & Docker Compose

Clone the Repository
bash
Copy
Edit
git clone https://github.com/yourusername/giftlink.git
cd giftlink
Run Locally with Docker
bash
Copy
Edit
docker-compose up --build
Frontend: http://localhost:3000

Backend: http://localhost:3060/api/gifts

📡 API Endpoints
Base URL: https://giftlink-backend.onrender.com/api/gifts

Method	Endpoint	Description
GET	/api/gifts	Fetch all gifts
POST	/api/gifts	Create a new gift
GET	/api/gifts/:id	Fetch gift by ID
DELETE	/api/gifts/:id	Delete a gift

Sample POST Request:

json
Copy
Edit
{
  "name": "Teddy Bear",
  "ageRange": "3-6",
  "category": "Toys",
  "condition": "New"
}
🐳 Docker Reference
To run only the backend:

bash
Copy
Edit
cd giftlink-backend
docker build -t giftlink-backend .
docker run -p 3060:3060 giftlink-backend
To run only the frontend:

bash
Copy
Edit
cd giftlink-frontend
docker build -t giftlink-frontend .
docker run -p 3000:3000 giftlink-frontend
To run both with Docker Compose:

bash
Copy
Edit
docker-compose up --build
🚀 Deployment
Both frontend and backend are deployed using Render:

Backend uses the Express Dockerfile inside giftlink-backend/

Frontend uses the React Dockerfile inside giftlink-frontend/

Ensure your REACT_APP_API_URL in the frontend points to your Render backend URL.

🤝 Contributing
Contributions are welcome! Here’s how:

Fork the repository

Create a new branch: git checkout -b feature/your-feature

Commit your changes: git commit -m "Add your feature"

Push to the branch: git push origin feature/your-feature

Open a Pull Request

📄 License
This project is licensed under the Apache License.
See the LICENSE file for more details.

🙌 Acknowledgements
IBM Full Stack JavaScript Capstone Project

Render.com for free cloud hosting

MongoDB Atlas for cloud database support

👤 Author
Built by Eze George
