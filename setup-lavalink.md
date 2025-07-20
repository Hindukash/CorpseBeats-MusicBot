# Lavalink Setup Guide

## Option 1: Use Docker (Recommended)
The bot includes Docker configuration with Lavalink. Run:
```bash
docker-compose up -d
```

## Option 2: Manual Lavalink Setup
1. Download Java 17+ if not installed
2. Download latest Lavalink.jar from: https://github.com/lavalink-devs/Lavalink/releases
3. Create `application.yml`:
```yaml
server:
  port: 2333
  address: 0.0.0.0
lavalink:
  server:
    password: "youshallnotpass"
    sources:
      youtube: true
      bandcamp: true
      soundcloud: true
      twitch: true
      vimeo: true
      http: true
      local: false
    filters:
      volume: true
      equalizer: true
      karaoke: true
      timescale: true
      tremolo: true
      vibrato: true
      distortion: true
      rotation: true
      channelMix: true
      lowPass: true
    bufferDurationMs: 400
    frameBufferDurationMs: 5000
    youtubePlaylistLoadLimit: 6
    playerUpdateInterval: 5
    youtubeSearchEnabled: true
    soundcloudSearchEnabled: true
    gc-warnings: true
```
4. Run: `java -jar Lavalink.jar`

## Option 3: Public Lavalink (Not recommended for production)
Use public servers from: https://lavalink-list.darrennathanael.com/
Update config.js with public server details.

## Test Connection
After setup, the bot will automatically connect to Lavalink on startup.