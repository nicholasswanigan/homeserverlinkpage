# 🏠 My Home Server Setup

This repository documents how I run a full-featured home server using Docker on my Windows PC. It's designed for reliability, ease of use, and flexibility — all running off a dedicated NVMe SSD (non-root drive) for performance.

---

## 🧰 Overview

My home server setup covers a variety of personal and family needs — media streaming, game servers, web hosting, automation, and more — all containerized through Docker for easy management and isolation.

---

## ⚙️ Hardware & OS

- **Operating System:** Windows (with WSL2 + Docker Desktop)
- **Storage:** 4TB NVMe SSD (non-root drive) for Docker containers and volumes alongside 2x Seagate IronWolf 12TB HDD
- **CPU/RAM:** AMD Ryzen 9 7900X / 2x CORSAIR VENGEANCE DDR5 RAM 32GB (2x16GB) 6000MHz

---

## 🛠️ Services I'm Running

Here’s a breakdown of the services I’m currently using, all running in Docker containers:

| Service Category     | Apps & Tools Used                                         |
|----------------------|-----------------------------------------------------------|
| 🎬 Media Streaming   | Plex Media Server                                         |
| 🗄️ Databases         | MySQL (used for multiple apps)                            |
| 🎮 Game Hosting      | Minecraft Server                                          |
| 📁 File Sharing      | Samba / Nextcloud / or similar for easy network storage   |
| 🏡 Home Automation   | Home Assistant or similar                                 |
| 🧩 Utility Services  | Portainer, Watchtower (for container management & updates)|
| 🌐 Web Hosting       | Nginx / Apache + Dockerized websites                      |
| 🛡️ VPN Access        | WireGuard or OpenVPN                                      |

---

## 📂 Docker Files

Here are links to the Docker Compose files for each group of services:

- [docker-media-stack](https://github.com/nicholasswanigan/media-stack) – Plex 
- [docker-simple-sql](https://github.com/nicholasswanigan/docker-simple-sql) - MySQL
- [docker-minecraft](https://github.com/nicholasswanigan/minecraft-server) – Minecraft server 
- [docker-file-storage](https://github.com/nicholasswanigan/file-storage) – Storage & file 
- [docker-home-automation](https://github.com/nicholasswanigan/home-automation) – Home Assistant
- [docker-webapp-services](https://github.com/nicholasswanigan/webapp-services) – Nginx 
- [docker-vpn](https://github.com/nicholasswanigan/VPN) - VPN

> **Note:** These repos contain `docker-compose.yml` files and `.env` templates to get everything running.
