---
layout: "default"
title: "🎉 release - Simple Setup for Convenient Use"
description: "🚀 Integrate and manage file storage with ease using our unified player and spider project, optimized for local networks and NAS environments."
---
# 🎉 release - Simple Setup for Convenient Use

[![Download](https://img.shields.io/badge/Download-latest%20release-brightgreen)](https://github.com/xuxulino/release/releases)

---

## 🚀 Getting Started

Welcome to the **release** project. This application combines multiple features in a user-friendly format. Follow these steps to download and run the software smoothly.

## 📥 Download & Install

1. Visit this page to download: [Release Downloads](https://github.com/xuxulino/release/releases).
2. Choose the latest version suitable for your system.
3. Click on the appropriate file to start the download.

**Important Note:** Follow the system requirements on the release page to ensure compatibility.

---

## 🛠️ Setup Instructions

### 1️⃣ Copy Docker Directory

- Locate the `docker` directory in the downloaded files.
- Copy the entire directory to your preferred location on your device.

### 2️⃣ Start the Service

- Open your terminal.
- Navigate to the directory where `docker-compose.yml` is located.
- Run the following command to start the service:

```bash
docker-compose up -d
```

---

## ⚙️ Configuration Files to Edit

### 1️⃣ Vod Configuration

- Open the configuration file located at:

```text
/docker/vod/config.json
```

- Edit the settings according to your needs.

### 2️⃣ Clash Configuration

- Open the configuration file at:

```text
/docker/clash/config.yaml
```

- Add your Clash subscription URL in the designated area. You can write custom rules if you prefer.

---

## 🔑 Admin Information

- Access the backend using the following link:

```text
http://[Container IP]:8080
```

- Use these default login credentials:
  - Username: `vodspider`
  - Password: `abc123`

---

## ⚠️ Important Considerations

- Downloading Docker images might be restricted by some networks.
  
  👉 To avoid issues, consider using a mirror site:

```text
https://dockerpull.com
```

- **Update Information**:
  - Usually, you only need to replace:

```text
/docker/vod/index.js
```

  - In special cases, you may replace files in the `player` folder.
  - Most other files do not need changes, but you may modify `config.json` as necessary.

---

## 🔍 Release Notes

Below are important updates included in the latest version:

- **2025/12/26**
  - Added WebDAV support for Baidu share mounting.
  - Enhanced WebDAV support for Tianyi mount with root directory file support for iOS (Popcorn playback).
  - Updated backend settings to no longer show unconfigured cloud types. If you fill in Baidu ck, a prompt will indicate "undefined cloud type."

- **2025/12/24**
  - Merged projects, resolved issues with playing Baidu no-password shared links.

---

## 🙋‍♂️ Troubleshooting Tips

If you encounter issues:

- Ensure you are running the application in a network environment, such as a home NAS or local network.
- Verify that Docker is installed and running properly on your system. Refer to Docker's official documentation for installation steps.
- Check configurations in `config.json` and `config.yaml` for correctness.

---

Feel free to download, configure, and enjoy the features of the **release** application. For more detailed instructions or FAQs, refer to the documentation within the repository.