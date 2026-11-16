# DevOps Deployment Dashboard — Docker & Nginx

A beginner-friendly DevOps portfolio project demonstrating how to build, version, and deploy a static website using Docker and Nginx.

## Project Features

- Custom HTML, CSS, and JavaScript dashboard
- Docker image versioning (v1, v2, v3)
- Nginx Alpine as the base image
- Interactive deployment details button
- Multiple containers running on separate host ports

## Technology Stack

- HTML5
- CSS3
- JavaScript
- Docker
- Nginx
- Ubuntu Linux
- Git and GitHub

## Docker Images

| Image | Version |
|---|---|
| my-docker-website | v1 |
| my-docker-website | v2 |
| my-docker-website | v3 |

## Deployment Ports

| Version | Host Port | Container Port |
|---|---:|---:|
| v1 | 8082 | 80 |
| v2 | 8083 | 80 |
| v3 | 8084 | 80 |

## Run the Latest Version

Build the Docker image:

```bash
sudo docker build -t my-docker-website:v3 .
```

Run the container:

```bash
sudo docker run -d --name my-docker-website-v3 -p 8084:80 my-docker-website:v3
```

Check running containers:

```bash
sudo docker ps
```

Open the dashboard:

```text
http://localhost:8084
```

## Project Structure

```text
docker-nginx-mini-project/
├── Dockerfile
├── index.html
└── README.md
```

## Learning Outcomes

- Understanding Docker images and containers
- Writing and updating a Dockerfile
- Building custom Docker images
- Deploying Nginx websites inside containers
- Mapping host ports to container ports
- Managing multiple container versions
- Using Git and GitHub for version control

## Future Improvements

- Add Docker Compose
- Implement GitHub Actions CI/CD
- Deploy the application to AWS
- Add monitoring with Prometheus and Grafana

## Author

DevOps Learning Portfolio Project
