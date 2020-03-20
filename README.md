# Docker
Epitech Third Year Project, DevOps project, Docker

This project aims to teach you the basics of containerization using docker and docker-compose.
The application you are working on during this project is a simple poll web application.
Poll is a Python Flask web application that gathers the votes to push them into a Redis queue.
The Java Worker consumes the votes stored in the Redis queue, then pushes it into a PostgreSQL database.
Finally, the Node.js Result web application fetches the votes from the DB and displays the result.
