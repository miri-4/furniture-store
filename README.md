# Furniture Store

This is a full-stack web application for an online furniture store.  
Users can browse furniture items, add them to a cart, and place orders.

## Preview
![image](https://github.com/user-attachments/assets/e060c00b-c812-4d1c-b9f9-640e8028de8f)

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
### 3. Start the frontend

Since the backend is already deployed to Render, you don't need to run it locally.
The client is pre-configured to use the deployed backend.

Start the React app:
```env
npm run dev
```
Then open your browser at: http://localhost:5173

## 
If you still want to run the backend locally (for development purposes), navigate to the server folder, install dependencies, create a .env file with your MONGO_URI, and run:
```bash
node server
```

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
