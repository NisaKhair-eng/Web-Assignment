
 Practical Assignment Summary: Backend To-Do List App

 Objective

The primary goal of this assignment was to develop a simple backend application using Node.js and Express.js that allows users to manage a to-do list. The application provides three core functionalities:

* Add a task
* View all tasks
* Delete a task by ID

These functionalities were implemented through the following API endpoints:

* `POST /addTask`: Adds a new task.
* `GET /tasks`: Retrieves all tasks.
* `DELETE /task/:id`: Deletes a task by its ID.

Tools & Technologies

* Backend Framework**: Express.js (Node.js)
* API Testing**: Postman
* Data Storage**: In-memory array (no database used)

 Implementation Details

The application was built using Express.js, a minimal and flexible Node.js web application framework. The server was set up to handle JSON requests and responses. An in-memory array was utilized to store tasks, eliminating the need for a database.

 API Endpoints:

1. POST /addTask: Accepts a JSON body with a `taskName` property. If the `taskName` is provided, a new task is created with a unique ID and added to the tasks array.

2. GET /tasks: Returns a JSON array of all tasks currently stored in memory.

3. DELETE /task/\:id: Accepts a task ID as a URL parameter. If a task with the given ID exists, it is removed from the tasks array.

Sample Task Structure:

```json
{
  "id": 1,
  "taskName": "Learn Express.js"
}
```

Testing with Postman

Postman was used to test the API endpoints:

* POST /addTask: A POST request was made with a JSON body containing the `taskName`. The response included the newly created task with a unique ID.

* GET /tasks: A GET request was made to retrieve all tasks. The response included a JSON array of all tasks.

* DELETE /task/\:id: A DELETE request was made with a specific task ID. The response indicated whether the deletion was successful.

 Deliverables

* Server File: The complete Express.js server file (`server.js`) containing the implementation of the API endpoints.

* Postman Screenshots: Screenshots demonstrating the functionality of each API endpoint, including request and response examples.

Learning Outcomes
 
This assignment provided hands-on experience in building a RESTful API using Express.js. Key takeaways include:

* Understanding the basics of RESTful API design.
* Gaining proficiency in handling HTTP requests and responses.
* Learning how to test APIs using Postman.
* Gaining insight into in-memory data storage and its limitations.
