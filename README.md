
### Context
You are a DevOps engineer working on a new web application that uses a Python Flask API backend and a Redis cache. You've been tasked with containerizing this application using Docker and defining the multi-container environment using Docker Compose.

### Objective
Create a `docker-compose.yml` file that:

1. Defines two services: one for the Flask API and another for the Redis cache.
2. Uses multi-stage builds for the Flask API to minimize the image size.
3. Utilizes environment variables to pass configurations to your services.
4. Mounts volumes to persist data and improve development experience.
5. Uses networks to isolate and secure communication between services.
6. Ensures the Flask API waits for the Redis service to be fully operational before starting.

### Constraints
- Make sure to use version `3` or above for the Docker Compose file format.
- Follow best practices for Dockerfile and Compose file design (e.g., avoid using the `root` user, use `.dockerignore`, etc.)
- Your services should restart automatically if they fail.

### Bonus
- Use overrides (`docker-compose.override.yml`) to manage settings that are specific to a development environment.
- Implement a healthcheck for your services.

### Deliverables
- The `docker-compose.yml` file.
- Any additional Dockerfiles or script files used.
- A README outlining:
  - How to bring up and down the environment.
  - How to scale services.
  - Any design choices or assumptions you made.
