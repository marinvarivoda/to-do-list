# To-Do List

A to-do list app with an Express backend, MongoDB storage, and a Vue 2 reactive frontend.

## Tech Stack

- **Backend:** Node.js, Express, Mongoose
- **Frontend:** Vue 2 (CDN)
- **Database:** MongoDB / MongoDB Atlas

## Features

- Add tasks
- Display tasks in a reactive list
- Persistent storage in MongoDB

## Prerequisites

- Node.js v14+
- MongoDB Atlas account (or local MongoDB)

## Quick Start

1. **Clone and install**

   ```bash
   npm install
   ```

2. **Configure environment**

   Create a `.env` file in the project root:

   ```
   MONGODB_URI=mongodb+srv://user:password@cluster.mongodb.net/todo-list?retryWrites=true&w=majority
   ```

   Replace with your [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) connection string.

3. **Run**

   ```bash
   npm start
   ```

4. Open [http://localhost:3000](http://localhost:3000)

## API

| Method | Endpoint     | Description   |
| ------ | ------------ | ------------- |
| GET    | `/api/tasks` | Get all tasks |
| POST   | `/api/tasks` | Add a task    |

**POST /api/tasks** — Body: `{ "text": "Task description" }`

## Structure

```
├── server.js       # Express server + API
├── public/
│   └── index.html  # Vue 2 frontend
└── .env            # MongoDB URI (not committed)
```
