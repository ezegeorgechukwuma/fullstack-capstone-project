# 🎁 GiftLink - Gift Sharing Web Application

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Node.js](https://img.shields.io/badge/Backend-Node.js-blue.svg)](https://nodejs.org/)
[![MongoDB](https://img.shields.io/badge/Database-MongoDB-green.svg)](https://www.mongodb.com/)
[![Deployed on IBM Cloud](https://img.shields.io/badge/Deployed-IBM%20Cloud-blue)](https://giftwebsite.1wa78gnru4vq.us-south.codeengine.appdomain.cloud)

---

## 📌 Project Overview

**GiftLink** is a fullstack JavaScript web application that allows users to share and discover gifts. Users can register, post gifts, and search for gifts by name, category, condition, or appropriate age range. It is built using modern web technologies and deployed on IBM Cloud using Docker and Code Engine.

---

## ✨ Features

- 👤 User registration
- 🎁 Add and manage gift listings
- 🔍 Filter gifts by:
  - Name (case-insensitive partial match)
  - Category (e.g., toys, books)
  - Condition (e.g., new, used)
  - Age range (slider)
- 🔐 RESTful API with secure data handling
- 🌐 Fully containerized and deployed to IBM Cloud

---

## 🛠 Tech Stack

| Layer         | Technology                          |
|---------------|--------------------------------------|
| Frontend      | HTML, CSS, JavaScript                |
| Backend       | Node.js, Express.js                  |
| Database      | MongoDB                              |
| API           | RESTful endpoints                    |
| Containerization | Docker                           |
| Cloud Deployment | IBM Cloud, IBM Code Engine       |

---

## 🚀 Setup Instructions

### Prerequisites

- Node.js & npm installed
- MongoDB instance running locally or in the cloud
- Docker (for containerized build)
- IBM Cloud CLI (for deployment)

### Backend Setup

```bash
git clone https://github.com/your-username/giftlink.git
cd giftlink-backend
npm install
npm start
