# 🛡️ CyberShield SOC: Intelligence & Monitoring Dashboard

A Python-based **Security Operations Center (SOC)** tool designed to monitor, filter, and report on global threat intelligence data. This project demonstrates a **Defense-in-Depth** approach to web application security and threat management.

## 🚀 Project Overview
This application serves as a centralized dashboard for security analysts to investigate malicious IP addresses and locations. It bridges the gap between raw threat data and actionable intelligence by providing a secure, searchable, and exportable interface.

## 🔒 Security Implementations (The "CyberShield" Framework)
To align with industry-standard security practices, the following protections are hard-coded into the architecture:

* **Anti-DoS Rate Limiting:** Implements a sliding-window logic to prevent API abuse and brute-force attempts (Status 429 handling).
* **SQL Injection (SQLi) Protection:** All database interactions utilize **Parameterized Queries**, ensuring user input is never executed as code.
* **XSS & Input Sanitization:** Utilizes Regex-based filtering to sanitize search queries and prevent Cross-Site Scripting.
* **Defense Headers:** Implements professional HTTP security headers (`X-Frame-Options`, `X-Content-Type-Options`) to protect against clickjacking and MIME-sniffing.
* **Audit Logging:** Integrated system logging tracks every access attempt and security alert for forensic review.

## 🛠️ Tech Stack
* **Language:** Python 3.12
* **Framework:** Flask
* **Database:** SQLite3 (Persistent Threat Storage)
* **Tunneling:** Cloudflare (Secure remote access without port forwarding)
* **Data Handling:** CSV Reporting Engine & JSON API v2.0

## 📂 File Structure
* `app.py`: The core application containing security logic, routes, and the dashboard.
* `threat_intel.db`: SQLite database for persistent threat storage.
* `requirements.txt`: List of dependencies for rapid deployment.

## ⚙️ Installation & Usage
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/CyberShield-SOC.git](https://github.com/YOUR_USERNAME/CyberShield-SOC.git)
