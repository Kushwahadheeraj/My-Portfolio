# My Portfolio

A full-stack personal portfolio application built with **React.js, Vite, Node.js, Express.js, MongoDB, Redux Toolkit, Tailwind CSS, and Cloudinary**.

The project consists of three separate applications:

* **Portfolio** – Public-facing personal portfolio website
* **Dashboard** – Protected admin panel for managing portfolio content
* **Server** – REST API and backend services

The admin can manage projects, skills, software applications, timeline entries, profile information, messages, and authentication from the dashboard.

---

## 🚀 Features

### 🌐 Public Portfolio

* Responsive personal portfolio website
* Dynamic user profile
* Hero section with animated typewriter
* About section
* Skills with proficiency levels
* Experience and education timeline
* Projects showcase
* Individual project details page
* Software applications and tools section
* Resume link
* GitHub and social media links
* Contact form
* Dark mode support

### 🔐 Admin Dashboard

* Secure login and logout
* JWT-based authentication
* Protected dashboard
* Profile management
* Update password
* Forgot password functionality
* Reset password functionality
* Add, update, view and delete projects
* Add and manage skills
* Update skill proficiency
* Add and manage software applications
* Add and manage timeline entries
* View and delete contact messages
* Upload images and files using Cloudinary

### ⚙️ Backend

* RESTful API architecture
* Express.js server
* MongoDB database
* Mongoose ODM
* JWT authentication
* HTTP-only authentication cookies
* Password hashing with bcrypt
* Password reset using email
* Cloudinary media storage
* File upload support
* Centralized error handling
* CORS configuration

---

# 🛠 Tech Stack

## Frontend

### Portfolio

* React.js
* Vite
* React Router DOM
* Redux Toolkit
* React Redux
* Axios
* Tailwind CSS
* React Toastify
* Lucide React
* React Simple Typewriter

### Admin Dashboard

* React.js
* Vite
* React Router DOM
* Redux Toolkit
* React Redux
* React Hook Form
* Zod
* Axios
* Tailwind CSS
* Radix UI
* Lucide React
* React Toastify

## Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* JWT
* bcrypt
* Cloudinary
* Nodemailer
* express-fileupload
* cookie-parser
* CORS
* dotenv

---

# 📁 Project Structure

```text
My-Portfolio/
│
├── dashboard/
│   ├── src/
│   │   ├── components/
│   │   │   └── ui/
│   │   │
│   │   ├── pages/
│   │   │   ├── sub-components/
│   │   │   ├── LoginPage.jsx
│   │   │   ├── HomePage.jsx
│   │   │   ├── ForgotPassword.jsx
│   │   │   ├── ResetPassword.jsx
│   │   │   ├── ManageProjects.jsx
│   │   │   ├── ManageSkills.jsx
│   │   │   ├── ManageTimeline.jsx
│   │   │   ├── UpdateProject.jsx
│   │   │   └── ViewProject.jsx
│   │   │
│   │   ├── store/
│   │   │   ├── slices/
│   │   │   └── store.js
│   │   │
│   │   ├── App.jsx
│   │   └── main.jsx
│   │
│   ├── package.json
│   └── vite.config.js
│
├── portfolio/
│   ├── src/
│   │   ├── components/
│   │   │   └── ui/
│   │   │
│   │   ├── pages/
│   │   │   ├── miniComponents/
│   │   │   │   ├── Hero.jsx
│   │   │   │   ├── About.jsx
│   │   │   │   ├── Skills.jsx
│   │   │   │   ├── Timeline.jsx
│   │   │   │   ├── Protfolio.jsx
│   │   │   │   ├── MyApps.jsx
│   │   │   │   ├── Contact.jsx
│   │   │   │   └── Footer.jsx
│   │   │   │
│   │   │   ├── Home.jsx
│   │   │   └── ProjectView.jsx
│   │   │
│   │   ├── store/
│   │   ├── App.jsx
│   │   └── main.jsx
│   │
│   ├── package.json
│   └── vite.config.js
│
├── server/
│   ├── config/
│   │   └── config.env
│   │
│   ├── controller/
│   │   ├── messageController.js
│   │   ├── projectController.js
│   │   ├── skillController.js
│   │   ├── softwareApplicationController.js
│   │   ├── timelineController.js
│   │   └── userController.js
│   │
│   ├── database/
│   │   └── database.js
│   │
│   ├── middlewares/
│   │   ├── auth.js
│   │   ├── catchAsyncErrors.js
│   │   └── errors.js
│   │
│   ├── models/
│   │   ├── messageModel.js
│   │   ├── projectModel.js
│   │   ├── skillModel.js
│   │   ├── softwareApplicationModel.js
│   │   ├── timelineModel.js
│   │   └── userModel.js
│   │
│   ├── routes/
│   │   ├── messageRouter.js
│   │   ├── projectRouter.js
│   │   ├── skillRouter.js
│   │   ├── softwareApplicationRouter.js
│   │   ├── timelineRouter.js
│   │   └── userRouter.js
│   │
│   ├── utils/
│   │   ├── jwtToken.js
│   │   └── sendEmail.js
│   │
│   ├── server.js
│   └── package.json
│
└── README.md
```

