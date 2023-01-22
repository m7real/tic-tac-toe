# Tic Tac Toe Game

## Project Definition

The project is an asynchronous multi-player Tic Tac Toe game built using the MERN stack (MongoDB, Express, React, Node.js) and Socket.io for real-time communication. The project also utilizes Firebase for user authentication and database management.

## Features

- User management: Users can log in / register using basic information, email id & username are unique per user, and once logged in, user stays logged in until cache is cleared from the browser.
- Starting an asynchronous game with anyone via their email id: Only one ongoing game with any other user is allowed, and the game can be started with anyone using their email id. As soon as the game is created, the initiator gets the first move, and every player sees X as their piece & O as the other player’s piece in every game.
- Gameplay: Standard 3x3 Tic Tac Toe game, first player to put their piece in 3 consecutive squares wins the game, and the game can be drawn too.
- Home page: As soon as the games are started, a card is created for every game, and these cards are sorted in descending order of their last updated time.
- Mobile web layout is supported

## Technologies

- ReactJS for building the frontend
- Node.js, Express for building the backend API
- MongoDB for database management
- Socket.io for real-time communication
- Firebase for user authentication
- Tailwind CSS for styling

## Architecture

The project is divided into two main folders, the client and server. The client folder contains the React application, and the server folder contains the Node.js API.
The project uses MongoDB for data storage, and the database is connected using Mongoose.
Firebase is used for user authentication, and JWT tokens are used for maintaining the user session.
The frontend and backend communicate using Socket.io for real-time updates.
Next.js is used for server-side rendering

## How to run the code

1. Clone the repository
2. Run npm install in the root directory to install the dependencies for both client and server.
3. Run npm run dev in the root directory to start the development server
4. Run npm run build and npm start inside the client folder to build and start the client.
5. Run npm start inside the server folder to start the server.
6. The application should be running on http://localhost:3000/

## Assumptions

- As the project only supports mobile web layout, the game may not be responsive to other screen sizes.

## Problems Faced

- One of the biggest challenges was to implement real-time communication between the frontend and backend using Socket.io.
- Another challenge was to properly manage the state of the game and the different states it can be in (Won, Drawn, Waiting for other player to play, Waiting for
