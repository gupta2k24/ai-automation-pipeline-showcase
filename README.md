# AI Automation Pipeline – Serverless Content Publishing System

## 📌 Project Overview

This project demonstrates a serverless AI-driven automation pipeline that converts a 4-hour manual content publishing process into a fully automated 2-minute workflow.

The system generates quote-based images and automatically publishes them to:

- Instagram
- Facebook
- Email

The architecture is modular, scalable, and secure.

---

## 🚀 Problem Statement

Manual content creation and cross-platform publishing was:

- Time consuming (4 hours per post)
- Repetitive
- Error-prone
- Inconsistent in formatting and quality

There was a need to automate:

1. Quote image generation  
2. Caption formatting  
3. Multi-platform publishing  
4. Email notification  

---

## 💡 Solution Architecture

The system uses:

- Python for orchestration
- GitHub Actions as serverless backend engine
- Meta Graph API for Instagram & Facebook
- SMTP for automated email
- Google Apps Script + Web UI trigger (front-end button)

---

## 🧱 Architecture Diagram

<img width="1280" height="720" alt="Serverless_Automation_Pipeline" src="https://github.com/user-attachments/assets/343906a1-6518-4e4c-8502-14c89cead4ef" />


---

## 🔄 End-to-End Workflow

### Step 1 – Image Generation (create_image.py)
- Loads background image
- Crops & resizes to 1080x1350
- Wraps text using balanced layout logic
- Dynamically resizes font
- Adds watermark + shadow effects
- Generates timestamped output image

### Step 2 – Instagram Publishing
- Uses Instagram Graph API
- Reads secure Access Token
- Uploads media container
- Publishes automatically

### Step 3 – Facebook Publishing
- Uses Facebook Graph API
- Uploads image to page endpoint

### Step 4 – Email Dispatch
- Uses SMTP authentication
- Attaches generated image
- Sends automated email notification

---

## 🛠 Technical Stack

- Python
- Pillow (PIL)
- textwrap
- datetime
- requests
- smtplib
- GitHub Actions
- Meta Graph API

---

## 🔐 Security Design

- No username/password automation
- Uses official Meta Graph API
- Access tokens stored securely
- Serverless execution model

---

## 🎥 Live Demo

Demo Video (Unlisted)-
https://youtu.be/ArCVBvE7cJs

---

## 🏗 Engineering Highlights

- Modular script design
- API-based authentication
- Serverless CI/CD execution
- Error handling & logging
- Scalable workflow structure
- Production-oriented system design

---

## 📌 Note

The production repository remains private to protect business logic and credentials.  
This public repository showcases system architecture and implementation methodology.
