# Portainer Deployment with Docker Compose

This project provides a simple way to deploy [Portainer CE](https://www.portainer.io/) using Docker Compose.  
Portainer is a lightweight management UI that allows you to easily manage your Docker environments (hosts or Swarm clusters).

---

## 📦 Requirements

- Docker 
- Docker Compose 

```bash
sudo pacman -S docker docker-compose
```

---

## 🚀 Quick Start

1. **Clone this repository:**

```bash
mkdir portainer-setup && cd portainer-setup
```
2. **Run The Composer:**

```bash
docker compose up -d
```

---

🔐 Access Portainer

```
https://localhost:9443
```

📁 Volumes Used

- `portainer_data`: Persistent volume to store Portainer's data.

- `/var/run/docker.sock`: Allows Portainer to communicate with the Docker daemon.

---

🛑 Stop and Remove

- To stop and remove Portainer:

```bash
docker compose down

```

- To remove everything including the volume:

```bash
docker compose down -v

```