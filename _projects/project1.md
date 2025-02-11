---
layout: project
title: "Simple WordPress Docker Environment"
description: "A streamlined Docker environment for WordPress with automated daily backups and environment variable management."
permalink: /wpbk/
github_url: "https://github.com/superdoccimo/wpbk"
---

## Overview

This project provides a simplified Docker setup for running WordPress alongside MySQL. It features automatic daily database backups, persistent storage for WordPress files and the database, and convenient environment variable management through a `.env` file.

## Key Features

- **WordPress & MySQL Setup:** Quickly deploy WordPress with a MySQL database.
- **Automated Backups:** Daily backups ensure your database is safely preserved.
- **Data Persistence:** Ensures WordPress files and database changes are retained.
- **Log Access:** Apache logs are accessible from the host system.
- **Easy Configuration:** Manage environment settings with a simple `.env` file.

## Quick Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/superdoccimo/wpbk.git
