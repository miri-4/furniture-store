# Furniture Store

This is a full-stack web application for an online furniture store.  
Users can browse furniture items, add them to a cart, and place orders.

## Tech Stack

### Client (Frontend):
- React
- Axios
- MUI (Material-UI)
- HTML, CSS

### Server (Backend):
- Node.js
- Express
- MongoDB Atlas

### Deployment:
- Render (for server)
- MongoDB Atlas (cloud database)

## Getting Started

### 1. Clone the project

```bash
git clone https://github.com/miri-4/furniture-store.git
cd furniture-store
```

### 2. Install dependencies
#### Client:

```bash
cd client
npm install
```
#### Server:

```bash
cd ../server
npm install
```
### 3. Set up environment variables
Create a .env file inside the server directory and add:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
```
Make sure to replace your_mongodb_connection_string with your actual MongoDB Atlas URI.

### 4. Start the app
Start the backend:

```bash
cd server
node server
```
Start the frontend:

```bash
cd ../client
npm run dev
```
Open your browser at: http://localhost:5173

## Project Structure
```bash
furniture-store/
├── client/                    # React frontend
│   ├── public/                # Public assets (images, logos)
│   ├── src/                   # Source code
│   │   ├── api/               # Axios service modules
│   │   ├── app/               # Redux store configuration
│   │   ├── assets/            # Static assets (like SVGs)
│   │   ├── components/        # UI components (NavBar, Footer, etc.)
│   │   ├── featurs/           # Redux slices (cart, user)
│   │   ├── pages/             # Route-based pages (Login, Signup, etc.)
│   │   └── utils/             # Utility functions
│   ├── index.html
│   ├── vite.config.js
│   └── package.json
│
├── server/                   # Node.js backend
│   ├── Controllers/          # Logic for orders, products, users
│   ├── Middlewares/          # Middleware functions (auth, file upload)
│   ├── Models/               # Mongoose schemas
│   ├── routers/              # API routes
│   ├── staticFile/images/    # Uploaded product images
│   ├── utils/                # JWT helpers
│   ├── config/               # DB connection config
│   ├── server.js             # Main server entry
│   └── package.json
└── README.md                 # Project overview

```

## Author
Created by Miriam
GitHub: https://github.com/miri-4
