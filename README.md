# Authentication & Authorization - MySQL, REACT, EXPRESS, NODE.JS, PASSPORT.JS

![Image of HeaderPage]()
A simple Crud Application using nodejs-express-sequelize-mysql.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Things you need to install the software and how to install them

```
Make sure you have node.js  and npm . node v10.16.3 (https://nodejs.org/en/download/)installed
How to install node.js and NPM on windows (https://treehouse.github.io/installation-guides/windows/node-windows.html)
How to install node.js and NPM on mac (https://treehouse.github.io/installation-guides/mac/node-mac.html)
```

```
Make sure you have installed MySQL on your local machine (https://dev.mysql.com/downloads/mysql/)
How to install MySQL (https://dev.mysql.com/doc/mysql-getting-started/en/)
```

```
Make sure you have installed MySQL Benchmark Tool (https://dev.mysql.com/downloads/benchmarks.html)
You only need this to easily manage your database
```

### Installing

A step by step series of examples that tell you how to get a development env running

```
Download or fork this repo

```

```
cd to the root folder

```

open the .env file and provide the following...

```
DB_PASSWORD='the database password you created in MySQL'
DB_USER='your MySQL username'

```

open the db.config.js file in the config folder and provide the following

```
HOST: "localhost",
USER: process.env.DB_USER, // this remain the same
PASSWORD: process.env.DB_PASSWORD, // this remain the same
DB: "the name you gave the scheme you created in the MySQL server you downloaded earlier",
dialect: "mysql", // this remain the same

```

open the server.js file
Find the //database

Anytime you want to drop the whole table simply un-comment

this

```
db.sequelize
.sync({
force: true,
})
.then(() => {
console.log("Drop and Resync Database with { force: true }");
initial();
});
```

and comment this out

```
// db.sequelize
// .sync()


```

Open your terminal

```

type : npm install

```

in the terminal opened for the root folder

```
type : npm start

```

## Deployment

Depending on your deployment platform

## Built With

- [Node](https://nodejs.org/en/download/) - The web framework used
- [Mysql](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwjJxLuPw8rqAhWN3oUKHR83De4Q0gIoATAAegQIAxAI&url=https%3A%2F%2Fdev.mysql.com%2Fdownloads%2F&usg=AOvVaw0sgOa3GBI0b7wNx3SlFMDn) - Used to create local database

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository]().

## Authors

- **Adeola Oni** - _Initial work_ - [Oneil213](https://github.com/oneil213/)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

-
