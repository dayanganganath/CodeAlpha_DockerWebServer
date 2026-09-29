# CodeAlpha Docker Web Server

A static web page served by Nginx inside a Docker container.

## Files

- `index.html` — the web page
- `Dockerfile` — builds the Nginx image and copies the page into it

## Requirements

- Docker Desktop (or Docker Engine)

## Build

Run these commands from the project directory:

```powershell
docker build -t codealpha-web:1.0 .
```

## Run

```powershell
docker run -d --name codealpha-custom -p 8081:80 codealpha-web:1.0
```

Open http://localhost:8081 in a browser.

## Manage the container

```powershell
docker ps
docker logs codealpha-custom
docker stop codealpha-custom
docker start codealpha-custom
```

The browser will only reach the page while the container is running.
