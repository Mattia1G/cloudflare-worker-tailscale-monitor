# Cloudflare Worker Tailscale Monitor 🌐🔍

![GitHub Release](https://img.shields.io/github/release/Mattia1G/cloudflare-worker-tailscale-monitor.svg) ![GitHub Stars](https://img.shields.io/github/stars/Mattia1G/cloudflare-worker-tailscale-monitor.svg) ![GitHub Forks](https://img.shields.io/github/forks/Mattia1G/cloudflare-worker-tailscale-monitor.svg)

Welcome to the **Cloudflare Worker Tailscale Monitor** repository! This project provides a simple and efficient way to monitor the status of your Tailscale devices. It leverages the power of Cloudflare Workers to send notifications via Telegram when device status changes.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Getting Started](#getting-started)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [Notifications](#notifications)
- [Contributing](#contributing)
- [License](#license)
- [Links](#links)

## Introduction

Tailscale is a mesh VPN that simplifies secure access to your devices. However, keeping track of device status can be challenging. This project aims to solve that problem by monitoring Tailscale devices and sending real-time notifications to your Telegram account.

## Features

- Monitor Tailscale device status in real-time.
- Send notifications to Telegram on device status changes.
- Lightweight and efficient, running on Cloudflare Workers.
- Easy to set up and configure.

## Getting Started

To get started with the Cloudflare Worker Tailscale Monitor, you will need a few prerequisites:

1. A Tailscale account.
2. A Telegram account and a bot token.
3. A Cloudflare account to deploy the worker.

## Installation

You can download the latest release of the Cloudflare Worker Tailscale Monitor [here](https://github.com/Mattia1G/cloudflare-worker-tailscale-monitor/releases). Follow the instructions provided in the release notes to execute the necessary files.

### Prerequisites

- Node.js (for local development)
- Cloudflare Workers CLI (Wrangler)

## Configuration

Once you have downloaded and installed the necessary files, you will need to configure the application. Open the configuration file and set the following parameters:

- **Tailscale API Key**: Obtain this from your Tailscale account.
- **Telegram Bot Token**: Create a new bot via [BotFather](https://t.me/botfather) on Telegram.
- **Chat ID**: You can find this by sending a message to your bot and checking the updates.

### Example Configuration

```json
{
  "tailscale_api_key": "YOUR_TAILSCALE_API_KEY",
  "telegram_bot_token": "YOUR_TELEGRAM_BOT_TOKEN",
  "chat_id": "YOUR_CHAT_ID"
}
```

## Usage

After configuring the application, you can deploy the Cloudflare Worker. Use the following command:

```bash
wrangler publish
```

This command will upload your worker to Cloudflare. Once deployed, the worker will start monitoring your Tailscale devices.

## Notifications

When a device's status changes, the Cloudflare Worker will send a notification to your Telegram account. You can customize the message format in the configuration file.

### Example Notification

```
Device: MyDevice
Status: Online
```

## Contributing

We welcome contributions to improve the Cloudflare Worker Tailscale Monitor. If you have suggestions or enhancements, please fork the repository and submit a pull request.

### Steps to Contribute

1. Fork the repository.
2. Create a new branch for your feature or fix.
3. Make your changes.
4. Commit and push your changes.
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Links

For more information, check the [Releases](https://github.com/Mattia1G/cloudflare-worker-tailscale-monitor/releases) section. Here, you can find the latest updates and download files.

Feel free to explore the project and contribute! If you have any questions, don't hesitate to reach out.