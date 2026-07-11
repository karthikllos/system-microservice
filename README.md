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

Every approved pull request to the `main` branch triggers:

1. Code validation
2. Unit tests
3. Docker image build
4. Image push to registry
5. Production deployment

## Maintainers

Platform Engineering Team
