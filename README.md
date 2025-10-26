# Shippi - AI-Powered Development Platform

This repository contains the core technology that powers **Shippi** - an innovative AI-powered development platform that enables interactive terminal sessions and AI coding assistance through Telegram.

## What is Shippi?

Shippi leverages **coderBOT** technology to provide developers with secure, remote access to AI coding assistants (GitHub Copilot, Claude, Cursor) directly through Telegram. This creates a seamless workflow for coding, debugging, and managing projects from anywhere.

## The Technology: coderBOT

The underlying technology, **coderBOT**, provides:

- 🖥️ **Interactive Terminal Access** - Full terminal sessions via Telegram with PTY support
- 🤖 **AI Coding Assistant Integration** - Works with GitHub Copilot CLI, Claude CLI, Cursor CLI, or any command-line AI tool
- 🔐 **Robust Security** - Environment-based authentication with auto-kill on unauthorized access
- 📸 **Visual Feedback** - Real-time terminal screenshots using Puppeteer
- 📁 **Media Management** - Automatic file watching and delivery
- 🔄 **Session Management** - Multiple concurrent sessions with intelligent timeout handling
- 🎮 **Administrative Control** - ControlBOT for managing worker processes

## Learn More

For comprehensive information about Shippi and how to get started:

👉 **Visit [shippi.art](https://shippi.art)**

The Shippi website provides:
- Complete documentation and tutorials
- Use cases and examples
- Community resources
- Support and contact information

## Quick Start

### Option 1: Run with npx (Fastest)

```bash
# Run instantly with npx
npx @tommertom/coderbot@latest
```

On first run, it will create a `.env` file for configuration. See the [coderBOT directory](../coderBOT/) for full documentation.

### Option 2: Run with Docker

To run coderBOT in a containerized environment:

1. **Create a `.env` file** in the project root with your configuration:
   ```bash
   # Required: Your Telegram Bot Token
   TELEGRAM_BOT_TOKEN=your_bot_token_here
   
   # Optional: Additional configuration
   # ALLOWED_CHAT_IDS=123456789,987654321
   ```

2. **Build and start the container**:
   ```bash
   docker-compose up -d
   ```

3. **View logs**:
   ```bash
   docker-compose logs -f
   ```

4. **Stop the container**:
   ```bash
   docker-compose down
   ```

The Docker setup includes:
- Pre-installed GitHub CLI and Copilot CLI
- Persistent logs in `./logs` directory
- Automatic media file management
- Auto-restart on failure

## Repository Structure

- `/coderBOT` - Core coderBOT technology and implementation
- This repository - Integration and deployment for Shippi platform

## Contributing

Interested in contributing to Shippi? Visit [shippi.art](https://shippi.art) for contribution guidelines and community information.

## License

MIT License - See LICENSE file for details

---

**Learn more about Shippi at [shippi.art](https://shippi.art)**
