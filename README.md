# 🎁 GiftLink - Gift Sharing Web Application

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Node.js](https://img.shields.io/badge/Backend-Node.js-blue.svg)](https://nodejs.org/)
[![MongoDB](https://img.shields.io/badge/Database-MongoDB-green.svg)](https://www.mongodb.com/)
[![React](https://img.shields.io/badge/Frontend-React-blue.svg)](https://reactjs.org/)
[![Deployed on IBM Cloud](https://img.shields.io/badge/Deployed-IBM%20Cloud-blue)](https://giftwebsite.1wa78gnru4vq.us-south.codeengine.appdomain.cloud)

---

## 📌 Project Overview

**GiftLink** is a fullstack JavaScript web application that allows users to share and discover gifts. Users can register, post gifts, and search for gifts by name, category, condition, or age range. It is built using modern technologies like **React**, **Node.js**, and **MongoDB**, and is deployed on IBM Cloud using Docker and Code Engine.

---

## ✨ Features

- 👤 User registration
- 🎁 Add and manage gift listings
- 🔍 Filter gifts by:
  - Name (case-insensitive partial match)
  - Category (e.g., toys, books)
  - Condition (e.g., new, used)
  - Age range (via slider)
- 🔐 RESTful API with secure data handling
- 🌐 Fully containerized and deployed to IBM Cloud

---

## 🛠 Tech Stack

| Layer         | Technology                          |
|---------------|--------------------------------------|
| Frontend      | React, HTML, CSS, JavaScript         |
| Backend       | Node.js, Express.js                  |
| Database      | MongoDB                              |
| API           | RESTful endpoints                    |
| Containerization | Docker                           |
| Cloud Deployment | IBM Cloud, IBM Code Engine       |

---

## 🚀 Setup Instructions

### Prerequisites

- Node.js & npm installed
- MongoDB instance (local or cloud)
- Docker (for containerized build)
- IBM Cloud CLI (for deployment)

### Backend Setup

```bash
git clone https://github.com/your-username/giftlink.git
cd giftlink-backend
npm install
npm start


📘 Usage Guide
Open the React frontend interface.

Register as a new user.

Add a new gift with name, category, condition, and age suitability.

Use the search bar and filters to find available gifts.

📡 API Endpoints
GET /api/search
Query gifts by filters.

Example Request:

sql
Copy
Edit
GET /api/search?name=lego&age_years=8&category=toys&condition=new
Query Parameters:

name (optional)

age_years (optional, slider-based)

category (optional)

condition (optional)

Example Response:

json
Copy
Edit
[
  {
    "name": "Lego Set",
    "age_years": 8,
    "category": "toys",
    "condition": "new"
  }
]
🐳 Docker Reference
Dockerfile (Backend or Fullstack Container)
Dockerfile
Copy
Edit
# Use Node.js base image
FROM node:20

# Create app directory
WORKDIR /app

# Install dependencies
COPY package*.json ./
RUN npm install

# Copy app files
COPY . .

# Expose port
EXPOSE 3060

# Start the app
CMD ["node", "app.js"]
Docker Commands
bash
Copy
Edit
# Build the image
docker build -t giftapp .

# Tag the image for IBM Cloud Container Registry
docker tag giftapp us.icr.io/sn-labs-ezegeorgechu/giftapp

# Push to IBM Cloud
docker push us.icr.io/sn-labs-ezegeorgechu/giftapp
☁️ Deployment to IBM Cloud
Log in to IBM Cloud CLI

Create a Code Engine project

Deploy using the pushed Docker image

Set environment variables and expose required ports

Access your app via:
https://giftwebsite.1wa78gnru4vq.us-south.codeengine.appdomain.cloud

🤝 Contributing
Contributions are welcome! Please follow these steps:

Fork the repository

Create a feature branch (git checkout -b feature-name)

Commit your changes (git commit -m 'Add feature')

Push to the branch (git push origin feature-name)

Open a Pull Request

📄 License
This project is licensed under the MIT License.

🌍 Live Demo
🔗 GiftLink App on IBM Cloud
