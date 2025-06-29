# Blog-App

A full stack blogging platform built with React for the front‑end and Express + MongoDB for the back‑end. The app supports authentication, creating posts with image uploads and viewing posts from all users.

## Prerequisites

- **Node.js** v16 or later
- **npm**
- **MongoDB** instance (local or remote)

## Installation

1. **Backend dependencies**
   ```bash
   npm install
   ```
2. **Frontend dependencies**
   ```bash
   cd client
   npm install
   cd ..
   ```

## Configuration

Create a `.env` file in the project root with the following variables:

```env
MONGO_URI=<your Mongo connection string>
JWT_SECRET=<any secret string>
```

## Running the app

Start the API and the React client in separate terminals.

### Backend (http://localhost:4000)
```bash
npx nodemon api/index.js
# or
node api/index.js
```

### Frontend (http://localhost:3000)
```bash
cd client
npm start
```

Open `http://localhost:3000` in your browser to use the application.

## Testing

Inside the `client` directory you can run the React tests:
```bash
npm test
```

## Project structure

- `api/` – Express server and Mongoose models
- `client/` – React application (Create React App + Tailwind)
- `api/uploads/` – Uploaded images served from `/uploads`

## Features

- User registration and login with JWT authentication
- Create, edit and view blog posts
- Upload and display images for posts
- Styled with Tailwind CSS
