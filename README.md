# 🚀 Automated Job Alert System (n8n)

## 📌 Overview
This project automatically monitors LinkedIn job postings using Google Alerts RSS.
It filters React, MERN, and Full Stack Developer roles and sends a single email
digest every hour with only new jobs.

## 🛠️ Tech Stack
- n8n (Workflow Automation)
- Google Alerts (RSS)
- Gmail
- Docker
- Railway (Deployment)

## ⚙️ Features
- Runs automatically every 1 hour
- Filters relevant job roles
- Prevents duplicate alerts
- Sends one clean email with all new jobs
- Runs 24/7 in cloud

## 🏗️ Architecture
Schedule Trigger → RSS Read → IF Filter → Deduplication → Email


## 🔐 Credentials Setup

This workflow does not include any credentials.

After importing the workflow into n8n:
1. Add your Gmail OAuth2 credentials
2. Connect the Gmail node manually
3. Update the recipient email if needed

RSS feed is public and does not require authentication.

## 🚀 Deployment
Deployed using Docker on Railway.app (free tier).

## 📂 Run Locally
```bash
docker-compose up
