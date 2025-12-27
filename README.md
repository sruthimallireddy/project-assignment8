# To-Do List Application

## Overview
This is a full-stack To-Do List application built with a **Node.js backend** and a **React frontend**.  
The backend manages the API and data storage using MongoDB, while the frontend provides an interactive user interface.

---

## Features
- Create, read, update, and delete to-do items.
- Synchronization of data between frontend and backend.
- Environment variables used for configuration.
- Clean and maintainable code structure.

---

## Setup and Run Locally

### Prerequisites
- Node.js and npm installed
- MongoDB installed and running locally or use MongoDB Atlas

---

### Backend Setup

1. Navigate to the backend directory:
    ```bash
    cd backend
    ```

2. Install dependencies:
    ```bash
    npm install
    ```

3. Create a `.env` file (if not already present) in the backend folder with the following content:
    ```
    MONGO_URI=mongodb://localhost:27017/todoapp
    PORT=5000
    ```

4. Start the backend server:
    ```bash
    npm start
    ```

Backend will run on `http://localhost:5000` by default.

---

### Frontend Setup

1. Navigate to the frontend directory:
    ```bash
    cd frontend
    ```

2. Install dependencies:
    ```bash
    npm install
    ```

3. Start the frontend development server:
    ```bash
    npm start
    ```
    or, if `npm start` does not work, try:
    ```bash
    npm run dev
    ```

4. Open your browser and visit:
    ```
    http://localhost:3000
    ```
    or the URL shown in your terminal.

---

## Environment Variables / Configuration

- `MONGO_URI`: MongoDB connection string.  
- `PORT`: Port for backend server.

**Note:** Do not commit `.env` file with sensitive credentials to the repo.

---

## Challenges Faced and Solutions

- **Connecting Frontend and Backend:**  
  Initially faced CORS and connection issues due to port mismatches. Resolved by configuring the frontend to send API requests to the correct backend URL and enabling CORS in backend.

- **MongoDB Setup:**  
  Had issues installing and running MongoDB locally. Solved by carefully following the official MongoDB installation steps and verifying the service was running before starting the backend.

- **Deployment:**  
  Understanding how to deploy the backend and frontend on separate services (Render and Netlify) and making sure the frontend points to the deployed backend was a learning curve.

---

## How to Deploy (Summary)

- Backend deployed on Render.com with environment variables configured.
- Frontend deployed on Netlify and configured to consume backend API.
- Both apps communicate over internet, not localhost.

---

## Contact

For any questions or issues, please contact [Your Name] at [Your Email].

---

