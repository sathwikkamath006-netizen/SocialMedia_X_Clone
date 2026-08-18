# Social App (MERN)

A full-stack social media app with posts, comments, likes, notifications, and authentication.

## Tech Stack
- Frontend: React (Vite), custom hooks, components, pages
- Backend: Node.js, Express
- Database: MongoDB (Mongoose)
- Auth: JWT (cookie-based)

## Project Structure
backend/
  controllers/   # auth, user, post, notification logic
  db/            # MongoDB connection
  lib/utils/     # token generation
  middleware/    # route protection
  models/        # Mongoose schemas
  routes/        # API routes
  server.js

frontend/
  src/
    components/
    hooks/
    pages/
    utils/
    App.jsx
    main.jsx

## Setup

# install dependencies
cd backend && npm install
cd ../frontend && npm install

# run backend
cd backend && npm run dev

# run frontend
cd frontend && npm run dev

## .env Example (backend root)

PORT=5000
MONGO_URI=mongodb+srv://<user>:<password>@cluster.mongodb.net/socialapp
JWT_SECRET=your_jwt_secret_here
NODE_ENV=development

CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

## Features
- Signup / Login / Logout with JWT auth
- Create, like, comment, delete posts
- Follow/unfollow users
- Real-time-style notifications
- Profile edit & image upload (Cloudinary)
