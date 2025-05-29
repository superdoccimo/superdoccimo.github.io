---
layout: project
title: "Simple WordPress Docker Environment"
description: "A streamlined Docker environment for WordPress with automated daily backups and environment variable management."
permalink: /wpbk/
github_url: "https://github.com/superdoccimo/wpbk"
json_ld: >
  <script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@graph": [
      {
        "@type": "Article",
        "headline": "Simple WordPress Docker Environment",
        "description": "Learn how to quickly deploy WordPress with Docker, including daily backups and persistent storage setup.",
        "author": {
          "@type": "Person",
          "name": "Mamu Minokamo"
        },
        "publisher": {
          "@type": "Organization",
          "name": "Minokamo Project",
          "logo": {
            "@type": "ImageObject",
            "url": "https://superdoccimo.github.io/assets/logo.png"
          }
        },
        "datePublished": "2024-09-19",
        "url": "https://superdoccimo.github.io/wpbk/"
      },
      {
        "@type": "VideoObject",
        "name": "DockerでWordPressを動かす方法",
        "description": "Dockerと自動バックアップを使ってWordPressを運用する手順を解説しています。",
        "thumbnailUrl": "https://i.ytimg.com/vi/MjQ9jPClsaY/maxresdefault.jpg",
        "uploadDate": "2024-09-19",
        "contentUrl": "https://youtu.be/MjQ9jPClsaY",
        "embedUrl": "https://www.youtube.com/embed/MjQ9jPClsaY"
      }
    ]
  }
  </script>
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
    ```
