// README.md
# DevConnector API

A RESTful API built with Node.js, Express, and MongoDB for a basic developer social network application. It supports user authentication, profile management, and posting functionality. This project is suitable as a backend code sample for MLH Fellowship.

## Features

- User registration and login with JWT-based authentication
- Create, read, and update user profiles
- Create and view posts
- Add comments to posts
- Input validation with `express-validator`

## Technologies Used

- Node.js
- Express
- MongoDB with Mongoose
- JWT for authentication
- Bcrypt for password hashing

## Getting Started

### Prerequisites
- Node.js
- MongoDB (local or MongoDB Atlas)

### Installation
```bash
git clone https://github.com/your-username/devconnector-api.git
cd devconnector-api
npm install
```

### Environment Variables
Create a `.env` file in the root directory and add:
```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
PORT=5000
```

### Running the Server
```bash
npm run server
```

### API Endpoints
- `POST /api/users` - Register a user
- `POST /api/auth` - Login user & get token
- `GET /api/auth` - Get logged-in user
- `GET /api/profile/me` - Get logged-in user's profile
- `POST /api/profile` - Create/update profile
- `POST /api/posts` - Create a new post

## Folder Structure
```
.
├── config
│   └── db.js
├── middleware
│   └── auth.js
├── models
│   ├── Post.js
│   ├── Profile.js
│   └── User.js
├── routes
│   ├── auth.js
│   ├── posts.js
│   ├── profile.js
│   └── users.js
├── server.js
└── .env
```

## License
