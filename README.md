# CodeAlpha Docker Web Server

A simple web page served by Nginx inside a Docker container.

## Files

- `index.html` — web page
- `Dockerfile` — instructions to build the Docker image

## Build and run

```powershell
docker build -t codealpha-web:1.0 .
docker run -d --name codealpha-custom -p 8081:80 codealpha-web:1.0