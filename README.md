# 🎤 VoiceCraft - Dynamic Voice Channel Bot

VoiceCraft is a professional Discord bot that allows users to create and manage their own voice channels with full customization options.

## ✨ Features

- **Join-to-Create System**: Users join a designated channel to create personal voice channels
- **4-Digit Unique IDs**: Each channel gets a unique identifier like "5832+Username"
- **Full Customization**: Rename, bitrate, user limit, lock/unlock channels
- **Role-Based Access**: Invite friends with generated roles
- **Text Channel Integration**: Each voice channel gets its own text channel
- **Auto Cleanup**: Empty channels delete automatically after 60 seconds
- **Multi-Server Support**: Works across unlimited servers
- **Admin Controls**: Easy setup with `/setup` command
- **Live Statistics**: Real-time stats with `/about` command

## 🚀 Installation

### Prerequisites
- Python 3.8 or higher
- Discord Bot Token

### Setup Steps

1. **Clone/Download the bot files**
   ```
   voicecraft-bot/
   ├── main.py
   ├── config.py
   ├── requirements.txt
   ├── .env
   └── ...
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure environment**
   Create a `.env` file:
   ```env
   DISCORD_TOKEN=your_bot_token_here
   ```

4. **Run the bot**
   ```bash
   python main.py
   ```

## 📋 Bot Commands

### Admin Commands
- `/setup` - Configure VoiceCraft in your server
- `/settings` - View current server settings
- `/cleanup` - Manually cleanup empty voice channels

### User Commands
- `/panel` - Open voice channel control panel
- `/invite @user` - Invite user to your voice channel
- `/help` - Show help information
- `/about` - About VoiceCraft with live statistics

## 🔧 Bot Setup in Discord

### Required Permissions
- ✅ Manage Channels
- ✅ Manage Roles
- ✅ Move Members
- ✅ View Channels
- ✅ Send Messages
- ✅ Embed Links
- ✅ Connect
- ✅ Speak

### Setup Process
1. Invite the bot to your server with the required permissions
2. Use `/setup` command as an administrator
3. Select:
   - **Join Channel** - Where users join to create channels
   - **Category** - Where temporary channels will be created
   - **Log Channel** (Optional) - For bot activity logs

4. Users can now join the designated channel to create their own voice channels!

## 📊 How It Works

1. **User joins** the designated "join-to-create" channel
2. **Bot creates** a personal voice channel with unique ID
3. **User becomes owner** with full control
4. **Control panel** appears in text channel
5. **Owner can customize**:
   - Rename channel
   - Adjust bitrate (8-96kbps)
   - Set user limit
   - Lock/unlock channel
   - Invite friends
6. **Auto cleanup** when channel is empty for 60 seconds

## 🔐 Security Features

- No hardcoded user IDs
- Proper permission checks
- Database encryption
- Rate limiting
- Error handling
- Logging system

## 🐛 Troubleshooting

### Common Issues

1. **Bot doesn't create channels**
   - Check bot permissions
   - Ensure `/setup` was completed
   - Verify join channel ID is correct

2. **Channels not deleting**
   - Check if bot has Manage Channels permission
   - Wait 60 seconds after channel empties

3. **Roles not working**
   - Ensure bot has Manage Roles permission
   - Check role hierarchy (bot role must be above created roles)

### Logs
Check `voicecraft.log` for detailed error information.

## 🤝 Support

- **Support Server**: [Join Discord](https://discord.gg/voicecraft)
- **GitHub**: [VoiceCraft Repository](https://github.com/TheshanBMR/voicecraft-bot)
- **Issures**: [Report Issues](https://github.com/TheshanBMR/voicecraft-bot/issues)

## 📄 License

MIT License - See LICENSE file for details.

---

Made with Python by the VoiceCraft Team
