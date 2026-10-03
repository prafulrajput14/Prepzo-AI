# 🚀 Prepzo AI

**Prepzo AI** is an AI-powered interview preparation platform that analyzes a candidate's resume against a target job description, identifies skill gaps, and generates personalized interview preparation strategies.

**Live Demo:** https://prepzo-ai-five.vercel.app/login

---

## 📌 Overview

Prepzo AI is a full-stack AI application designed to help candidates prepare for software engineering interviews.

The platform analyzes a candidate's **resume/profile** against a **target job description** and generates personalized insights, including:

- Candidate-job match analysis
- Skill gap identification
- Resume improvement suggestions
- Technical and behavioral interview questions
- Personalized preparation roadmap
- Role-specific interview strategies

The application combines a **React frontend**, **Node.js/Express backend**, **MongoDB database**, **JWT-based authentication**, and **AI/LLM integration** into a complete full-stack application.

---

## ✨ Key Features

### 🤖 AI-Powered Resume Analysis

- Analyzes candidate resume/profile information
- Identifies relevant skills and experience
- Evaluates alignment with target job requirements
- Provides actionable resume improvement suggestions

### 🎯 Candidate-Job Matching

- Compares candidate skills against job requirements
- Generates a job-match score
- Identifies strengths and skill gaps
- Highlights areas requiring improvement

### 📊 Skill Gap Analysis

- Identifies missing or under-represented skills
- Prioritizes important areas for improvement
- Provides targeted preparation recommendations

### 🧠 AI Interview Preparation

Generates role-specific:

- Technical interview questions
- Behavioral interview questions
- Preparation strategies
- Personalized learning recommendations

### 🗺️ Personalized Preparation Roadmap

- Creates a structured preparation plan
- Prioritizes topics based on identified skill gaps
- Helps candidates focus on role-specific requirements

### 🔐 Authentication & Authorization

- JWT-based authentication
- Protected routes
- Role-based access control
- Secure session handling
- Guest access support

### 🎨 Responsive Dashboard

- Modern React-based interface
- Responsive design
- Interactive preparation dashboard
- Smooth UI animations
- Mobile-friendly experience

---

## 🏗️ System Architecture

```text
                         ┌─────────────────────┐
                         │        User         │
                         └──────────┬──────────┘
                                    │
                                    ▼
                         ┌─────────────────────┐
                         │   React Frontend    │
                         │ Vite + Tailwind CSS │
                         └──────────┬──────────┘
                                    │
                               REST APIs
                                    │
                                    ▼
                         ┌─────────────────────┐
                         │ Node.js + Express   │
                         │     Backend API     │
                         └───────┬───────┬─────┘
                                 │       │
                    ┌────────────┘       └────────────┐
                    ▼                                 ▼
          ┌──────────────────┐              ┌──────────────────┐
          │     MongoDB      │              │   AI / LLM API   │
          │    + Mongoose    │              │    Processing    │
          └──────────────────┘              └────────┬─────────┘
                                                     │
                                                     ▼
                                          ┌────────────────────┐
                                          │     AI Results     │
                                          │ • Match Analysis   │
                                          │ • Skill Gaps       │
                                          │ • Questions        │
                                          │ • Roadmap          │
                                          └────────────────────┘
```

---

## 🔄 Application Workflow

```text
Resume / Candidate Profile
            │
            ▼
Target Job Description
            │
            ▼
Candidate Profile Analysis
            │
            ▼
Job Requirement Analysis
            │
            ▼
Skill Gap Detection
            │
            ▼
Candidate-Job Match Analysis
            │
            ▼
AI Interview Strategy
            │
       ┌────┴────┐
       ▼         ▼
Technical    Behavioral
Questions    Questions
       │         │
       └────┬────┘
            ▼
Personalized Preparation Roadmap
```

---

## 🛠️ Technology Stack

### Frontend

- React.js
- Vite
- Tailwind CSS
- Framer Motion
- Axios

### Backend

- Node.js
- Express.js
- REST APIs

### Database

- MongoDB
- Mongoose

### Authentication & Security

- JSON Web Tokens (JWT)
- Role-Based Access Control (RBAC)
- Protected API routes
- Environment-based secret management

### AI

- Large Language Models (LLMs)
- Prompt Engineering
- AI-powered resume analysis
- AI-generated interview preparation

### Deployment

- Vercel — Frontend
- Render — Backend
- MongoDB Atlas — Database

---

## 📂 Project Structure

```text
Prepzo-AI/
│
├── Backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── services/
│   ├── package.json
│   └── ...
│
├── Frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── ...
│
├── .gitignore
└── README.md
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/prafulrajput14/Prepzo-AI.git
cd Prepzo-AI
```

### 2. Backend Setup

```bash
cd Backend
npm install
```

Create a `.env` file inside the `Backend` directory and configure the required environment variables.

```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
AI_API_KEY=your_ai_api_key
```

Start the backend:

```bash
npm start
```

### 3. Frontend Setup

Open a new terminal:

```bash
cd Frontend
npm install
npm run dev
```

The frontend will start using the Vite development server.

> **Note:** Environment variable names should match the configuration used by the application. Never commit `.env` files, API keys, database credentials, or other secrets to the repository.

---

## 🔑 Environment Configuration

The application requires environment-specific configuration for:

- MongoDB connection
- JWT authentication
- AI/LLM API integration
- Backend API configuration

Sensitive credentials must be stored using environment variables and must never be committed to GitHub.

---

## 🔐 Security

The application incorporates several security practices:

- JWT-based authentication
- Protected routes and APIs
- Role-based authorization
- Environment-based secret management
- Input validation
- Controlled API access
- Separation of frontend and backend responsibilities

---

## 🎯 Core Functional Modules

| Module | Description |
| :--- | :--- |
| **Authentication** | User registration, login, and protected route access |
| **Resume Analysis** | Extracts and analyzes candidate profile and core competencies |
| **Job Analysis** | Parses and processes target role requirements |
| **Match Analysis** | Compares candidate profile against target job criteria |
| **Skill Gap Analysis** | Identifies missing or under-represented technical skills |
| **Interview Generator** | Generates role-specific technical and behavioral questions |
| **Preparation Strategy** | Creates a personalized learning and preparation roadmap |
| **Dashboard** | Interactive analytics view of readiness and preparation results |

---

## 💡 Engineering Concepts Demonstrated

This project demonstrates practical implementation of:

- Full-stack MERN development
- RESTful API design
- Client-server architecture
- JWT authentication
- Role-based authorization
- MongoDB data modeling
- API integration
- AI/LLM integration
- Prompt engineering
- Resume and job-description analysis
- Frontend state management
- Responsive UI development
- Cloud deployment
- Secure application development

---

## 📋 Project Information

| Property | Details |
| :--- | :--- |
| **Project** | Prepzo AI |
| **Domain** | Artificial Intelligence / Full-Stack Development |
| **Architecture** | MERN + AI |
| **Application Type** | AI-powered Full-Stack Platform |
| **Frontend** | React.js |
| **Backend** | Node.js + Express.js |
| **Database** | MongoDB |
| **Authentication** | JWT |
