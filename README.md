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
- Backend: Node.js, Express, Sequelize (MySQL)
- Frontend: Angular
- Database: MySQL

## Installation

### Prerequisites
- Node.js (v16+)
- MySQL (v8+)
- Angular CLI (v15+)

### Backend Setup
1. Clone the repository
2. Install dependencies:
   ```bash
   cd backend
   npm install
   ```
3. Create a `.env` file based on `.env.example`
4. Set up MySQL database:
   ```bash
   mysql -u root -p
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
   cd frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   ng serve
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

## Running the Application
1. Start backend server:
   ```bash
   cd backend
   npm start
   ```
2. Start frontend development server:
   ```bash
   cd frontend
   ng serve
   ```
3. Access the application at `http://localhost:4200`

## License
MIT License
