# Secrets A Whisper App Clone

![License](https://img.shields.io/github/license/bbland1/Secrets-App?style=plastic)
![Version](https://img.shields.io/github/package-json/v/bbland1/Secrets-App?style=plastic)
![State](https://img.shields.io/github/deployments/bbland1/Secrets-App/Production?style=plastic)
![Language](https://img.shields.io/github/languages/top/bbland1/Secrets-App?style=plastic)

*A simplified Whisper App Clone, **Secrets**, users are able to make an account with their email or with their Google account and then view any secrets that have been submitted anonymously by others or submit one themselves.*

- Authentication: Google OAuth & Passport.js 
- Frontend: EJS and Bootstrap
- Backend: Express with Node.js, MongoDB and Mongoose
* Deployment: https://pacific-headland-63101.onrender.com


## Requirements
Install all the dependecies of this project by using the [package.json](./package.json). You will need to run the install command in your terminal after forking and cloning the project.

## Built With
* [dotenv](https://www.npmjs.com/package/dotenv)
* [EJS](https://ejs.co)
* [Express.js](https://expressjs.com)
* [MongoDB](https://www.mongodb.com)
* [Mongoose](https://mongoosejs.com)
* [Passport](https://www.passportjs.org)

### Local Development
1. Download and install the LTS version of [Node.js](https://nodejs.org/en). In this project [nvm](https://www.freecodecamp.org/news/node-version-manager-nvm-install-guide/) was used for the installing of a node version.
2. Install the project requirements
3. Create a `env` file
```shell
npm install
```

**My personal highlights of this project:**
Acutally learning and getting the authentication process to work was really eye opening. In this project we worked through the levels of authentication and understanding how hashing, salting, cookies and OAuth. We started at a very basic just saving the email & password, which obviously wasn't secure but we built on the knowledge of database storage and how to take it from plain text to salted & hashed passwords. It was really intersting to see what we all know is important and how keeping those things secure is done. I felt like I was learning the secret of the internet and I was just so amazed as it worked more and more when we added more layers.

**My struggles while building this:**
Deploying this, I had to take a break as I was trying to figure something things out to get it to work. I asl had some issues with getting the parts that should behind the authentication to be behind them. I was implementing it at first but still anyone could see it which wasn't the person and I needed to review the code thoroughly and slow down.


**What I learned in the process:**
.env files usefulness and a bit more understanding of what cookies are. These was a lot missing in my knowledge of just what cookies can do and the informaiton that the hold. So while learning authentication and learning so many new aspects was really motivating jsut proving that there is always more to learn (not that I thought there wasn't but it is nice to see).
