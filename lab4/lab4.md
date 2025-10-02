https://www.youtube.com/watch?v=gqTg9eX715k

1. What are the main differences between a Docker image and a Docker container?
   
   Docker image is a read-only template used to create Docker containers.
   Docker container is a running instance of a Docker image.

2. Explain how Docker's layered architecture improves efficiency.
   
   Each layer in the Docker image is read-only, and any changes made to the container are stored in a writable layer. Each container has its own writable layer, which allows for isolation and separation of concerns. Changes made to the container do not affect the underlying image. This ensures that each container has its own environment and dependencies.
   
3. Why does each container get its own writable layer?
   
   Each container gets its own writable layer to ensure isolation and separation of concerns. This allows for efficient use of storage space and faster image downloads. Each container has its own environment and dependencies, which ensures that changes made to one container do not affect the others.


4. What are the benefits of using Docker Compose over running containers individually?
   
   Docker Compose allows for easy management of multiple containers. It allows for the definition of container dependencies, networks, and volumes in a single file. This makes it easier to manage and scale applications. Docker Compose is well suited for development environments, as it allows for the definition of multiple containers in a single file.

