# Apache Multi-Site Docker Setup

This project demonstrates how to run five independent Apache web servers using Docker and Docker Compose. Each site is deployed in its own container and accessible on a unique port.

## 🌐 Project Overview

- 5 containers running Apache
- Each serves a unique `index.html` file
- Managed using Docker Compose
- Ports exposed: 81, 82, 83, 84, 85

## 📁 Folder Structure

apache-multi/
├── Dockerfile
├── docker-compose.yml
├── site1/
│ └── index.html
├── site2/
│ └── index.html
├── site3/
│ └── index.html
├── site4/
│ └── index.html
└── site5/
└── index.html

## 🛠️ How to Run

```bash
# Step into the project folder
cd apache-multi

# Build and run the containers
sudo docker-compose up -d --build

# Check running containers
sudo docker ps

Access Your Sites

Replace YOUR_EC2_PUBLIC_IP with your actual IP (e.g., 52.23.164.197):

http://YOUR_EC2_PUBLIC_IP:81 → Site 1

http://YOUR_EC2_PUBLIC_IP:82 → Site 2

http://YOUR_EC2_PUBLIC_IP:83 → Site 3

http://YOUR_EC2_PUBLIC_IP:84 → Site 4

http://YOUR_EC2_PUBLIC_IP:85 → Site 5
