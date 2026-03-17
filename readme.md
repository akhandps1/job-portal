# 🚀 Job Portal - Full Stack MERN Application

A comprehensive **Job Portal Application** built using the **MERN Stack** (MongoDB, Express.js, React, Node.js). This platform bridges the gap between students seeking opportunities and recruiters looking for talent, offering a seamless, real-time job application experience.

---

## 🔗 Live Demo
- **Frontend Deployed URL:** [Add Vercel Link Here]
- **Backend Deployed URL:** [Add Render Link Here]

---

## ✨ Features

### 👨‍🎓 For Students
- **User Authentication:** Secure Signup/Login with JWT.
- **Job Search:** Advanced filtering by keyword, location, and industry.
- **Apply for Jobs:** One-click application process.
- **Profile Management:** Update profile, skills, and upload **Resume** (PDF/Image).
- **Application Tracking:** Real-time status updates (Pending, Accepted, Rejected).
- **Browse History:** View all applied jobs.

### 🏢 For Recruiters
- **Company Registration:** Register and manage companies.
- **Post Jobs:** Create detailed job listings with requirements and salary.
- **Applicant Management:** View list of applicants for specific jobs.
- **Status Update:** Accept or Reject applications with immediate reflection on the student side.

---

## 🛠️ Tech Stack

### **Frontend**
- **React.js (Vite):** For building a fast and interactive UI.
- **Redux Toolkit:** For efficient global state management (Auth, Jobs, Companies).
- **Tailwind CSS:** For modern, responsive styling.
- **Shadcn UI:** For pre-built, accessible UI components.
- **Axios:** For making HTTP requests.

### **Backend**
- **Node.js & Express.js:** RESTful API architecture.
- **MongoDB & Mongoose:** NoSQL database and schema modeling.
- **JWT (JSON Web Tokens):** For secure authentication and authorization.
- **Bcrypt.js:** For password hashing.
- **Cookie-Parser:** For handling secure HTTP-only cookies.
- **Cors:** For handling Cross-Origin Resource Sharing.

### **Tools & Services**
- **Cloudinary:** For cloud storage of profile pictures and resumes.
- **Multer:** For handling file uploads.
- **Postman:** For API testing.

---

## 📂 Project Structure

```bash
job-portal/
├── backend/                 # Node.js & Express Server
│   ├── controllers/         # API Logic (User, Job, Company, Application)
│   ├── middlewares/         # Auth & File Upload Middlewares
│   ├── models/              # Mongoose Schemas
│   ├── routes/              # API Routes
│   ├── utils/               # DB Connect, Cloudinary Config
│   └── index.js             # Entry Point
│
├── frontend/                # React Vite Client
│   ├── src/
│   │   ├── components/      # Reusable UI Components
│   │   ├── hooks/           # Custom React Hooks
│   │   ├── redux/           # State Slices & Store
│   │   └── App.jsx          # Main App Component
│   └── tailwind.config.js   # Tailwind Configuration
└── README.md
```

## 🚀 Getting Started

Follow these steps to set up the project locally.

### 1. Clone the Repository

```
git clone [https://github.com/your-username/job-portal.git](https://github.com/your-username/job-portal.git)
cd job-portal
```

### 2. Backend Setup

Navigate to the backend folder and install dependencies:

```
cd backend
npm install
```

**Environment Variables:** Create a `.env` file in the `backend` root and add the following:

```
PORT=3000
MONGO_URI=your_mongodb_connection_string
SECRET_KEY=your_jwt_secret_key
CLOUD_NAME=your_cloudinary_cloud_name
API_KEY=your_cloudinary_api_key
API_SECRET=your_cloudinary_api_secret
```

Start the backend server:

```
npm run dev
```

### 3. Frontend Setup

Open a new terminal, navigate to the frontend folder, and install dependencies:

```
cd frontend
npm install
```

Start the frontend development server:

```
npm run dev
```

The application should now be running at `http://localhost:5173`.

---

## 🔌 API Endpoints

### **User Routes** (`/api/v1/user`)

- `POST /register` - Register a new user (Student/Recruiter).
    
- `POST /login` - Login user.
    
- `GET /logout` - Logout user.
    
- `POST /profile/update` - Update profile (Bio, Skills, Resume).
    

### **Job Routes** (`/api/v1/job`)

- `POST /post` - Post a new job (Recruiter only).
    
- `GET /get` - Get all jobs (with search/filter).
    
- `GET /get/:id` - Get job details by ID.
    
- `GET /getadminjobs` - Get jobs posted by the logged-in recruiter.
    

### **Company Routes** (`/api/v1/company`)

- `POST /register` - Register a new company.
    
- `GET /get` - Get all companies registered by the recruiter.
    
- `PUT /update/:id` - Update company details.
    

### **Application Routes** (`/api/v1/application`)

- `GET /apply/:id` - Apply for a specific job.
    
- `GET /get` - Get all jobs applied by the student.
    
- `GET /:id/applicants` - Get all applicants for a specific job (Recruiter).
    
- `POST /status/:id/update` - Update application status (Accept/Reject).
    

---
## 📸 Screenshots

|**Landing Page**|**Job Page**|
|---|---|
|||

|**Admin Dashboard**|**Application Status**|
|---|---|
|||


## 🤝 Contributing

Contributions are welcome!

1. Fork the repository.
    
2. Create a new branch (`git checkout -b feature-name`).
    
3. Commit your changes (`git commit -m 'Add some feature'`).
    
4. Push to the branch (`git push origin feature-name`).
    
5. Open a Pull Request.
    

## 📞 Contact

If you have any questions, feel free to reach out:

- **Name:** Akhand Pratap Singh
    
- **Email:** akhandps2007@gmail.com
    
- **LinkedIn:** [www.linkedin.com/in/akhandps1]
