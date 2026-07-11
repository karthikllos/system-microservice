# System Microservice

A lightweight backend microservice responsible for handling authentication, request routing, and service-to-service communication for the internal platform.

## Features

- JWT-based authentication
- REST API endpoints
- Health monitoring
- Docker support
- GitHub Actions CI/CD
- Production deployment pipeline

## Project Structure

```
system-microservice/
├── src/
│   ├── app.py
│   ├── auth.py
│   └── config.py
├── tests/
├── Dockerfile
├── requirements.txt
└── README.md
```

## Local Development

### Install dependencies

```bash
pip install -r requirements.txt
```

### Run the application

```bash
python src/app.py
```

### Run tests

```bash
pytest
```

## Docker

Build the container

```bash
docker build -t system-microservice .
```

Run the container

```bash
docker run -p 8080:8080 system-microservice
```
## CI/CD Pipeline

Every approved pull request triggers:

- Code validation
- Unit tests
- Docker image build
- Push image to the container registry
- Deployment to the production-v3 environment



## Maintainers

Platform Engineering Team
