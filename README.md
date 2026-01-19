# 🚀 DevOps EC2 Deployment Project

This project demonstrates a production-style deployment of a static website to an AWS EC2 instance using CI/CD best practices.

It covers:

- Cloud infrastructure setup
- Secure server configuration
- Automated deployment
- Backup and rollback strategy
- Real-world DevOps troubleshooting

---

## 🏗️ Architecture Overview

- AWS EC2 (Ubuntu 24.04)
- Nginx Web Server
- GitHub Actions (CI/CD)
- SSH Key Authentication
- UFW Firewall

---

## 🔄 CI/CD Flow

1. Code pushed to `main`
2. GitHub Actions triggered
3. Files copied to EC2 (user directory)
4. Backup of current production site
5. Deployment to `/var/www/html`
6. Nginx reload

---

## 🔐 Security Measures

- SSH key-based authentication
- Root login disabled
- Password login disabled
- UFW firewall enabled (ports 22 and 80 only)

---

## 🧪 Key Learnings

- Linux permissions and ownership
- Safe deployment patterns
- CI/CD troubleshooting
- Production-minded automation

---
