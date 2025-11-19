# Тестовое задание: Real-time

Я сделал три репозитория с фронтендом. Почему так получилось? 
---
Изначально я сделал две версии фронтенда React + Firebase и Vue + Pinia + WebSocket с помощью ИИ. Однако я понял, что такой подход неправильный тестовое задание же создано что выявить уровень разработчика, поэтому я решил переписать весь фронтенд полностью самостоятельно на React + Redux + WebSocket.

Таким образом, основная работа в репозитории "React-Online-Chat" и логика чата реализованы полностью мной. Стоит отметить, что подключение WebSocket было выполнено с помощью ИИ, так как у меня ещё не было опыта работы с WebSocket.



1. **React (самостоятельная работа):**  
   [React-Online-Chat](https://github.com/daniarmakyev/React-Online-Chat)  
   Эта версия была выполнена мной полностью самостоятельно, за исключением интеграции WebSocket.
   Иногда сокет может не подключатся в чате надо будет перезапустить страницу.
   
3. **Vue версия чата:**  
   [Online-Chat-Vue](https://github.com/daniarmakyev/Online-Chat-Vue)  
   Сделано на Vue 3 + Pinia + WebSocket backend.

4. **React версия чата:**  
   [Online-Chat-React](https://github.com/daniarmakyev/Online-Chat-React)  
   Сделано на React + Redux Toolkit + Firestore + Firebase.

5. **Backend (Express.js):**  
   [Backend-ExpressJS-Online-Chat](https://github.com/daniarmakyev/Backend-ExpressJS-Online-Chat)  
   Сервис для работы с каналами, пользователями и сообщениями на Express + MongoDB + socket.io.



---

## Примечания

Все проекты задеплоены, но есть важная особенность: бэкэнд был развернут на Render, поэтому при первом запросе может потребоваться около 5 минут для "пробуждения" сервера после 1 запроса он надеюсь будет работать.

## Ссылки на сайты

- React (самостоятельная работа): https://react-online-chat-flax.vercel.app/
- Vue версия: https://online-chat-vue.vercel.app/auth
- React версия: https://online-chat-rosy.vercel.app/
- Backend Express.js : https://online-chat-backend-jin2.onrender.com/

---

## Конфигурация `.env` файлов (локальный запуск)

Ниже описано, какие переменные нужны для локального запуска.

---

## 1. Backend (Express.js)

Файл: `.env`

```env
DB_URL=mongodb+srv://daniarmakyev:danigame002@onlinechat.vbg54ji.mongodb.net/?appName=OnlineChat
PORT=3012
JWT_SECRET=boss123

```

## 2. Frontend (Vue 3)

Файл: `.env`

```env
VITE_API=http://localhost:3012/
```

## 3. React с Firebase

Файл: `.env`

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

## 4. React с websocket

Файл: `.env`

```env
VITE_API=http://localhost:3012/
VITE_SOCKET_URL=http://localhost:3012/
```
