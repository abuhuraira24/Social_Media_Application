### [ssociall.herokuapp.com](https://ssociall.herokuapp.com/)

# MERN Stack Social Media Application

## [Client](https://github.com/abuhuraira24/socialClient)
## [Server](https://github.com/abuhuraira24/socialServer)
## [SocketIo](https://github.com/abuhuraira24/socketIo_server)


#### Built with the MERN stack (MongoDB, Express, React and NodeJS).
![Invoice](https://res.cloudinary.com/dza2t1htw/image/upload/v1659948547/Screenshot_75_q8cedq.png)
=
## Table of contents

- [Introduction](#introduction)
- [Key Features](#key-features)
- [Technologies used](#technologies-used)
  - [Client](#client)
  - [Server](#server)
  - [Database](#database)
- [Configuration and Setup](#configuration-and-setup)
- [Author](#author)
## Introduction

This is a site project I've been working on. A full stack social media application made using the MERN stack (MongoDB, Express, React & Nodejs), With this application, where people can connect with other people. Jump right off the [Live App](https://ssociall.herokuapp.com/login) or download the entire [Client source code](https://github.com/abuhuraira24/socialClient), [Server source code](https://github.com/abuhuraira24/socialServer), [SocketIo Server soutce code](https://github.com/abuhuraira24/socketIo_server) and run it on your server. This project is something I've been working on in my free time so I cannot be sure that everything will work out correctly. But I'll appreciate you if can report any issue.

![Profile](https://res.cloudinary.com/dza2t1htw/image/upload/v1660057956/Screenshot_78_atazwu.png)

## Key Features

- Email verification  via nodemailer
-Account creation and forgot password via email
- User can create post, upload photos, deletion and update post.
- Real time Comment and like/unlike.
- User can follow and unfollow others.
- User can see tottal followers and others posts
- User registration and Login/logout system.
- Authentication using jsonwebtoken (jwt).

## Technologies used

This project was created using the following technologies.

#### Client

- React JS
- Context API (for managing and centralizing application state)
- React-router-dom (To handle routing)
- Axios (for making api calls)
- Styled Commponents & SCSS Module (for User Interface)
- React toastify  (To display success/error notifications)
- Cloudinary (to allows users to upload their business logo)
- React-google-login (To enable authentication using Google)
- Apollo Clien (to data fetching)

#### Server

- Express
- Mongoose
- JWT (For authentication)
- bcryptjs (for data encryption)
- Nodemailer (for sending invoice via email)
- SocketIo
- GraphQL/Apollo Server
- multer

#### Database

MongoDB (MongoDB Atlas)

## Configuration and Setup

In order to run this project locally, simply fork and clone the repository or download as zip and unzip on your machine.

- Open the project in your prefered code editor.
- Go to terminal -> New terminal (If you are using VS code)
- Split your terminal into two (run the client on one terminal and the server on the other terminal)

In the first terminal

- cd client and create a .env file in the root of your client directory.
- Supply the following credentials

```
REACT_APP_SERVER_URL =
REACT_APP_CLIENT_URL = 
REACT_APP_SOCKETIO_SERVER_URL = 
REACT_APP_CLOUDINRY_UPLOAD_API =

```

```
$ cd client
$ npm install (to install client-side dependencies)
$ npm start (to start the client)
```

In the second terminal

- cd server and create a .env file in the root of your server directory.
- Supply the following credentials

```
MONGODB  = URL
PORT = 5000
AUTH_EMAIL = (to send email via nodemailer)
AUTH_PASS = (nodemailer pass)
SECRET_KEY = 
SECURE = Boolean
SERVICE = gmail
COVER = (default user profile cover photo url)
```

Please follow [This tutorial](https://dev.to/dalalrohit/how-to-connect-to-mongodb-atlas-using-node-js-k9i) to create your mongoDB connection url, which you'll use as your DB_URL

```
$ cd server
$ npm install (to install server-side dependencies)
& npm start (to start the server)
```


## Comment

I intend to keep adding more features to this application, so if you like it, please give it a star, that will encourage me to
to keep improving the project.

## Author

- Twitter: [@abuhuraira\_](https://twitter.com/abuhuraira24)
- Github: [@abuhuraira](https://github.com/abuhuraira24)
- Linkedin: [@abuhuraira](https://www.linkedin.com/in/abu-huraira-34423821b/)
- Email: [@abuhuraira](mailto:devloperabuhuraira@gmail.com)

