# Beginner DevOps Todo App

A simple yet practical DevOps project demonstrating Docker containerization, GitHub Actions CI/CD pipelines, and modern deployment practices.

## What You'll Learn

- **Docker**: Create a Dockerfile to containerize a Node.js application
- **GitHub Actions**: Set up automated CI/CD pipelines for testing and deployment
- **DevOps Basics**: Understanding of containerization, automated workflows, and deployment
- **Git & GitHub**: Version control and collaboration best practices

## Project Structure

```
begineer-devops-todo-app/
├── app.js              # Simple Node.js Todo application
├── package.json        # Node.js dependencies and metadata
├── Dockerfile         # Docker configuration for containerization
├── .github/
│  └── workflows/       # GitHub Actions CI/CD workflows
└── README.md          # Project documentation (this file)
```

## Prerequisites

- Git installed on your machine
- Docker installed and running
- Node.js (v14+) for local testing
- GitHub account

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/beginner-devops-todo-app.git
cd beginner-devops-todo-app
```

### 2. Run Locally (Without Docker)

```bash
# Install dependencies
npm install

# Run the application
node app.js
```

The app will be available at `http://localhost:3000`

### 3. Run with Docker

```bash
# Build the Docker image
docker build -t beginner-devops-todo-app .

# Run the container
docker run -p 3000:3000 beginner-devops-todo-app
```

## Key DevOps Concepts in This Project

### Docker
- **Image**: A lightweight, standalone executable package
- **Container**: A running instance of a Docker image
- **Dockerfile**: Instructions to build a Docker image

### CI/CD with GitHub Actions
- Automated testing on every commit
- Automated Docker image building
- Deployment workflows

## File Explanations

### `app.js`
Simple Node.js application with basic todo CRUD operations.

### `Dockerfile`
Configuration file that contains:
- Base image selection
- Dependency installation
- Application setup
- Port exposure

### `.github/workflows/`
YAML files defining automated workflows:
- Test on push/pull request
- Build Docker image
- Push to registry (optional)

## Next Steps to Extend This Project

1. **Add Unit Tests**: Implement test cases and run them in CI/CD
2. **Kubernetes Deployment**: Learn to deploy on Kubernetes
3. **Container Registry**: Push images to Docker Hub or GitHub Registry
4. **Infrastructure as Code**: Use Terraform to manage infrastructure
5. **Monitoring**: Add Prometheus and Grafana for monitoring

## Common Commands

```bash
# View Docker images
docker images

# View running containers
docker ps

# Stop a container
docker stop <container_id>

# View logs
docker logs <container_id>
```

## Learning Resources

- [Docker Documentation](https://docs.docker.com/)
- [GitHub Actions Docs](https://docs.github.com/en/actions)
- [Node.js Official Guide](https://nodejs.org/en/docs/)

## Contributing

Feel free to fork this repository, make improvements, and submit pull requests!

## License

MIT License - See LICENSE file for details

---

**Happy Learning! This project is designed to help beginners understand DevOps concepts in a practical way.**
