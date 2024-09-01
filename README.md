# ChatU

# Introduction

This repository consists of a Chat Application built with the MERN stack
(MongoDB, Express.js, Node.js, and React.js).

This is a full-stack chat application that can be up and running with just a few steps. Its frontend is built with [Material UI](https://mui.com/material-ui/) running on top of [React](https://react.dev/). The backend is built with [Express.js](https://expressjs.com/) and [Node.js](https://nodejs.org/en). Real-time message broadcasting is developed using [Socket.IO](https://socket.io/).

# Features

This application provides users with the following features:

- **Authentication** using [JWT Tokens](https://jwt.io/).
- A **Global Chat** which can be used by anyone using the application to broadcast
  messages to everyone else.
- A **Private Chat** functionality where users can chat with other users privately.
- **Real-time updates** to the user list, conversation list, and conversation
  messages.

## Screenshots

### Register
![Screenshot 2024-09-01 064008](https://github.com/user-attachments/assets/0e7fc1f7-2f63-4acb-885d-a7d054ec4c91)

### Login
![Screenshot 2024-09-01 063953](https://github.com/user-attachments/assets/76983705-b88a-45e3-988a-8aafe34359b6)

### Global Chat
![Screenshot 2024-09-01 064242](https://github.com/user-attachments/assets/645d90eb-f36b-4f14-a28b-8e317e6f4b8a)

![Screenshot 2024-09-01 070654](https://github.com/user-attachments/assets/918e2a60-f279-4e7e-83d1-821fea73096a)

### Private Chat
![Screenshot 2024-09-01 064332](https://github.com/user-attachments/assets/0eb14af0-f18f-40bf-b84f-a7de21b712cb)

![Screenshot 2024-09-01 070119](https://github.com/user-attachments/assets/452ead9c-1e6e-44db-863e-5eb9e1e6ba79)

# How to use

You can have this application up and running with just a few steps because it has both the frontend and the backend in a single repository. Follow the steps below to do so:

1. Clone this repo  
   ```git clone https://github.com/R-K-Mishra/Chat-Application.git```
2. Once you have the repo, you need to install its dependencies. So using a
   terminal, move into the root directory of the project (```cd ChatU```) and execute ```npm install``` to install the dependencies of the Node.js server and then run 
   ```npm run client-install``` to install the dependencies of the frontend or client. The second command is a custom command that I wrote to simplify the installation process.
3. This application uses MongoDB as its Database. So make sure you have it installed. You can find detailed guide on how to do so [here](https://www.mongodb.com/docs/manual/administration/install-community/). Once installed, make sure that your local MongoDB server is not protected by any kind of authentication. If there is authentication involved, make sure you edit ```mongoURI``` in the ```config/keys.js``` file.  
**NOTE:** Use the ```npm audit fix --force``` command to address any errors or vulnerabilities that may have occurred during the installation of the dependencies.
4. Finally, all you have to do is simply run ```npm run dev```. If this command
   fails, try installing the package [concurrently](https://www.npmjs.com/package/concurrently) globally by running ```npm install -g concurrently``` and then running the ```dev``` command.
5. The frontend of the application will automatically open in your web browser, and you can test it right away.

# Things to note

* The frontend is built using [create-react-app](https://create-react-app.dev/).
* Backend database connections are managed through [Mongoose ORM](https://mongoosejs.com/).
* Code quality is ensured using [ESlint](https://eslint.org/).
* Passwords are securely hashed using the [bcrypt.js](https://www.npmjs.com/package/bcrypt) library before being stored in the database.
* String inputs are validated and sanitized with the help of [validator.js](https://www.npmjs.com/package/validator) library to ensure maximum security.
* User authentication is handled through the [passport](https://www.npmjs.com/package/passport) middleware along with [JWT tokens](https://jwt.io/).


