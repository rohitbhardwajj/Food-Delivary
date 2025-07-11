# 🍽️ DineDocker – Dockerized Food Delivery App

**DineDocker** is a full-stack Food Delivery Web App built with the **MERN Stack** (MongoDB, Express.js, React.js, Node.js) and fully containerized using **Docker** and **Docker Compose**. This project is designed to demonstrate modern **DevOps practices** such as containerization, orchestration, environment management, and scalable deployment.

---

## ✨ Features

✅ User Signup/Login with JWT Authentication  
✅ Browse Food Items and Place Orders  
✅ Admin Dashboard for Managing Items  
✅ Secure Payment Gateway with Stripe (Test Mode)  
✅ Frontend & Backend are Dockerized  
✅ Docker Compose for multi-container orchestration  
✅ Environment variables via `.env` file  
✅ MongoDB Atlas integration  
✅ Deployed using AWS EC2 Instance

---

## 🚀 Technologies Used

| Part        | Tech Stack                        |
|-------------|------------------------------------|
| 🧑‍🎨 Frontend | React + Vite                     |
| 🧠 Backend   | Node.js + Express                 |
| 🗃️ Database  | MongoDB (Atlas)                   |
| 🔐 Auth      | JWT + bcrypt                      |
| 💳 Payments  | Stripe API                        |
| 🐳 DevOps    | Docker, Docker Compose            |

---

## 📁 Project Structure

DineDocker/
├── frontend/ # React frontend
│ ├── Dockerfile
│ └── src/
├── backend/ # Node.js backend
│ ├── Dockerfile
│ ├── routes/
│ ├── controllers/
│ ├── config/
│ └── server.js
├── docker-compose.yaml
├── README.md
└── .gitignore



### 📄 `./backend/.env`
Create a `.env` file in the `backend` folder with the following content:

```env
JWT_SECRET=your_super_secret_key
SALT=10
MONGO_URL=mongodb+srv://<username>:<password>@cluster.mongodb.net/food-app
STRIPE_SECRET_KEY=sk_test_xxxxxxxxxxxxxxxxxxx
FRONTEND_URL=http://localhost:5173



🐳 How to Run Locally with Docker
1️⃣ Clone the Project
bash
Copy
Edit
git clone https://github.com/yourusername/DineDocker.git
cd DineDocker
2️⃣ Create .env inside ./backend
Refer to the sample above 👆

3️⃣ Build and Run the Containers
bash
Copy
Edit
docker-compose up --build
4️⃣ Visit in Browser
Frontend: http://localhost:5173

Backend API: http://localhost:5000

