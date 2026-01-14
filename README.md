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
chell lmstudio
```

A QR code will appear in your terminal. Scan it with the Chell mobile app to start coding.

### Permission Modes

To run Claude Code in `--dangerously-skip-permissions` mode, use the `--yolo` flag:

```bash
chell claude --yolo
```

For cloud environments, visit "Experimental Flags" in the Account Settings menu on the iOS app to change the permission mode.

## Daemon

For the best experience, ensure the daemon is running. This enables seamless mobile terminal connection.

```bash
chell daemon start       # Start the daemon (runs in background)
chell daemon stop        # Stop the daemon (sessions stay alive)
chell daemon status      # Show daemon status
chell daemon list        # List active sessions
```

The daemon starts automatically when you launch a session.

## Notifications

Chell sends push notifications to your mobile device when Claude requests permission or completes a task. You can configure notification behavior using the settings command.

### Notification Modes

```bash
chell settings notifications           # Show current setting
chell settings notifications local     # Only notify in local/interactive mode
chell settings notifications remote    # Only notify in remote mode
chell settings notifications both      # Notify in both modes (default)
chell settings notifications neither   # Never send notifications
```

**Modes explained:**
- `local` - Send push notifications only when you're using Claude interactively in the terminal
- `remote` - Send push notifications only when controlling Claude from the mobile app
- `both` - Send push notifications in all modes (default)
- `neither` - Disable all push notifications

### Minimum Duration

To avoid notification spam for quick tasks, you can set a minimum duration threshold. Notifications will only be sent for prompts that take longer than the specified time:

```bash
chell settings minDuration             # Show current setting
chell settings minDuration 0           # Always notify (default)
chell settings minDuration 30          # Only notify for prompts > 30 seconds
chell settings minDuration 60          # Only notify for prompts > 1 minute
```

### Manual Notifications

You can also send custom push notifications:

```bash
chell notify -p "Deployment complete!"
chell notify -p "Build finished" -t "CI/CD"
```

**Note:** Notifications from permission hooks only trigger for Chell-managed Claude sessions. If you run Claude Code directly (not through `chell claude`), no notifications will be sent.

## Settings

```bash
chell settings                         # Show available settings
chell settings notifications [value]   # Configure push notifications
chell settings minDuration [seconds]   # Set minimum prompt duration for notifications
```

## Terminal

Control the interactive terminal (PTY) feature:

```bash
chell terminal enable    # Enable PTY terminal (default)
chell terminal disable   # Disable PTY terminal
chell terminal status    # Show current status
```

## Authentication

```bash
chell auth               # Manage authentication
chell reauth             # Reset auth to connect from a new device
```

## Diagnostics

```bash
chell doctor             # Run diagnostics and troubleshooting
chell doctor clean       # Kill any runaway Chell processes
```

## LM Studio (Local LLMs)

Run local language models through LM Studio:

```bash
chell lmstudio
chell lmstudio --base-url http://localhost:1234  # Custom LM Studio URL
```

You can also set the base URL via environment variable:
```bash
export LMSTUDIO_BASE_URL=http://localhost:1234
chell lmstudio
```

## Requirements

- Node.js 20.0.0 or higher
- At least one AI assistant CLI installed

## Support

See [SUPPORT.md](./SUPPORT.md) for all support options.

- Join our Discord for quick questions: https://discord.gg/2gwYUwve58
- Open GitHub issues for bugs/feature requests: https://github.com/Cerulin/Chell/issues
- Email us directly: contact@cerulin.com

## License

MIT
