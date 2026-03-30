# AnythingAI-Assignment
# Task Management App - Backend Developer Intern Assignment

## Tech Stack
- Node.js
- Express.js
- MongoDB
- JWT Authentication
- bcryptjs
- React.js (Vite)
- Swagger / Postman

## Features
- User Registration & Login
- JWT Authentication
- Role-Based Access Control (User/Admin)
- Task CRUD APIs
- Protected Dashboard
- API Validation & Error Handling

## Project Structure
backend/
frontend/

## Backend Setup
1. cd backend
2. npm install
3. Add .env file
4. npm run dev

## Frontend Setup
1. cd frontend
2. npm install
3. npm run dev

## API Endpoints

### Auth
- POST /api/v1/auth/register
- POST /api/v1/auth/login

### Tasks
- POST /api/v1/tasks
- GET /api/v1/tasks
- GET /api/v1/tasks/:id
- PUT /api/v1/tasks/:id
- DELETE /api/v1/tasks/:id

## Authentication Flow
- User registers with hashed password
- User logs in with email/password
- JWT token is generated
- Protected routes require Bearer token

## Database Schema

### User
- name
- email
- password
- role

### Task
- title
- description
- status
- createdBy

## Scalability Notes
- API versioning via /api/v1
- Modular folder structure for future modules
- Can scale horizontally using multiple backend instances
- Load balancing can be introduced with Nginx
- Redis can be used for caching sessions and frequent reads
- MongoDB indexes can improve query performance

## Bonus Implemented
- Morgan logging
- Swagger docs

## Author
Shaik Nayab Rasul
