# CI Docker Compose Validation

## Overview
This project demonstrates a CI pipeline that validates a multi-container application using Docker Compose.

## Architecture
- web: Nginx service
- automation: Health-check container

## CI Flow
1. Build images
2. Start services using Docker Compose
3. Validate service availability
4. Tear down services automatically

## Failure Handling
If any service fails to start or respond, the CI pipeline fails immediately.

## Technologies Used
- Docker
- Docker Compose
- GitHub Actions