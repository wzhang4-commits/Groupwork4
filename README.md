## Use of Docker

Docker is used in this project to create a consistent and portable environment for running the database. Instead of installing MySQL manually, Docker allows the database to run inside a container with all required configurations already set.

Using Docker Compose, the database is automatically created and initialized using SQL scripts when the container starts. This ensures that anyone who clones the repository can run the project with a single command (`docker compose up`) without worrying about setup issues.

Docker also helps maintain consistency across different machines and simplifies testing and deployment.

## Use of GitHub Actions

GitHub Actions is used to automate parts of the development workflow. It allows tasks such as building, testing, or validating the project to run automatically whenever code is pushed to the repository.

In this project, GitHub Actions can be used to verify that the repository is properly structured and that the project can be built without errors. This automation improves reliability and ensures that changes to the code do not break the system.

Overall, GitHub Actions helps streamline development and maintain code quality.
