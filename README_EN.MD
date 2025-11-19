# Test Task: Real-time 

## Implementation

Why did I end up with three frontend repositories? Initially, I made two frontend versions: React + Firebase and Vue + Pinia + WebSocket using AI. However, I realized that this approach was wrong — the test task is meant to assess the developer's level, so I decided to rewrite the entire frontend completely on my own using React + Redux + WebSocket.

Thus, the main work is in the repository "React-Online-Chat," and the chat logic is fully implemented by me. It is worth noting that the WebSocket connection was implemented with the help of AI, as I had no prior experience working with WebSocket.

1. **Vue version of the chat:**  
   [Online-Chat-Vue](https://github.com/daniarmakyev/Online-Chat-Vue)  
   Built with Vue 3 + Pinia + WebSocket backend.

2. **React version of the chat:**  
   [Online-Chat-React](https://github.com/daniarmakyev/Online-Chat-React)  
   Built with React + Redux Toolkit + Firestore + Firebase.

3. **Backend (Express.js):**  
   [Backend-ExpressJS-Online-Chat](https://github.com/daniarmakyev/Backend-ExpressJS-Online-Chat)  
   Service for managing channels, users, and messages using Express + MongoDB + socket.io.

4. **React version with WebSocket connection:**  
   [React-Online-Chat](https://github.com/daniarmakyev/React-Online-Chat)  
   This version was fully implemented by me, except for WebSocket integration.

---

## Notes

All projects are deployed, but there is an important feature: the backend is hosted on Render, so on the first request it may take about 5 minutes for the server to "wake up." After the first request, it should work normally.

## Links to Sites

- Vue version: https://online-chat-vue.vercel.app/auth
- React version: https://online-chat-rosy.vercel.app/
- Backend Express.js: https://online-chat-backend-jin2.onrender.com/
- React (self-worked): https://react-online-chat-flax.vercel.app/

---

## `.env` Files Configuration (Local Setup)

Below are the variables required for running locally.

---

## 1. Backend (Express.js)

File: `.env`

```env
DB_URL=mongodb+srv://daniarmakyev:danigame002@onlinechat.vbg54ji.mongodb.net/?appName=OnlineChat
PORT=3012
JWT_SECRET=boss123
```

## 2. Frontend (Vue 3)

File: `.env`

```env
VITE_API=http://localhost:3012/
```

## 3. React with Firebase

File: `.env`

```env
VITE_FIREBASE_API_KEY=AIzaSyBg4hMOK57ijze-Ykphjzn_fpmPVSvgAX0
VITE_FIREBASE_AUTH_DOMAIN=onlinechat-b5ee6.firebaseapp.com
VITE_FIREBASE_PROJECT_ID=onlinechat-b5ee6
VITE_FIREBASE_STORAGE_BUCKET=onlinechat-b5ee6.appspot.com
VITE_FIREBASE_MESSAGING_SENDER_ID=660030870738
VITE_FIREBASE_APP_ID=1:660030870738:web:eb1ee94d7f481c71e3c90b
VITE_API=http://localhost:3012/
VITE_SOCKET_URL=http://localhost:3012/
```

## 4. React with WebSocket

File: `.env`

```env
VITE_API=http://localhost:3012/
VITE_SOCKET_URL=http://localhost:3012/
```
