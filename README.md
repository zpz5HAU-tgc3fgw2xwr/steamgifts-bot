# 🤖 Steamgifts Bot

A feature-rich bot built with TypeScript to automate interactions on the Steamgifts platform. Designed for efficiency, modularity, and ease of use, this project brings a modern approach to managing giveaways and accounts with advanced automation capabilities.

## ✨ Features

- **Multi-Account Support**: Manage multiple accounts via a JSON configuration file.
- **Rate Limiting and Throttling**: Intelligent request handling to avoid bans.
- **Headless Automation**: Utilize Puppeteer to interact with the Steamgifts website.
- **API Integration**: Leverage API calls wherever feasible for better performance.
- **Dockerized Deployment**: Run the bot seamlessly in the background using Docker.
- **Extensible Design**: Built with TypeScript for modularity and future enhancements.

## 🚀 Project Knowledge Goals

- **Learn Efficient Browser Automation**: Implement headless browser control with Puppeteer.
- **Enhance Modular Design Skills**: Develop extensible and maintainable code with TypeScript.
- **Understand Throttling Techniques**: Apply intelligent rate limiting to simulate realistic usage patterns.
- **Master Deployment Strategies**: Containerize the project with Docker for efficient deployment.

## 📦 Installation

### Prerequisites

- [Node.js](https://nodejs.org) (v16 or higher recommended)
- [Docker](https://www.docker.com) (optional, for containerized deployment)

### Steps

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/zpz5HAU-tgc3fgw2xwr/steamgifts-bot.git
   ```

2. **Navigate to the Project Directory**:

   ```bash
   cd steamgifts-bot
   ```

3. **Install Dependencies**:

   ```bash
   npm install
   ```

4. **Configure Accounts**:

   - Update the `accounts.json` file with your Steamgifts account details.

5. **Run the Bot**:

   - For local execution:

     ```bash
     npm start
     ```

   - For Dockerized deployment:

     ```bash
     docker build -t steamgifts-bot .
     docker run -d steamgifts-bot
     ```

## 🌟 Planned Enhancements

- **OpenVPN Integration**: (Stretch Goal) Route account-specific traffic through OpenVPN for added anonymity.
- **Rate Limit Testing**: Fine-tune request intervals to prevent account flags.
- **Advanced Configurations**: Support for custom filters, proxies, and intervals.
- **Web UI**: (Potential Future Addition) A simple interface to monitor and control the bot.

## 🖥️ Technologies Used

- **TypeScript**: Core programming language.
- **Puppeteer**: Headless browser automation.
- **Docker**: Containerization for deployment.
- **Node.js**: Runtime environment.

## 🤝 Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or suggestions.

## 💬 Acknowledgments

This project is inspired by the [Python implementation of a Steamgifts bot](https://github.com/s-tyda/steamgifts-bot). Special thanks to the original creator for the concept and initial groundwork.

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

**Note**: Ensure that the `accounts.json` file is kept secure and not shared publicly, as it contains sensitive account information.
