# Architecture

The system uses a single EC2 instance running Ubuntu 24.04.

Traffic Flow:
User → EC2 Public IP → Nginx → Static Website

CI/CD Flow:
GitHub → GitHub Actions → SSH → EC2
