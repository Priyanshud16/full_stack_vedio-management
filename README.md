# full_stack_vedio-management

# Video Management Application

## Overview
This is a **MERN stack**-based **Video Management Application** that allows users to:
- **Authenticate** using a username and password.
- **Upload videos** from local storage.
- **View and manage** their own uploaded videos.


## Features
### 1. Authentication & User Access
- Users can **sign up** and **log in** with a username and password.
- Each user can see **only their uploaded videos** after logging in.
- **JWT-based authentication** is implemented for secure access.

### 2. Video Uploading & Storage
- Users can **upload videos** from their local storage.
- **Metadata** (title, description, tags, file size) is stored in **MongoDB**.



### 4. Frontend
- Built with **React.js** for a responsive and user-friendly UI.
- Includes a **video player** for viewing uploaded videos.

## Tech Stack
### **Frontend:**
- React.js
- Tailwind CSS (for styling)
- React Router (for navigation)

### **Backend:**
- Node.js
- Express.js
- MongoDB (for storing user and video data)
- Multer (for handling video uploads)
- JWT (for authentication)



## Setup Instructions
### Prerequisites:
- Node.js and npm installed
- MongoDB installed and running

### **Backend Setup:**
```bash
# Clone the repository
git clone https://github.com/Priyanshud16/full_stack_vedio-management.git
cd server

# Install dependencies
npm install

# Create a .env file and add the following:
MONGO_URI=mongodb+srv://priyanshu:Rd4e4d0edTJQ1LxF@cluster0.rjmy12x.mongodb.net/?retryWrites=true&w=majority&appName=Cluster0
JWT_SECRET=masai
PORT=5000

# Start the server
npm run dev
```

### **Frontend Setup:**
```bash
cd client

# Install dependencies
npm install

# Create a .env file and add the API URL:
REACT_APP_API_URL=http://localhost:5000

# Start the application
npm start
```

## API Endpoints
| Endpoint | Method | Description |
|----------|--------|-------------|
| `/api/auth/signup` | POST | User Registration |
| `/api/auth/login` | POST | User Login |
| `/api/videos/upload` | POST | Upload Video |
| `/api/videos/` | GET | Get All User Videos |
| `/api/videos/:id` | GET | Get Single Video |

## Deployment Instructions
### Docker Setup:
1. Create a **Dockerfile** for both frontend and backend.
2. Use **docker-compose** to define services.
3. Run `docker-compose up` to start the application.

### Cloud Deployment:
- Deploy the frontend using **Vercel** or **Netlify**.
- Deploy the backend using **Render** or **Heroku**.
- Use **MongoDB Atlas** for cloud database hosting.

## Demo & Submission
- **GitHub Repository:** [Insert Link Here]
- **Video Walkthrough:** [Insert Video Link Here]

## License
This project is licensed under the **MIT License**.

