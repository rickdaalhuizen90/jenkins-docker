# Jenkins Docker Setup

This repository provides a simple way to set up Jenkins using Docker. Follow these steps to get started:

## Getting Started

1. **Clone Repository:**
   ```bash
   git clone <repository_url>
   cd <repository_directory>
   ```

2. **Install Docker and Docker Compose:**
   Ensure you have Docker and Docker Compose installed on your system.

3. **Customize Jenkins Configuration:**
   Customize the Jenkins configuration to your requirements by modifying the Dockerfile, casc.d, plugins.groovy, and plugins.txt files.

4. **Start Jenkins:**
   Start Jenkins using Docker Compose:
   ```bash
   docker-compose up -d
   ```

5. **Retrieve Admin Password:**
   To retrieve the admin password, you can check the Docker logs:
   ```bash
   docker logs <jenkins_container_id>
   ```
   Look for the line containing the admin password.

## Configuring Jobs

1. **Navigate to Jenkins Dashboard:**
   Open your web browser and go to [http://localhost:8080](http://localhost:8080).

2. **Create a New Job:**
   - Click on "New Item" to create a new job.
   - Choose the type of job you want to create (e.g., Freestyle project, Pipeline).

3. **Configure Job Settings:**
   - Set up build triggers, build steps, and post-build actions as needed.

## Resources

- [Learn Jenkins! Complete Jenkins Course - Zero to Hero](https://www.youtube.com/watch?v=6YZvp2GwT0A&t=11s)
