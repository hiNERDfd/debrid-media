# 🎥 debrid-media - Simplify Your Plex Experience

[![Download](https://img.shields.io/badge/Download-Latest%20Release-blue.svg)](https://github.com/hiNERDfd/debrid-media/releases)

## 🚀 Getting Started

Debrid Media makes it easy to run a Plex media server with Real-Debrid. Follow these simple steps to get started.

## 📋 Prerequisites

To use Debrid Media, you need the following accounts:

- **Real-Debrid Premium Account**: This will allow you to access premium services.
- **Plex Account**: You’ll need this to set up your media server.

## ⚙️ Setup

### 1. Configure Environment Variables

- **Rename the example file**:
  - Rename `.env.example` to `.env` in your project folder.

- **Set Your Timezone**:
  - Open `.env` and find the line with `TZ`. Change it to your timezone (e.g., `America/New_York`).

- **Adjust Cache Limit**:
  - Find `RCLONE_CACHE_LIMIT` in the same file. Set it to the disk space you want to dedicate to caching (e.g., `10G` for 10 gigabytes).

- **Get Your Plex Claim Token**:
  - Visit [Plex Claim](https://plex.tv/claim) while signed in. Copy the claim token and paste it into the `PLEX_CLAIM` line in `.env`.

### 2. Provide Your Real-Debrid API Key

- **Open Configuration File**:
  - Navigate to `config/config.yml`.

- **Insert Your API Key**:
  - Find the line that starts with `token`. Replace the placeholder with your Real-Debrid API key. You can get this key from [Real-Debrid Device Page](https://real-debrid.com/devices).

### 3. Launch the Stack

- **Use Docker to Start**:
  - In your terminal, run the command:
    ```
    docker compose up -d
    ```
  This will start all necessary services in the background.

### 4. Plex Setup

- **Access Plex**:
  - Open a web browser and go to `http://<your_server_ip>:32400/web` to set up your media server.

- **Add Content**:
  - Click on `Add Library` and select from `Movies`, `TV Shows`, or `Other Videos`. These should be located under the `/data` directory.

- **Adjust Library Settings**:
  - Go to `Settings` → `Library` in Plex and change the `Library scan interval` to every 15 minutes. This ensures that your library stays up to date.

## 📥 Download & Install

To download the latest version of Debrid Media, visit [this page to download](https://github.com/hiNERDfd/debrid-media/releases).

After downloading, make sure to follow the setup steps above to get everything running.

## 🔄 What's Next

Once your setup is complete, head over to [Debrid Media Manager](https://debridmediamanager.com). Here, you can add the movies or shows you want to enjoy.

Feel free to refer to the configuration and setup sections anytime you need help. Enjoy seamless entertainment with your new Plex server!