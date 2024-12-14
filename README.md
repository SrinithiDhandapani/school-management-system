# School Management System

A comprehensive School Management System built using the **MERN stack** (MongoDB, Express, React, Node.js). This project provides a platform for managing student, teacher, and administrative activities efficiently.

## Features

### Admin Features
- Manage students (add, edit, delete, and view details)
- Manage teachers (add, edit, delete, and view details)
- Assign classes and subjects
- Generate reports

### Teacher Features
- View and manage assigned classes
- Track student performance and attendance
- Share study materials

### Student Features
- View personal details and academic performance
- Access study materials
- Submit assignments

## Tech Stack

- **Frontend**: React.js
  - State Management: Redux/Context API
  - UI Framework: Material-UI / Bootstrap
- **Backend**: Node.js, Express.js
- **Database**: MongoDB (Mongoose for schema modeling)
- **Authentication**: JSON Web Tokens (JWT)
- **Others**: Axios, RESTful APIs

## Installation

### Prerequisites
- Node.js installed on your machine
- MongoDB instance running (local or cloud-based, e.g., MongoDB Atlas)

### Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/school-management-system.git
   cd school-management-system
   ```

2. Install dependencies for the backend:
   ```bash
   cd backend
   npm install
   ```

3. Set up environment variables in `backend/.env`:
   ```env
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_secret_key
   ```

4. Start the backend server:
   ```bash
   npm start
   ```

5. Install dependencies for the frontend:
   ```bash
   cd ../frontend
   npm install
   ```

6. Set up environment variables in `frontend/.env`:
   ```env
   REACT_APP_API_URL=http://localhost:5000/api
   ```

7. Start the frontend server:
   ```bash
   npm start
   ```

8. Open your browser and navigate to `http://localhost:3000` to access the application.

## Folder Structure

```
school-management-system/
├── backend/          # Backend code (Node.js, Express)
│   ├── models/       # Mongoose schemas
│   ├── routes/       # Express routes
│   ├── controllers/  # Business logic
│   ├── middleware/   # Middleware (e.g., auth)
│   ├── config/       # Configuration files
│   └── server.js     # Entry point for backend
│
├── frontend/         # Frontend code (React.js)
│   ├── src/
│   │   ├── components/  # Reusable components
│   │   ├── pages/       # Application pages
│   │   ├── redux/       # Redux-related files
│   │   └── App.js       # Entry point for React app
│
├── .gitignore        # Files to be ignored by Git
├── README.md         # Project documentation
└── package.json      # Project metadata
```

