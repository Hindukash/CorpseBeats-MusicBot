# CorpseBeats 🎵

A modern Discord music bot with web dashboard, built on Discord.js v14 and Lavalink.

## Features

- **🎧 High-Quality Audio** - Lavalink-powered music streaming
- **⚡ Slash Commands** - Modern Discord interactions (32+ commands)
- **🌐 Web Dashboard** - Browser-based management panel
- **🎵 Multi-Source** - YouTube, Spotify, SoundCloud support
- **🔧 Enterprise Ready** - Docker deployment with environment config
- **🎛️ Advanced Controls** - Filters, queue management, 24/7 mode

## Quick Setup

### Prerequisites
- Node.js 18+
- Docker & Docker Compose
- Discord Bot with proper permissions

### Installation

```bash
# Clone and setup
git clone https://github.com/Hindukash/CorpseBeats-MusicBot.git
cd CorpseBeats-MusicBot
cp .env.example .env

# Configure your .env file with Discord credentials
# TOKEN, CLIENT_ID, CLIENT_SECRET, ADMIN_ID

# Start with Docker
docker-compose up -d

# Dashboard available at http://localhost:4200
```

## Discord Bot Setup

1. Create bot at [Discord Developer Portal](https://discord.com/developers/applications)
2. Copy bot token to `.env` file
3. Add OAuth2 redirect: `http://localhost:4200/api/callback`
4. Invite with proper permissions

## Commands

| Category | Commands |
|----------|----------|
| **Music** | `/play`, `/pause`, `/resume`, `/skip`, `/stop`, `/queue` |
| **Control** | `/volume`, `/loop`, `/shuffle`, `/seek`, `/nowplaying` |
| **Advanced** | `/filters`, `/lyrics`, `/search`, `/247`, `/autoleave` |

## Configuration

The bot uses environment variables for secure configuration:

```env
TOKEN=your_discord_bot_token
CLIENT_ID=your_bot_application_id  
CLIENT_SECRET=your_bot_client_secret
ADMIN_ID=your_discord_user_id
```

## Development

```bash
# Local development
npm install
npm start

# Dashboard development
cd dashboard && npm run dev
```

## License

Apache-2.0 License - Based on [SudhanPlayz/Discord-MusicBot](https://github.com/SudhanPlayz/Discord-MusicBot)

## About This Project

This Discord Music Bot was built using an existing template and enhanced through AI-assisted development. All modifications from the original template—including updates for 2025 compatibility—were implemented using AI coding tools and prompt engineering.

The project demonstrates how AI can effectively adapt and modernize existing codebases through guided workflows and intelligent code generation.

## Contributing

Contributions welcome! Please read our contributing guidelines and submit pull requests.

---

**Built with ❤️ by the open-source community**