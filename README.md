# 🐳 Apache Docker Demo

## 📌 Project Overview

This project demonstrates how to containerize a basic Apache HTTP server using Docker. The container serves two custom HTML pages — `home.html` and `about.html` — making it a simple yet effective example of deploying static web content via Docker.

---

## 🧰 Technology Stack

- **Web Server**: Apache HTTP Server
- **Containerization**: Docker
- **Content**: Static HTML pages (`home.html`, `about.html`)

---

## 📁 Repository Structure
``` Markdown
apache-docker-demo/
├── Dockerfile
└── site-content/
    ├── home.html
    └── about.html
```

- `Dockerfile`: Defines the Apache server setup and copies HTML files into the container.
- `site-content/`: Contains the static HTML pages served by Apache.

---

## 🚀 How to Run the Project

### 1. Clone the Repository
```bash
git clone https://github.com/Prashanttmahamuni/apache-docker-demo.git
cd apache-docker-demo
```

### 2. Build the Docker Image
```bash
docker build -t apache-demo .
```

### 3. Run the Docker Container
```bash
docker run -d -p 8080:80 apache-demo
```

### 4. Access the Web Pages
Open your browser and visit:
- http://localhost:8080/home.html

- http://localhost:8080/about.html

## 🛠️ Customization
To modify the content:

1. Edit home.html or about.html in the site-content/ directory.

2. Rebuild the Docker image:

```bash
docker build -t apache-demo .
```

3. Restart the container.

## 📦 Deployment Notes
This project can be deployed on any Docker-compatible host, including:

- Local machines

- Cloud VMs (e.g., AWS EC2, Azure VM)

- Kubernetes clusters (with minor adjustments)

