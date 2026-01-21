# Actual Budget

Actual Budget is a local-first personal finance tool with optional sync capabilities. It's privacy-focused, fast, and gives you complete control over your financial data with zero-based budgeting methodology.

## Features

- **Zero-Based Budgeting**: Allocate every dollar before spending
- **Bank Sync**: Import transactions from financial institutions
- **Multi-Device Sync**: Optional end-to-end encrypted synchronization
- **Offline First**: Works completely offline, sync when you want
- **Reports**: Visualize spending patterns and trends
- **Goals**: Set and track savings goals
- **Schedules**: Plan recurring transactions
- **Rules**: Auto-categorize transactions
- **Multi-Currency**: Support for multiple currencies
- **Open Source**: Full control and transparency

## Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/actualbudget/main/docker-compose.yaml" | docker compose -f - up -d
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

## Configuration

### Ports

- `5006`: Web interface

## Initial Setup

1. Access Actual Budget at `http://localhost:5006`
2. Create your first budget or import existing
3. Set up accounts (checking, savings, credit cards)
4. Create budget categories
5. Configure bank sync (optional)
6. Set up rules for auto-categorization

## Security Recommendations

- **HTTPS**: Use reverse proxy with SSL/TLS
- **Backups**: Regular backups of budget data
- **Network Access**: Restrict access with firewall rules
- **Sync Encryption**: Use end-to-end encryption for sync
- **Updates**: Keep Actual Budget updated

## Backup

Critical directories to backup:
- `./rootfs/data/actualbudget`: All budget files and data

## Documentation

- Official Documentation: https://actualbudget.org/docs/
- GitHub: https://github.com/actualbudget/actual-server
- Community: https://discord.gg/pRYNYr4W5A

## License

Actual Budget is licensed under the MIT License.
