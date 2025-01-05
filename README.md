# Student Management System

A comprehensive system for managing student details, courses, modules, and exam results.

## Features
- Student registration and management
- Course and module management
- Exam result tracking
- Report generation in Excel format
- RESTful API backend
- Angular-based frontend

## Technologies
- Backend: Node.js, Express, Sequelize
- Frontend: Angular
- Database: PostgreSQL

## Installation

### Prerequisites
- Node.js (v16+)
- PostgreSQL (v12+)
- Angular CLI (v15+)

### Backend Setup
1. Clone the repository
   ```bash
   git clone --recursive https://github.com/your-username/student-management-system.git
   ```
2. Install dependencies:
   ```bash
   cd backend
   npm install
   ```
3. Create a `.env` file based on `.env.example`
   ```bash
   cp ../.env.example .env
   ```
4. Set up PostgreSQL database:
   ```bash
   psql -u root -p
   CREATE DATABASE student_management;
   ```
5. Run migrations:
   ```bash
   npx sequelize-cli db:migrate
   ```
6. Start the server:
   ```bash
   npm start
   ```

### Frontend Setup
1. Navigate to frontend directory:
   ```bash
   cd ..
   cd frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm start
   ```

## API Documentation

### Student Endpoints
- `POST /api/students` - Create new student
- `GET /api/students` - Get all students
- `GET /api/students/:id` - Get student by ID
- `PUT /api/students/:id` - Update student
- `DELETE /api/students/:id` - Delete student

### Course Endpoints
- `POST /api/courses` - Create new course
- `GET /api/courses` - Get all courses
- `GET /api/courses/:id` - Get course by ID
- `PUT /api/courses/:id` - Update course
- `DELETE /api/courses/:id` - Delete course

### Result Endpoints
- `POST /api/results` - Add exam result
- `GET /api/results/student/:id` - Get results by student ID
- `GET /api/results/export` - Export results to Excel

## License
MIT License

