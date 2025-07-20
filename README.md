# CorpseBeats - Enterprise Discord Music Bot

A powerful, enterprise-ready Discord music bot built with Discord.js and Lavalink, featuring a web dashboard and comprehensive music controls.

## 🎵 Features

- **High-Quality Music Playback** - Powered by Lavalink audio processing
- **32+ Slash Commands** - Modern Discord interaction support
- **Web Dashboard** - Browser-based management interface
- **Multi-Platform Support** - YouTube, Spotify, SoundCloud, and more
- **Advanced Controls** - Queue management, filters, lyrics, and search
- **Enterprise Ready** - Docker deployment with environment configuration
- **24/7 Mode** - Continuous operation support
- **Permission System** - Role-based access controls

## 🚀 Quick Start

### Prerequisites
- Node.js 18+
- Docker & Docker Compose
- Discord Bot Application with proper permissions

### Installation

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd CorpseBeats-MusicBot
   ```

2. **Set up environment variables**
   ```bash
   cp .env.example .env
   # Edit .env with your Discord bot credentials
   ```

3. **Start with Docker**
   ```bash
   docker-compose up -d
   ```

4. **Access the web dashboard**
   Open http://localhost:4200 in your browser

## ⚙️ Configuration

### Required Environment Variables

```env
TOKEN=your_discord_bot_token
CLIENT_ID=your_bot_application_id
CLIENT_SECRET=your_bot_client_secret
ADMIN_ID=your_discord_user_id
```

### Discord Bot Setup
1. Create application at https://discord.com/developers/applications
2. Enable bot user and copy token
3. Set up OAuth2 redirects: `http://localhost:4200/api/callback`
4. Invite bot with proper permissions

## 🎮 Commands

### Music Controls
- `/play <song>` - Play music from various sources
- `/pause` / `/resume` - Control playback
- `/skip` - Skip current track
- `/queue` - View current queue
- `/volume <1-100>` - Adjust volume

### Advanced Features
- `/loop` - Loop current track or queue
- `/shuffle` - Shuffle queue
- `/filters` - Apply audio filters
- `/lyrics` - Get song lyrics
- `/search` - Search for tracks

### Administration
- `/247` - Enable 24/7 mode
- `/autoleave` - Auto-disconnect when empty
- `/clean` - Clear queue

## 🛠️ Development

### Local Development
```bash
npm install
npm start
```

### Dashboard Development
```bash
cd dashboard
npm install
npm run dev
```

## 🐳 Docker Deployment

The bot includes production-ready Docker configuration:

```yaml
# Uses Node.js 18 Alpine
# Includes Lavalink audio server
# Automatic dependency installation
# Environment-based configuration
```

## 🔧 Customization

- **Branding**: Update bot name, avatar, and embed colors in `config.js`
- **Features**: Add custom commands in the `commands/` directory
- **Dashboard**: Customize the web interface in the `dashboard/` folder

## 📝 License

This project is based on the SudhanPlayz Discord-MusicBot template and is licensed under Apache-2.0.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📞 Support

For support and questions, please open an issue in this repository.

---

**⚠️ Note**: This bot requires a working Lavalink server for music functionality. The included configuration uses a reliable public server for development and testing.