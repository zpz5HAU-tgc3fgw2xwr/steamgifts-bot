# 🎁 Steamgifts Bot

<p align="center">
  <img src="https://via.placeholder.com/150" alt="Project Logo" width="150" height="150">
</p>

<p align="center">
  <b>A modern TypeScript implementation of the Steamgifts Bot, inspired by the original Python project.</b>
</p>

<p align="center">
  <a href="https://github.com/zpz5HAU-tgc3fgw2xwr/steamgifts-bot/actions">
    <img src="https://img.shields.io/github/actions/workflow/status/zpz5HAU-tgc3fgw2xwr/steamgifts-bot/ci.yml?branch=main" alt="Build Status">
  </a>
  <a href="https://github.com/zpz5HAU-tgc3fgw2xwr/steamgifts-bot/issues">
    <img src="https://img.shields.io/github/issues/zpz5HAU-tgc3fgw2xwr/steamgifts-bot" alt="Issues">
  </a>
  <a href="https://github.com/zpz5HAU-tgc3fgw2xwr/steamgifts-bot/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/zpz5HAU-tgc3fgw2xwr/steamgifts-bot" alt="License">
  </a>
</p>

---

## 🚀 Features

- **Multi-Account Support**: Manage multiple accounts via a JSON configuration file.
- **Rate Limiting and Throttling**: Intelligent request handling to avoid bans.
- **Headless Automation**: Utilize Puppeteer to interact with the Steamgifts website.
- **API Integration**: Leverage API calls wherever feasible for better performance.
- **Dockerized Deployment**: Run the bot seamlessly in the background using Docker.
- **Extensible Design**: Built with TypeScript for modularity and future enhancements.

---

## 📋 Planned Enhancements

- **OpenVPN Integration**: (Stretch Goal) Route account-specific traffic through OpenVPN for added anonymity.
- **Rate Limit Testing**: Fine-tune request intervals to prevent account flags.
- **Advanced Configurations**: Support for custom filters, proxies, and intervals.
- **Web UI**: (Potential Future Addition) A simple interface to monitor and control the bot.

---

## 📦 Installation

### Prerequisites

- [Node.js](https://nodejs.org/) (v16 or higher recommended)
- [Docker](https://www.docker.com/) (optional but recommended)

### Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/zpz5HAU-tgc3fgw2xwr/steamgifts-bot.git
   cd steamgifts-bot
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Build the project:
   ```bash
   npm run build
   ```
4. (Optional) Build the Docker image:
   ```bash
   docker build -t steamgifts-bot .
   ```

---

## ⚙️ Configuration

Create a `config.json` file in the root directory (or mount it into the Docker container). Example:

```json
{
  "accounts": [
    {
      "username": "account1",
      "password": "password1",
      "openvpn": "account1.ovpn"
    },
    {
      "username": "account2",
      "password": "password2",
      "openvpn": "account2.ovpn"
    }
  ],
  "settings": {
    "rateLimit": 5000,
    "maxRetries": 3
  }
}
```

---

## 🖥️ Usage

### Locally

```bash
npm start
```

### With Docker

```bash
docker run -d \  
  -v $(pwd)/config.json:/app/config.json \  
  steamgifts-bot
```

---

## 🤝 Contributing

Contributions are welcome! Please submit issues or pull requests on [GitHub](https://github.com/zpz5HAU-tgc3fgw2xwr/steamgifts-bot).

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

## 📣 Credits

- Inspired by [s-tyda/steamgifts-bot](https://github.com/s-tyda/steamgifts-bot)
- Built with TypeScript, Puppeteer, and Node.js
