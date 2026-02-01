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

## CI Failure and Recovery Demonstration

This project intentionally introduced a misconfigured Docker image for the web service to validate CI fail-fast behavior.

The CI pipeline failed during the Docker Compose startup phase, correctly preventing further steps from running.

After fixing the configuration, the pipeline recovered and completed successfully.

This demonstrates real-world CI debugging, validation, and recovery practices.

This project reflects real-world CI practices used to prevent broken configurations from reaching production.