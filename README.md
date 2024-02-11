
# **Guess The Capital**

Welcome to **Guess The Capital**, a simple and interactive web application that challenges users to guess the capitals of various countries. Test your knowledge and see how many capitals you can correctly identify!

## Table of Contents
- [Description](#description)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Technologies](#technologies)
- [UI](#ui)

## Description

**Guess The Capital** is a web-based game that presents users with a country and prompts them to enter the corresponding capital. The application features a dynamic interface, real-time scoring, and a high score tracker to keep users engaged and challenged. The game leverages a PostgreSQL database to store information about countries and capitals, ensuring a diverse and educational experience.

## Features

- **Real-time Scoring:** Keep track of your current score and see how many capitals you can guess correctly.
- **High Score:** Challenge yourself to beat your highest score and see how well you know the world's capitals.
- **Interactive Interface:** User-friendly interface with animations for correct and incorrect answers.
- **Educational:** Learn the capitals of different countries while playing the game.

## Installation

1. Ensure you have [Node.js](https://nodejs.org/) and [PostgreSQL](https://www.postgresql.org/) installed on your machine.
2. Clone the repository:
 ```bash
 git clone https://github.com/trigunom/Guess-The-Capital.git
 ```
3. Navigate to the project directory:

```bash
cd project-directory
```
4. Install dependencies:
```bash
npm i
```
5. Create a PostgreSQL database named "world" and then create a table named `capitals` as following:

| id [pk]         | country     | capital |
| ----------- | ----------- |---------|

6. Import the provided csv file `capitals.csv` to finsh setting up the table.

7. Update the PostgreSQL connection details in `index.js` to match your local setup:

```
const db = new pg.Client({
  user: "your_username",
  host: "localhost",
  database: "world",
  password: "your_password",
  port: 5432,
});
```

## Usage

1. Start the server:
```bash
npm index.js
```

2. Open your web browser and go to `http://localhost:3000`

3. Start guessing the capitals and enjoy the game!

## Technologies

- **Node.js:** Server-side JavaScript runtime.
- **Express:** Web application framework for Node.js.
- **PostgreSQL:** Open-source relational database.
- **HTML, CSS, EJS:** Front-end technologies for building the user     interface.

## UI

![WenPage] (public/images/screenshot.png)
