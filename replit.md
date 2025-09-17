# Discord Verification Bot

## Overview
This is a Discord verification bot imported from GitHub that manages user verification and welcome systems in Discord servers. The bot is written in Node.js using Discord.js v13 and includes comprehensive role management and welcome message features.

## Project Structure
- `index.js` - Main bot file with full feature set (verification + welcome system)
- `index_simple.js` - Simplified version with basic verification only
- `config.json` - Bot configuration (prefix and developer ID)
- `database.json` - JSON-based storage for server configurations
- `package.json` - Node.js dependencies

## Current Status
✅ **Fully Operational** - Bot is running successfully in Replit environment
- Connected to Discord as: magiura.#7009
- Loaded 25 commands successfully
- Keep-alive server running on port 5000
- Deployment configuration set for VM hosting

## Key Features
### Verification System
- Set verification channel and roles
- Auto role assignment on verification
- Role removal functionality
- Bulk verification reset

### Welcome System  
- Customizable welcome messages
- Auto role assignment for new members
- Auto-delete welcome messages
- Welcome message testing

### Administration
- Permission-based command access
- Comprehensive help system
- Portuguese language interface

## Technical Setup
- **Language**: Node.js
- **Framework**: Discord.js v13
- **Port**: 5000 (configurable via PORT env var)
- **Database**: JSON file-based storage
- **Secrets**: Discord bot TOKEN managed via Replit Secrets

## Important Notes
⚠️ **Required Discord Settings**: For full functionality, enable these in Discord Developer Portal:
- Server Members Intent (for member management)
- Message Content Intent (for command processing)

## Bot Commands
All commands use prefix: `.`

**Verification Commands:**
- `.setverify` - Set verification channel
- `.setrole` - Set verification role
- `.verify` - Verify user
- `.resetallverify` - Remove verification from all members

**Welcome Commands:**
- `.great` - Welcome system control panel
- `.setwelcome` - Set welcome channel
- `.setwelcomerole` - Set auto-role for new members

**Admin Commands:**
- `.help` - Show all commands
- Various reset commands for configuration management

## Recent Changes
- Fixed syntax error in index_simple.js
- Updated port configuration to use environment variable
- Configured for Replit deployment
- Set up proper secrets management