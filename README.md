Sure! Here's a comprehensive README for a Chat App built with the MERN stack:

---

# Chat App

Chat App is a real-time messaging application built using the MERN stack (MongoDB, Express.js, React, and Node.js). It allows users to create accounts, send and receive messages, and engage in real-time conversations.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

- **Real-time Messaging:** Send and receive messages in real time.
- **User Authentication:** Secure user registration and login.
- **Chat Rooms:** Create and join chat rooms for group conversations.
- **Private Messaging:** Send direct messages to individual users.
- **Responsive Design:** Fully responsive design using React and Bootstrap.

## Technologies Used

- **Frontend:**
  - React
  - Bootstrap
  - Socket.IO Client

- **Backend:**
  - Node.js
  - Express.js
  - MongoDB
  - Socket.IO

- **Other:**
  - JWT for authentication
  - Mongoose for MongoDB interaction

## Installation

Follow these steps to set up the project locally:

### Prerequisites

- Node.js installed on your machine
- MongoDB instance running

### Steps

1. **Clone the repository:**
    ```sh
    git clone https://github.com/techsaurabh-394/chat-app.git
    cd chat-app
    ```

2. **Install dependencies:**
    ```sh
    npm install
    cd client
    npm install
    cd ..
    ```

3. **Set up environment variables:**
    Create a `.env` file in the root directory and add the following:
    ```sh
    MONGO_URI=your-mongodb-uri
    JWT_SECRET=your-jwt-secret
    ```

4. **Run the server:**
    ```sh
    npm run server
    ```

5. **Run the client:**
    Open another terminal window, navigate to the `client` directory, and run:
    ```sh
    npm start
    ```

The application will be running on `http://localhost:3000` for the frontend and `http://localhost:5000` for the backend.

## Usage

### Registering a New User

1. Navigate to `http://localhost:3000`.
2. Click on the "Register" button.
3. Fill out the registration form with your details.
4. Click "Submit" to create your account.

### Logging In

1. Navigate to `http://localhost:3000`.
2. Click on the "Login" button.
3. Enter your credentials and click "Submit".

### Sending Messages

1. After logging in, you will see a list of chat rooms and users.
2. Click on a chat room to join or create a new one.
3. Type your message in the input field and press "Send".

## API Endpoints

### Authentication

- **POST /api/auth/register**
  - Register a new user.

- **POST /api/auth/login**
  - Log in a user.

### Users

- **GET /api/users**
  - Get a list of all users.

- **GET /api/users/:id**
  - Get details of a specific user.

### Messages

- **GET /api/messages**
  - Get a list of all messages.

- **POST /api/messages**
  - Send a new message.

- **GET /api/messages/:roomId**
  - Get messages for a specific chat room.

### Chat Rooms

- **GET /api/rooms**
  - Get a list of all chat rooms.

- **POST /api/rooms**
  - Create a new chat room.

- **GET /api/rooms/:id**
  - Get details of a specific chat room.

## Contributing

We welcome contributions to the Chat App! Here's how you can help:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature-name`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature/your-feature-name`).
6. Open a Pull Request.

