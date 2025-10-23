# Chell

Code from anywhere with AI assistance on your mobile device.

## Installation

```bash
npm install -g codebridge
```

## Prerequisites

It is highly recommended (but optional) that you have the respective AI CLI tools installed first:

- **Claude Code**: `npm install -g @anthropic-ai/claude-code`
- **OpenAI Codex**: Install the Codex CLI
- **Google Gemini**: Install the Gemini CLI

## Getting Started

Start a coding session with your preferred AI assistant:

```bash
codebridge claude
codebridge codex
codebridge gemini
```

A QR code will appear in your terminal. Scan it with the CodeBridge mobile app to start coding.

## Daemon

For the best experience, ensure the daemon is running. This enables seamless mobile terminal connection.

```bash
codebridge daemon start
codebridge daemon stop
```

The daemon starts automatically when you launch a session.

## Requirements

- Node.js 20.0.0 or higher
- At least one AI assistant CLI installed

## License

MIT
