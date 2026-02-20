# Chell

An integrated workspace for your AI coding agents. Manage all your agents from one organized spot, monitor and continue prompts from your phone, with built-in terminals and file editors to stay productive when away from your desk. End-to-end encrypted.

<p align="center">
  <img src="assets/chellgif.gif" alt="Chell Demo">
</p>

<p align="center">
  <a href="https://discord.gg/r9putKU2Dp"><img src="https://img.shields.io/discord/1404665022440800397?color=5865F2&logo=discord&logoColor=white" alt="Discord"></a>
</p>

<p align="center">
  <a href="https://apps.apple.com/au/app/chell/id6754867036"><img src="https://developer.apple.com/assets/elements/badges/download-on-the-app-store.svg" alt="Download on the App Store" height="50"></a>
  <a href="https://play.google.com/store/apps/details?id=com.cerulin.chell"><img src="https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png" alt="Get it on Google Play" height="68"></a>
</p>

## Installation

Click a button below to install the application:

<p align="center">
  <a href="https://github.com/Cerulin/Chell/releases/latest/download/chell-desktop-setup.exe"><img src="https://img.shields.io/badge/Windows-Download-0078D4?logo=windows&logoColor=white" alt="Windows"></a>
  <a href="https://github.com/Cerulin/Chell/releases/latest/download/chell-desktop-arm64.dmg"><img src="https://img.shields.io/badge/macOS_ARM-Download-000000?logo=apple&logoColor=white" alt="macOS ARM"></a>
  <a href="https://github.com/Cerulin/Chell/releases/latest/download/chell-desktop-x64.dmg"><img src="https://img.shields.io/badge/macOS_Intel-Download-000000?logo=apple&logoColor=white" alt="macOS Intel"></a>
  <a href="https://github.com/Cerulin/Chell/releases/latest/download/chell-desktop-x86_64.AppImage"><img src="https://img.shields.io/badge/Linux-Download-FCC624?logo=linux&logoColor=black" alt="Linux"></a>
</p>

### What if I don't want the Desktop app, but I want a CLI?

**Linux / macOS:**
```bash
curl -fsSL https://raw.githubusercontent.com/Cerulin/Chell-CLI-releases/main/install/install.sh | bash
```

**Windows (PowerShell):**
```powershell
irm https://raw.githubusercontent.com/Cerulin/Chell-CLI-releases/main/install/install.ps1 | iex
```

**Windows (Command Prompt):**
```cmd
curl -fsSL https://raw.githubusercontent.com/Cerulin/Chell-CLI-releases/main/install/install.cmd -o install.cmd && install.cmd && del install.cmd
```

No dependencies required — Chell CLI is a standalone binary. Run the same install command again to update.

## Prerequisites

It is required to have one CLI installed first:

- **[Claude Code](https://github.com/anthropics/claude-code)**
- **[OpenAI Codex](https://github.com/openai/codex)**
- **[Google Gemini](https://github.com/google-gemini/gemini-cli)**
- **[LM Studio](https://lmstudio.ai/)**

## Usage

**[View all commands](./COMMANDS.md)**

## Roadmap

- Full Codex, Gemini, and OpenCode integration
- Resume terminal/conversation fully on app or computer restart
- Replacing QR Code authentication with global email/pass authentication
- Multi-tab terminal interface
- Custom terminal launch scripts/profiles
- Settings UI and configuration
- Request a terminal from your phone
- Sync chats across all devices (iPad, iPhone, Desktop, Cloud)
- Seamless Chell-Cloud handoff when your computer is asleep

## Our Commitment to Safe Data Practices

Your code is your code. All Chell products are end-to-end encrypted, meaning we can never see your code, prompts, or conversations. Your data stays between your devices and your AI agents—nobody else.

## Support

See [SUPPORT.md](./SUPPORT.md) for all support options.

- Join our Discord for quick questions: https://discord.gg/r9putKU2Dp
- Open GitHub issues for bugs/feature requests: https://github.com/Cerulin/Chell/issues
- Email us directly: contact@cerulin.com

## License

UNLICENSED
