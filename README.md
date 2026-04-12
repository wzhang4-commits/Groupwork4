### GitHub Actions 

We are utilizing GitHub Actions as a means to automate aspects of our development workflow. In particular, the actions allow us to run certain processes (e.g. building/validating our project) automatically each time we commit/push changes to our repository.

In this project, we have configured GitHub actions as a way to verify that our repository structure is correct and that our docker configuration files have been validated. Doing this at the beginning of a project helps identify errors before they occur and ensures that our project continues to work after any updates.

Through these automated processes, GitHub actions create a way to increase the overall efficiency and quality of our code. Additionally, github actions provide us with a form of continuous integration, making it much simpler for us to manage and track changes made during the course of our development workflow.

## Using Docker

This project leverages Docker technology in order to define an identical environment for the purposes of running the database system. By providing all required dependencies, Docker allows the database to operate within a container rather than manually setting up MySQL on various computers.

Docker Compose is responsible for creating and initializing the MySQL container upon starting the project. During the initialization of the container, the SQL scripts located in the `init-db` directory will be run in order to create the necessary tables and insert sample data into the database.

As a result, anyone who chooses to clone this repository will be able to reproduce the same environment simply by executing one command, `docker compose up`, to start the database. In addition, utilizing Docker provides improved reliability of the database, assists with testing, and ensures consistency between development environments.