---

# ⚙️ Installation

## 1. Clone the Repository

```bash
git clone <your-repository-url>
```

```bash
cd My-Portfolio
```

---

# 🖥️ Backend Setup

Navigate to the server directory:

```bash
cd server
```

Install dependencies:

```bash
npm install
```

Create the following directory:

```text
server/config
```

Inside it, create:

```text
config.env
```

Example configuration:

```env
PORT=4000

MONGO_URL=your_mongodb_connection_string

JWT_SECRET_KEY=your_jwt_secret
JWT_EXPIRES=7d

PORTFOLIO_URL=http://localhost:5173
DASHBOARD_URL=http://localhost:5174

CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret

SMTP_HOST=your_smtp_host
SMTP_PORT=your_smtp_port
SMTP_SERVICE=your_smtp_service
SMTP_MAIL=your_email
SMTP_PASSWORD=your_email_password
```

Start the development server:

```bash
npm run dev
```

The backend will run on:

```text
http://localhost:4000
```

---

# 🌐 Portfolio Setup

Open a new terminal and navigate to the portfolio folder:

```bash
cd portfolio
```

Install dependencies:

```bash
npm install
```

Create a `.env` file:

```env
VITE_REACT_APP_BACKEND_URL=http://localhost:4000
```

Start the development server:

```bash
npm run dev
```

The portfolio will typically run on:

```text
http://localhost:5173
```

---

# 📊 Dashboard Setup

Open another terminal:

```bash
cd dashboard
```

Install dependencies:

```bash
npm install
```

Create a `.env` file:

```env
VITE_REACT_APP_BACKEND_URL=http://localhost:4000
```

Start the dashboard:

```bash
npm run dev
```

If the portfolio is already running on port `5173`, Vite will usually assign another available port such as:

```text
http://localhost:5174
```

---

# 🔑 Authentication

The application uses:

* JWT authentication
* Cookies
* bcrypt password hashing
* Protected API routes

Protected routes require the authenticated user cookie.

Examples include:

```text
GET    /api/v1/user/me
GET    /api/v1/user/logout
POST   /api/v1/project/add
PUT    /api/v1/project/update/:id
DELETE /api/v1/project/delete/:id
POST   /api/v1/skill/add
POST   /api/v1/timeline/add
GET    /api/v1/message/getall
```

---

# 📡 API Endpoints

## User API

Base URL:

```text
/api/v1/user
```

| Method | Endpoint                 | Description            |
| ------ | ------------------------ | ---------------------- |
| POST   | `/register`              | Register user          |
| POST   | `/login`                 | Login user             |
| GET    | `/logout`                | Logout user            |
| GET    | `/me`                    | Get authenticated user |
| PUT    | `/me/profile/update`     | Update profile         |
| PUT    | `/password/update`       | Update password        |
| GET    | `/portfolio/me`          | Get portfolio profile  |
| POST   | `/password/forgot`       | Request password reset |
| PUT    | `/password/reset/:token` | Reset password         |

---

## Project API

Base URL:

```text
/api/v1/project
```

| Method | Endpoint      | Description        |
| ------ | ------------- | ------------------ |
| POST   | `/add`        | Add project        |
| GET    | `/getall`     | Get all projects   |
| GET    | `/get/:id`    | Get single project |
| PUT    | `/update/:id` | Update project     |
| DELETE | `/delete/:id` | Delete project     |

Projects support:

* Project title
* Description
* GitHub repository link
* Live project link
* Technology stack
* Technologies
* Deployment information
* Project banner image

Project images are uploaded to Cloudinary.

---

## Skill API

Base URL:

