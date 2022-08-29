### [ssociall.herokuapp.com](https://ssociall.herokuapp.com/)

# MERN Stack Social Media Application

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
- [Troubleshooting](#troubleshooting)
- [Author](#author)
- [License](#license)

## Introduction

This is a site project I've been working on. A full stack social media application made using the MERN stack (MongoDB, Express, React & Nodejs), With this application, where people can connect with other people. Jump right off the [Live App](https://ssociall.herokuapp.com/login) or download the entire [Client source code](https://github.com/abuhuraira24/socialClient), [Server source code](https://github.com/abuhuraira24/socialServer)  and run it on your server. This project is something I've been working on in my free time so I cannot be sure that everything will work out correctly. But I'll appreciate you if can report any issue.

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
REACT_APP_GOOGLE_CLIENT_ID =
REACT_APP_API = http://localhost:5000
REACT_APP_URL = http://localhost:3000

```

To get your Google ClientID for authentication, go to the [credential Page ](https://console.cloud.google.com/apis/credentials) (if you are new, then [create a new project first](https://console.cloud.google.com/projectcreate) and follow the following steps;

- Click Create credentials > OAuth client ID.
- Select the Web application type.
- Name your OAuth client and click Create
- Remember to provide your domain and redirect URL so that Google identifies the origin domain to which it can display the consent screen. In development, that is going to be `http://localhost:3000` and `http://localhost:3000/login`
- Copy the Client ID and assign it to the variable `REACT_APP_GOOGLE_CLIENT_ID` in your .env file

```
$ cd client
$ npm install (to install client-side dependencies)
$ npm start (to start the client)
```

In the second terminal

- cd server and create a .env file in the root of your server directory.
- Supply the following credentials

```
DB_URL =
PORT = 5000
SECRET =
SMTP_HOST =
SMTP_PORT =
SMTP_USER =
SMTP_PASS =

```

Please follow [This tutorial](https://dev.to/dalalrohit/how-to-connect-to-mongodb-atlas-using-node-js-k9i) to create your mongoDB connection url, which you'll use as your DB_URL

```
$ cd server
$ npm install (to install server-side dependencies)
& npm start (to start the server)
```

## Troubleshooting

If you're getting error while trying to send or download PDF,
please run the following in your server terminal.

```
$ npm install html-pdf -g
$ npm link html-pdf
$ npm link phantomjs-prebuilt
```

## Docker

Using docker is simple. Just add the .env contextualized with the docker network.

e.g:

> goes to path "server/.env"

```
DB_URL = mongodb://mongo:27017/arch
PORT = 5000
SECRET =
SMTP_HOST =
SMTP_PORT =
SMTP_USER =
SMTP_PASS =
```

> goes to path "client/.env"

```
REACT_APP_GOOGLE_CLIENT_ID =
REACT_APP_API = http://localhost:5000
REACT_APP_URL = http://localhost
```

And run

```
docker-compose -f docker-compose.prod.yml build

And then

docker-compose -f docker-compose.prod.yml up
```

## Comment

I intend to keep adding more features to this application, so if you like it, please give it a star, that will encourage me to
to keep improving the project.

## Author

- Twitter: [@panshak\_](https://twitter.com/panshak_)
- Github: [@panshak](https://github.com/panshak)
- Linkedin: [@panshak](https://www.linkedin.com/in/panshak/)
- Email: [@ipanshak](mailto:ipanshak@gmail.com)

## License

- This project is [MIT](https://github.com/Panshak/accountill/blob/master/LICENSE.md) licensed.
