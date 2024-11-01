# WhatsApp Clone Application

This is a WhatsApp-like real-time chat application built with the MERN (MongoDB, Express, React, Node) stack. It includes features such as Google OAuth for authentication, Socket.io for live messaging, and Material-UI for a modern and responsive user interface.

## Table of Contents

- [Features](#features)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Environment Variables](#environment-variables)
- [Available Scripts](#available-scripts)
- [File Structure](#file-structure)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)

---

## Features

- **User Authentication**: Google OAuth2.0 for secure login.
- **Real-Time Messaging**: Built with Socket.io for live chat functionality.
- **Media Sharing**: Allows users to share images and files in chat.
- **Responsive UI**: Uses Material-UI for a consistent, responsive design.
- **MongoDB Storage**: Stores messages and user data securely in MongoDB.

---

## Project Structure

This project has three main components:

1. **Client** - The frontend, built with React and Material-UI.
2. **Server** - The backend, built with Node.js and Express.
3. **Socket** - The Socket.io server, handling real-time communication.

---

## Technologies Used

- **Frontend**: React, Material-UI, Google OAuth
- **Backend**: Node.js, Express, MongoDB, Multer (for file uploads), Socket.io
- **Database**: MongoDB with Mongoose ORM
- **Deployment**: Vercel (Frontend), TBD (Backend & Socket)

---

## Getting Started

### Prerequisites

Make sure you have the following installed:

- [Node.js](https://nodejs.org/)
- [MongoDB](https://www.mongodb.com/try/download/community)
- [Google Cloud Console](https://console.cloud.google.com/) account for OAuth credentials

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/UsmanMalik13/whatsapp-clone.git
    cd whatsapp-clone
    ```

2. Install dependencies for both client and server:

    ```bash
    # For frontend
    cd client
    npm install

    # For backend
    cd ../server
    npm install

    # For socket server
    cd ../socket
    npm install
    ```

3. Set up your environment variables (see [Environment Variables](#environment-variables) below).

4. Start MongoDB.

5. Start the servers:

    ```bash
    # In separate terminals or using a process manager

    # Client
    cd client
    npm start

    # Backend
    cd ../server
    npm start

    # Socket server
    cd ../socket
    npm start
    ```

---

## Environment Variables

Create `.env` files in the `server`, `client`, and `socket` folders with the following variables:

### Server `.env`

```env
PORT=3001
MONGODB_URI=<your-mongodb-uri>
JWT_SECRET=<your-jwt-secret>
GOOGLE_CLIENT_ID=<your-google-client-id>
GOOGLE_CLIENT_SECRET=<your-google-client-secret>
