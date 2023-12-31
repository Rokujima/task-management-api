# Task Management API

This is a simple Task Management API built using Node.js and Express.js, with MongoDB as the database. It allows you to manage tasks with basic operations such as creating, updating, deleting, and retrieving tasks.

## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

## Features

- Create new tasks with a title, description, and completion status.
- Retrieve a list of all tasks.
- Retrieve a specific task by its ID.
- Update an existing task.
- Delete a task by its ID.
- Uses MongoDB to store task data.

## Getting Started

### Prerequisites

Before you begin, ensure you have met the following requirements:

- Node.js installed
- MongoDB server running locally or a remote MongoDB connection URL

### Installation

1. Clone this repository:

   git clone https://github.com/Rokujima/task-management-api.git

2. Change into the project directory:
    cd task-management-api

3. Install the dependencies:
    npm install

4. Configure the MongoDB connection by editing the .env.sample file to .env file.
    MONGO_URI=
    PORT=

5. Start the server:
    npm run start

### API Endpoints
GET /api/tasks: Retrieve a list of all tasks.
POST /api/tasks: Create a new task.
GET /api/tasks/{id}: Retrieve a task by its ID.
PATCH /api/tasks/{id}: Update a task by its ID.
DELETE /api/tasks/{id}: Delete a task by its ID.

### Testing
To run the scenario tests for this API, follow these steps:

1. Ensure that the MongoDB server is running, or you have configured the connection in config/db.js.

2. Open a terminal and navigate to the project directory.

3. Run the tests using the following command:
   npm test
   
The tests will automatically start and provide feedback on the success or failure of the API endpoints.
