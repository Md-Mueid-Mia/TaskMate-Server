# TaskMate Server

A robust task management system backend built with Node.js and Express, featuring real-time updates with Socket.IO and secure authentication.

## Live Links

- Frontend: [TaskMate Live](https://taskmate-abb2d.web.app)
- Backend: [TaskMate API](https://task-mate-server-ashen.vercel.app)

## Technologies Used

- **Runtime Environment:** Node.js
- **Framework:** Express.js
- **Database:** MongoDB
- **Real-time Communication:** Socket.IO
- **Authentication:** JWT (JSON Web Tokens)
- **Security:** 
  - CORS
  - Cookie Parser
  - Morgan Logger
  - Secure HTTP Headers

## Dependencies

```json
{
  "cookie-parser": "^1.4.6",
  "cors": "^2.8.5",
  "dotenv": "^16.4.1",
  "express": "^4.18.2",
  "jsonwebtoken": "^9.0.2",
  "mongodb": "^6.3.0",
  "morgan": "^1.10.0",
  "socket.io": "^4.7.4"
}
```

## Installation Steps

1. Clone the repository:
```bash
git clone https://github.com/yourusername/TaskMate-Server.git
cd TaskMate-Server
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file in the root directory:
```env
PORT=5000
DB_USER=your_mongodb_username
DB_PASS=your_mongodb_password
ACCESS_TOKEN_SECRET=your_jwt_secret
NODE_ENV=development
```

4. Start the development server:
```bash
npm run dev
```

## Features

- 🔐 Secure JWT-based authentication
- 📊 CRUD operations for tasks
- 🔄 Real-time updates using Socket.IO
- 🎯 Task categorization
- 📱 RESTful API endpoints
- ⚡ Fast and efficient MongoDB queries
- 🛡️ Middleware for request validation

## API Endpoints

### Authentication
- `POST /jwt` - Generate JWT token
- `GET /logout` - Clear authentication

### Tasks
- `GET /tasks/:email` - Get user's tasks
- `POST /tasks` - Create new task
- `PUT /tasks/:id` - Update task
- `PATCH /tasks/:id` - Partial update task
- `DELETE /tasks/:id` - Delete task

### Users
- `POST /users` - Create new user
- `GET /users` - Get all users

## Environment Setup

Make sure you have:
- Node.js (v14 or higher)
- MongoDB Atlas account
- npm or yarn package manager

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.