## 👋 Welcome to actualbudget 🚀

Self-hosted actualbudget application

## 📋 Description

Self-hosted actualbudget application

## 🚀 Services

- **actualbudget**: actualbudget/actual-server:latest

## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/actualbudget/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/actualbudget" ~/.local/srv/docker/actualbudget
cd ~/.local/srv/docker/actualbudget
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install actualbudget
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:5006

## 📂 Volumes

- `./volumes/data/actualbudget` - Data storage

## 🔍 Logging

```shell
docker compose logs -f actualbudget
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
