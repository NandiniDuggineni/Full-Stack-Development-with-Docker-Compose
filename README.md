# Full-Stack-Development-with-Docker-Compose
how to use Docker Compose to effortlessly run a full stack application composed of:
A React frontend
A Flask backend API
A PostgreSQL database

Why Use Docker Compose for Full Stack Apps?
It lets you define and run multiple containers with a single YAML file.
Simplifies managing services like frontend, backend, and database.
Ensures your environment is consistent across development, testing, and production.
Great for microservice architectures or when your app depends on multiple components.

Step 1: Backend (Flask) Setup
Create a simple Flask API that serves data and connects to PostgreSQL.

Step 2: Frontend (React) Setup
A basic React app that fetches and displays data from the Flask API.

Step 3: Docker Compose Configuration
Here’s a sample docker-compose.yml to spin up all services:

Step 4: Build and Run
Run: docker-compose up --build

This will:
Pull the PostgreSQL image and start the DB container
Build and start your Flask backend
Build and serve the React frontend

Step 5: Networking and API Proxy
Make sure your React app calls the backend correctly. During development, you can add a proxy in your React package.json:

This forwards frontend API requests to Flask backend without CORS issues.

Why This Setup Rocks
Single command to spin up the entire stack — no manual juggling.
Service isolation — each component runs in its own container.
Easy to scale — add more backend instances or database replicas with minor config tweaks.
Perfect starting point for modern full stack development workflows.

Final Thoughts
Using Docker Compose makes managing complex apps a breeze and is a must-know for developers working with multi-service projects.
I hope this helps you get started with containerized full stack apps! Feel free to ask questions or share your experiences below.
Happy coding! 🚀

you can read the deatiled artical here: https://nandiniduggineni.hashnode.dev/simplify-full-stack-development-with-docker-compose
