# My Docker Website

This is a simple static website that I made for my Docker assignment. It has 4 pages (Home, About, Contact, and Student Page) and runs using Nginx inside a Docker container.

## What it does

It's a basic website that you can navigate through using the navbar at the top. The whole point is that it runs inside Docker so you don't have to install anything manually.

## Dependencies

- Docker (to build and run the container)
- Nginx (this gets pulled automatically when you build the image, you don't need to install it yourself)

## How to build the image

Make sure Docker is open on your computer, then run this in the project folder:

```bash
docker build -t docker-website .
```

## How to run the container

```bash
docker run -d -p 8080:80 docker-website
```

## Expected output

Open your browser and go to `http://localhost:8080` and you should see the website.

## How to stop it

```bash
docker ps
docker stop <container_id>
```
