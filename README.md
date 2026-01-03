🚀 Automated Job Alert System (n8n)
📌 Overview

This project automates job alerts by monitoring LinkedIn job postings using a Google Alerts RSS feed.
It filters React, MERN, and Full Stack Developer roles and sends a single email summary containing only new job postings.

This setup is intended for personal use and runs locally using Docker.

🛠️ Tech Stack

n8n – Workflow Automation

Google Alerts – RSS Feed Source

Gmail – Email notifications

Docker & Docker Compose – Local runtime

⚙️ Features

Runs automatically every 1 hour

Filters relevant job roles (React / MERN / Full Stack)

Avoids duplicate job alerts

Sends one consolidated email with new jobs only

Simple local setup (no cloud deployment required)

🏗️ Workflow Architecture
Schedule Trigger
   ↓
RSS Feed Reader
   ↓
Role Filter (IF condition)
   ↓
Deduplication (Static Data)
   ↓
Gmail Notification

🔐 Credentials Setup

⚠️ Credentials are NOT included in this repository

After importing the workflow into n8n:

Create Gmail OAuth2 credentials in n8n

Connect the credentials to the Gmail node

Update the recipient email address if required

ℹ️ The Google Alerts RSS feed is public and does not require authentication.

📂 Running Locally (No Deployment)
Prerequisites

Docker

Docker Compose

Start n8n
docker-compose up


After starting:

Open http://localhost:5678

Import the workflow JSON

Configure Gmail credentials

Enable the workflow

📝 Notes

This project is built for learning and personal automation

No production or cloud deployment is required

Sensitive files like .env are excluded via .gitignore

📄 License

This project is for personal use and learning purposes.