```text
/api/v1/skill
```

| Method | Endpoint      | Description              |
| ------ | ------------- | ------------------------ |
| POST   | `/add`        | Add skill                |
| GET    | `/getall`     | Get all skills           |
| PUT    | `/update/:id` | Update skill proficiency |
| DELETE | `/delete/:id` | Delete skill             |

Each skill contains:

* Title
* Proficiency
* SVG or image

---

## Software Application API

Base URL:

```text
/api/v1/application
```

| Method | Endpoint      | Description              |
| ------ | ------------- | ------------------------ |
| POST   | `/add`        | Add software application |
| GET    | `/getall`     | Get all applications     |
| DELETE | `/delete/:id` | Delete application       |

---

## Timeline API

Base URL:

```text
/api/v1/timeline
```

| Method | Endpoint      | Description              |
| ------ | ------------- | ------------------------ |
| POST   | `/add`        | Add timeline entry       |
| GET    | `/getall`     | Get all timeline entries |
| DELETE | `/delete/:id` | Delete timeline entry    |

Timeline entries include:

```text
Title
Description
From
To
```

---

## Message API

Base URL:

```text
/api/v1/message
```

| Method | Endpoint      | Description          |
| ------ | ------------- | -------------------- |
| POST   | `/send`       | Send contact message |
| GET    | `/getall`     | Get all messages     |
| DELETE | `/delete/:id` | Delete message       |

The public portfolio contact form stores messages in MongoDB.

---

# 🗄️ Database Models

The project uses the following MongoDB collections:

```text
User
Project
Skill
SoftwareApplication
Timeline
Message
```

---

# ☁️ Cloudinary Integration

Cloudinary is used for storing:

* User avatar
* Resume
* Project banner images
* Skill icons
* Software application icons

The backend uploads files using `express-fileupload` and stores the Cloudinary `public_id` and secure URL in MongoDB.

---

# 📦 Available Commands

## Portfolio

```bash
npm run dev
```

Run the development server.

```bash
npm run build
```

Create a production build.

```bash
npm run preview
```

Preview the production build.

```bash
npm run lint
```

Run ESLint.

---

## Dashboard

```bash
npm run dev
```

Run the dashboard development server.

```bash
npm run build
```

Create a production build.

```bash
npm run preview
```

Preview the production build.

```bash
npm run lint
```

Run ESLint.

---

## Backend

```bash
npm run dev
```

Run the backend with Nodemon.

```bash
npm start
```

Run the backend in production mode.

---

# 🔒 Environment Variables

The following sensitive files should not be committed to Git:

```text
server/config/config.env
portfolio/.env
dashboard/.env
```

A recommended `.gitignore`:

```gitignore
node_modules/
dist/
.env
.env.*
config/
*.log
```

---

# 🚀 Production Deployment

The application can be deployed as three services:

### Backend

Deploy the Express server to:

* Render
* Railway
* Hostinger VPS
* AWS
* DigitalOcean

### Portfolio Frontend

Build the application:

```bash
npm run build
```

Deploy the generated `dist` folder to:

* Vercel
* Netlify
* Hostinger
* Cloudflare Pages

### Dashboard

Build:

```bash
npm run build
```

Deploy separately and update:

```env
DASHBOARD_URL=https://your-dashboard-domain.com
```

Also update the frontend backend URL:

```env
VITE_REACT_APP_BACKEND_URL=https://your-api-domain.com
```

Update backend CORS variables:

```env
PORTFOLIO_URL=https://your-portfolio-domain.com
DASHBOARD_URL=https://your-dashboard-domain.com
```

---

# 🧑‍💻 Author

**Dheeraj Kushwaha**

Full Stack Developer

---

# ⭐ Future Improvements

* [ ] Remove hardcoded portfolio user ID and use a configurable user/profile system
* [ ] Add multiple portfolio support
* [ ] Add project categories and filtering
* [ ] Add project pagination
* [ ] Add image optimization
* [ ] Add API validation using Zod or Joi
* [ ] Add rate limiting
* [ ] Add Helmet security middleware
* [ ] Add automated tests
* [ ] Add Docker support
* [ ] Add CI/CD pipeline
* [ ] Add admin role-based authorization
* [ ] Add analytics dashboard
* [ ] Add email notifications for contact messages

---

## 📄 License

This project is intended for personal portfolio and educational use.

Feel free to customize and extend it according to your requirements.
