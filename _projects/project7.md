---
layout: project
title: "Nginx Reverse Proxy with Auto SSL"
description: "A simple toolkit for setting up an Nginx reverse proxy with automatic SSL certificate management, featuring one-script setup, secure configuration, and automatic certificate renewal."
permalink: /rev/
github_url: "https://github.com/superdoccimo/rev"
---

This project provides a straightforward solution to deploy an Nginx reverse proxy with automatic SSL certificate management using Let's Encrypt. The toolkit simplifies the setup process with a single script that configures your domain, email, and environment settings (staging or production).

**Key Features:**

- **Automatic SSL Setup:** Easily obtain and renew SSL certificates.
- **Secure Configuration:** Supports TLS 1.2/1.3 with modern cipher suites, HTTP to HTTPS redirection, and optional ads.txt support.
- **One-Script Setup:** Configure your settings in `init-letsencrypt.sh` and run the script to initialize the environment.
- **Websocket Support:** Ensures compatibility with modern web applications.

**Quick Start Guide:**

1. **Edit Configuration:**  
   Open `init-letsencrypt.sh` and update the following settings:
   - `domains`: Your domain name(s)
   - `email`: Your email address for certificate registration
   - `staging`: Set to `1` for testing and `0` for production

2. **Clone and Set Up:**
   ```bash
   git clone https://github.com/superdoccimo/rev.git
   cd rev
   chmod +x init-letsencrypt.sh
   sudo ./init-letsencrypt.sh
