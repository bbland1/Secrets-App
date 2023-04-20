# Secrets A Whisper App Clone

![License](https://img.shields.io/github/license/bbland1/Secrets-App?style=plastic)
![Version](https://img.shields.io/github/package-json/v/bbland1/Secrets-App?style=plastic)
![Language](https://img.shields.io/github/languages/top/bbland1/Secrets-App?style=plastic)

This is a simplified version of the Whisper App that focused on setting up authorization and authentication. Using methods that are commonly found on sites today to understand how they are implamented and how there is a difference between authorization and authentication.

A user can set up their own account by using their email and setting a password (that will be hashed and salted) for credentials that will be saved in the database. A user can also use their google account to log in if they don't want to create a new set of credentials. When the user is logged in they are able to see the annonymous secrets shared by others, they can also add a secret themselves.

Deployment: https://pacific-headland-63101.onrender.com

## Requirements
Install all the dependecies of this project by using the [package.json](./package.json). For this project to work you will also need a google developers account allowing you to use the Google OAuth process, and to have [installed Mongo DB] on your computer for local development.

## Built With
* [dotenv](https://www.npmjs.com/package/dotenv)
* Frontend
  * [EJS](https://ejs.co)
  * [Bootstrap](https://getbootstrap.com/docs/4.6/getting-started/introduction/)
* Backend
  * [Express.js](https://expressjs.com)
  * [MongoDB](https://www.mongodb.com)
  * [Mongoose](https://mongoosejs.com)
* Authentication & Authorization
  * [Passport](https://www.passportjs.org)
  * [GoogleOAuth](https://developers.google.com/identity/protocols/oauth2)

### Local Development
1. Download and install the LTS version of [Node.js](https://nodejs.org/en). In this project [nvm](https://www.freecodecamp.org/news/node-version-manager-nvm-install-guide/) was used for the installing of a node version.
2. Set up a google developers account.
3. Download and install mongo db on your computer.
4. Install the project requirements
```shell
npm install
```
4. Create a `env` file based on the `.env.sample` file and change `SECRET_KEY`, `MONGO_DB`, `CLIENT_ID`, `CLIENT_SECRET` to your specifc strings to connect to your database and access the required authorization process with google.
  - Change the  `callbackURL:` within the google strategy for the 2.0 set up to be towards your url
5. Run the app
```shell
node app.js
```

### Deployment
This project was origially deployed with Heroku. While it still could have been deployed there with the removal of their free teir it was moved to [Render](https://render.com). Typically deployment of an Express app would follow the process listed [here](https://render.com/docs/deploy-node-express-app), but this was a migration following the steps [here](https://render.com/docs/migrate-from-heroku). The migration process was also very straight forward and while you will most likely follow typical deployment just incase there is something you would like to migrate to Render yourself.  

### License
See the [LICENSE](./LICENSE) file for license rights and limitations (MIT).
