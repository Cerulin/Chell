# Chell

Code from anywhere with AI assistance on your mobile device.

## Installation

```bash
npm install -g @cerulin/chell
```

## Prerequisites

It is highly recommended (but optional) that you have the respective AI CLI tools installed first:

- **Claude Code**: `npm install -g @anthropic-ai/claude-code`
- **OpenAI Codex**: Install the Codex CLI
- **Google Gemini**: Install the Gemini CLI

## Getting Started

Start a coding session with your preferred AI assistant:

```bash
chell claude
chell codex
chell gemini
```

A QR code will appear in your terminal. Scan it with the Chell mobile app to start coding.

## Daemon

For the best experience, ensure the daemon is running. This enables seamless mobile terminal connection.

```bash
chell daemon start
chell daemon stop
```

The daemon starts automatically when you launch a session.

## Requirements

- Node.js 20.0.0 or higher
- At least one AI assistant CLI installed

## Support

If you need support, feel free to [create a GitHub issue](https://github.com/Cerulin/Chell/issues) or [join our Discord](https://discord.gg/2gwYUwve58) for direct support from the development team or to submit feature requests.

## License

MIT
