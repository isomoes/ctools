# CTools - Curated Tools Collection

A curated collection of self-hosted tools and applications, each pre-configured with Docker Compose for easy deployment and management.

## 🎯 Philosophy

**Simple. Self-hosted. Secure.**

Each tool in this collection comes with:

- 🐳 Ready-to-use Docker Compose configurations
- 📚 Comprehensive documentation and examples
- 🔒 Security-focused default settings
- 🚀 One-command deployment
- 🛠 Real-world usage examples

## 🧰 Available Tools

### 🔍 [changedetection/](./changedetection/) - Website Change Monitoring

Monitor websites for changes and get notified instantly.

- **What it does**: Track price changes, stock availability, content updates, and more
- **Key features**: Browser automation, JavaScript support, multi-channel notifications
- **Access**: http://localhost:5000
- **Quick start**: `cd changedetection && docker compose up -d`

**Perfect for**: E-commerce monitoring, API tracking, content updates, government sites

### [sitewatcher/](./sitewatcher/) - Website Uptime Monitoring

Keep a history of uptime and response times and get alerts before TLS certificates or domains expire.

- **Access**: http://127.0.0.1:8080
- **Quick start**: `cd sitewatcher && docker compose run --rm setup && docker compose up -d`

---

## 🚀 Quick Start

### Prerequisites

- Docker and Docker Compose installed
- Basic understanding of Docker containers

### Deploy a Tool

1. **Choose your tool** from the list above
2. **Navigate to the tool directory**:
   ```bash
   cd changedetection
   ```
3. **Start the service**:
   ```bash
   docker compose up -d
   ```
4. **Access the web interface** (URLs provided in each tool's README)

### General Management

**View running services**:

```bash
docker compose ps
```

**View logs**:

```bash
docker compose logs -f
```

**Stop services**:

```bash
docker compose down
```

**Update to latest version**:

```bash
docker compose pull
docker compose up -d
```

## 🤝 Contributing

### Adding New Tools

When adding tools to this collection, ensure they meet these criteria:

1. **Self-hosted**: Can run entirely on local infrastructure
2. **Docker ready**: Provides reliable Docker images
3. **Well documented**: Clear setup and usage instructions
4. **Actively maintained**: Regular updates and security patches
5. **Useful**: Solves real-world problems

### Tool Structure

Each tool should include:

```
tool-name/
├── README.md           # Comprehensive usage guide
├── docker-compose.yml  # Service configuration
└── [config-files]      # Additional configuration if needed
```

## 📄 License

This collection and configurations are provided under the MIT License. Individual tools maintain their respective licenses.

---

**Happy self-hosting! 🏠**

_Start with changedetection.io and expand your toolkit from there._
