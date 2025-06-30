# DevOps CI/CD Flask App Project

This project demonstrates a complete CI/CD pipeline using:
- ✅ Flask (Python web app)
- 🐳 Docker (Containerization)
- 🔁 GitHub Actions (Automation)
- ☁️ AWS EC2 (Deployment)

## 📦 Features
- Build & deploy Flask app using Docker
- CI/CD pipeline via GitHub Actions
- Auto-deploys on EC2 when code changes

## 🔐 Secrets Required (in GitHub Repo Settings > Secrets)
- `EC2_HOST` – your EC2 public IP or domain
- `EC2_USER` – usually `ubuntu`
- `EC2_SSH_KEY` – private key content

## 🚀 How it Works
1. Push code to `main`
2. GitHub Actions triggers CI/CD
3. SSH into EC2 & rebuilds Docker container
4. App is live at `http://<EC2-IP>:5000`
