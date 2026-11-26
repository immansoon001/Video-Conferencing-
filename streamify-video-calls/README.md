<h1 align="center">✨ Fullstack Chat & Video Calling App ✨</h1>

![Demo App](/frontend/public/screenshot-for-readme.png)

Highlights:

- 🌐 Real-time Messaging with Typing Indicators & Reactions
- 📹 1-on-1 and Group Video Calls with Screen Sharing & Recording
- 🔐 JWT Authentication & Protected Routes
- 🌍 Language Exchange Platform with 32 Unique UI Themes
- ⚡ Tech Stack: React + Express + MongoDB + TailwindCSS + TanStack Query
- 🧠 Global State Management with Zustand
- 🚨 Error Handling (Frontend & Backend)
- 🚀 Free Deployment
- 🎯 Built with Scalable Technologies like Stream
- ⏳ And much more!

---

## 🧪 .env Setup

### Backend (`/backend`)

```
PORT=5001
MONGO_URI=your_mongo_uri
STEAM_API_KEY=your_steam_api_key
STEAM_API_SECRET=your_steam_api_secret
JWT_SECRET_KEY=your_jwt_secret
NODE_ENV=development
```

### Frontend (`/frontend`)

```
VITE_STREAM_API_KEY=your_stream_api_key
VITE_API_URL=
```

---

## Deploy the frontend to Vercel

Import this repository into Vercel and deploy from the repository root. The root
`vercel.json` builds the Vite frontend and rewrites client-side routes to
`index.html`.

The Express backend is a separate, long-running service and is not deployed by
this Vercel configuration. Deploy `/backend` to a Node.js host, then set
`VITE_API_URL` in Vercel to that backend's URL ending in `/api`. Set
`CLIENT_URL` on the backend to the frontend's exact public origin, for example
`https://your-project.vercel.app`, and configure the backend's other required
environment variables there. For authentication cookies, use frontend and
backend custom domains under the same parent domain.

---

## 🔧 Run the Backend

```bash
cd backend
npm install
npm run dev
```

## 💻 Run the Frontend

```bash
cd frontend
npm install
npm run dev
```
