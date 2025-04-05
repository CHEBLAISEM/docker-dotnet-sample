# docker-dotnet-sample

![CI](https://github.com/CHEBLAISEM/docker-dotnet-sample/actions/workflows/main.yml/badge.svg)

A simple ASP.NET Core web application containerized with Docker and deployed using CI/CD via GitHub Actions.  
Originally inspired by [Docker's .NET Language Guide](https://docs.docker.com/language/dotnet/).

---

## 🧩 Project Highlights

- 🧱 ASP.NET Core (.NET 8) application
- 🐳 Dockerized with multi-stage builds
- 🧪 Unit tests with xUnit
- 🔁 Live reload during dev using Docker Compose Watch
- 🛢️ PostgreSQL integration with persistent volume
- ⚙️ CI/CD pipeline using GitHub Actions
- 🚢 Docker image pushed to Docker Hub on every `main` push

---

## 🚀 Run Locally

```bash
docker compose up --build

Visit: http://localhost:8080


 Run Unit Tests in a Container
docker compose run --build --rm server dotnet test /source/tests


 CI/CD Workflow Summary

This project uses GitHub Actions to:

🔐 Authenticate to Docker Hub using secrets

🧪 Build and test the application with Docker BuildKit

📦 Push the final image to Docker Hub on every push to main

🔗 View workflow file
🔗 Docker Hub Repo
 
Project Structure
.
├── src/              # ASP.NET Core app
├── tests/            # xUnit test project
├── Dockerfile        # Multi-stage Docker build
├── compose.yaml      # Compose setup for app + PostgreSQL
└── .github/
    └── workflows/
        └── main.yml  # GitHub Actions CI/CD


Author
Built and maintained with ❤️ by CHEBLAISEM
