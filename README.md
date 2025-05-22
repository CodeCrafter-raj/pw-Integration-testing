# pw-Integration-testing
Just a practice repository for integration testing


# 🧪 MERN Integration Testing Demo App

This is a simple MERN stack application built for demonstrating **integration testing** using **Jest**, **Supertest**, and **MongoDB**. The project includes user registration, login, and note creation functionalities with secure authentication.

---

## 📁 Project Structure

/server
├── controllers/ # Route handlers
├── models/ # Mongoose schemas
├── routes/ # Express routes
├── tests/ # Integration tests (Jest + Supertest)
├── server.js # Entry point
├── .env # Environment variables
├── jest.config.cjs # Jest configuration
├── babel.config.cjs # Babel configuration




---

## 🚀 Features

- User Registration & Login (JWT-based auth)
- Create and View Notes
- Integration testing for routes and middleware
- MongoDB database (local or Atlas)

---

## 🛠️ Technologies Used

- **MongoDB** & **Mongoose**
- **Express.js**
- **React.js** (optional frontend if needed)
- **Node.js**
- **Jest** & **Supertest** (for testing)
- **dotenv** for managing environment variables
- **bcryptjs** for password hashing
- **jsonwebtoken** for authentication

---

## 🧑‍💻 Getting Started

### 📦 Install Dependencies

```bash

⚙️ Set Environment Variables
Create a .env file in the server/ directory:
cd server
npm install
MONGO_URI=mongodb://127.0.0.1:27017/testdb
JWT_SECRET=your_jwt_secret
PORT=5000


Run the Server
npm run dev

🧪 Run Integration Tests
npm test


API ENDPOINT
| Method | Endpoint              | Description         | Auth Required |
| ------ | --------------------- | ------------------- | ------------- |
| POST   | `/api/users/register` | Register a new user | ❌             |
| POST   | `/api/users/login`    | Login and get token | ❌             |
| POST   | `/api/notes`          | Create a new note   | ✅ (JWT)       |
| GET    | `/api/notes`          | Get all user notes  | ✅ (JWT)       |

