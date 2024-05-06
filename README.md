# Shopping-on-the-Dock

## Table of Contents

- [Description](#description)

- [Live-Screen-Recording-of-Application-Functionality](#live-screen-recording-of-application-functionality)

- [Screenshots](#screenshots)

- [Technologies](#technologies)

- [Installation](#installation)

- [Credits](#credits)

- [Features](#features)

- [Usage](#usage)

## Description

This application was created so that internet retail companies can utilize a MySQL database and keep an up to date record of specific categories, products, and tags related to the sale, and inventory of their e-commerce business. This application uses Sequelize to interact with a MySQL database. The use of an ORM (object-relational-mapping) dependency (Sequelize) rather than strictly using MySQL query's helps make this particular projects code more readable and reusable, and helps further the organization of project code through destructuring of larger files into more manageable pieces. This can also help isolate bugs, keeps the code DRY, and makes code more maintainable for future development. This project is just the beginning of a complex back end application and can be interacted with through the use of tools such as Insomnia. My main struggles with building the application had to do with the joining of tables. Specifically the relation of Product belongsToMany Tag and Tag belongsToMany Product.

## Live Screen Recording of Application Functionality



## Screenshots



## Technologies

This application is powered by Node.js (v16.19.1), Express.js (v14.17.1), JavaScript, MySQL, and Sequelize (ORM). It utilizes the node package manager (npm) dependencies sequelize (v5.22.5), mysql2 (v2.3.3), express (v4.17.1), dotenv (v8.6.0), and nodemon (v2.0.3). Also, the Insomnia application was utilized to test the functionality of routes within the program.

![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/express.js-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white)
![Sequelize](https://img.shields.io/badge/Sequelize-52B0E7?style=for-the-badge&logo=Sequelize&logoColor=white)
![Nodemon](https://img.shields.io/badge/NODEMON-%23323330.svg?style=for-the-badge&logo=nodemon&logoColor=%BBDEAD)
![Insomnia](https://img.shields.io/badge/Insomnia-black?style=for-the-badge&logo=insomnia&logoColor=5849BE)

## Installation

1. Clone the repo:
   git clone: https://github.com/Masonmanshark4/Shopping-on-the-Dock.git

2. Open in VS Code. If you do not have VS code you must install it.

3. Using the terminal, install node.js v16. If you have homebrew, the command should look like the following (brew install node@16), however this may vary and the documentation should be consulted.

4. Once node.js v16 is installed, in the terminal, utilize the command npm init -y to initialize and create a package.json where project files will be stored.

5. Next, use the terminal to run the command npm i to install the dependencies associated with this application (developers may need to install dependencies directly from the command line).

   Commands to install each dependency:

   - Command for sequelize will be npm i sequelize
   - Command for mysql2 will be npm i mysql2
   - Command for express will be npm i express@4.17.1
   - Command for dotenv will be npm i dotenv
   - Command for nodemon will be npm i nodemon

6. Next, you will need to make sure you have an added .env file within the root directory of your repository, within which you will pass your environmental variables specifying the database name, your MySQL username, and your MySQL password. This will need to be completed before running the application, and will allow the connection.js file to utilize your environmental variables keeping your sensitive information protected.

7. If you do not have a MySQL account, you will need to create one (see https://dev.mysql.com/doc/mysql-installation-excerpt/5.7/en/).

8. Once all dependencies are installed, you will need to create the database. To do this you will need to navigate to the directory db directory containing the schema.sql file. Once there, you will need to open up a MySQL shell using the command mysql -u root -p, where you will then be prompted to enter you password. Once your password is entered you will be in the MySQL shell.

9. Once in the MySQL shell you will then run the command source schema.sql. This will create the database.

10. Once the database has been created, you will then need to seed the database (this will also create the model structure for the tables within the database). To do this, navigate to the root directory and run the command npm run seed. This needs to be done from the root directory because the .env file lives within the root.

11. Once the database has been seeded, you will then be able to run the command npm start from the root directory to spin up the server.

12. From there, you can utilize applications such as Insomnia to test the functionality of the routes within the program.

## Credits

Credit to my teacher and assistant teacher, Mr. Ragheed and Mr. Torres, for giving me the nessacary guidance to understand the coding languages. Along with Ohio State University for creating the Coding Bootcmap.

## Features

Features of this application include the users ability to manage the backend of their company's e-commerce website through Express routing. The functionality built within the application allows for users to navigate their company's database with GET routes, add and update new catagories, products, and tags to their website with POST and PUT routes, and delete any catagories, products, and tags no longer in use or that may be currently out of stock with DELETE routes.

## Usage

Usage of this application as of now, can be seen through the running and testing of routes with applications like Insomnia or strictly through using a MySQL shell. Once the database has been created, seeded, and the server spun up (see installation section for instructions on how to get the database set up and the server running), users can interact with the database through routing of different api end points.
