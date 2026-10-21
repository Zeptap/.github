<p align="center">
  <a href="https://zeptap.com"><img src="https://raw.githubusercontent.com/Zeptap/mcp/main/.github/assets/hero.png" alt="Zeptap: let AI agents use a real iPhone" width="100%"></a>
</p>

<p align="center">
  <b>Let AI agents see, tap, swipe and type on a real iPhone, from your Mac.</b>
</p>

<p align="center">
  <a href="https://github.com/Zeptap/releases/releases/latest/download/Zeptap.dmg"><img src="https://img.shields.io/badge/Download_for_Mac-000000?style=for-the-badge&logo=apple&logoColor=white" alt="Download for Mac"></a>
  &nbsp;
  <a href="https://zeptap.com/docs"><img src="https://img.shields.io/badge/Docs-3B82F6?style=for-the-badge" alt="Docs"></a>
  &nbsp;
  <a href="https://zeptap.com/pricing"><img src="https://img.shields.io/badge/Pricing-22C55E?style=for-the-badge" alt="Pricing"></a>
</p>

Zeptap is a Mac app that lets AI agents like Claude Code, Codex and Cursor operate a real iPhone through a local MCP server. The Mac reads the screen over the USB cable and sends taps and typing over Bluetooth through AssistiveTouch, so nothing is installed on the phone: no Xcode, no Developer Mode, no Apple Developer account. Everything runs on your Mac, with no account and no cloud relay.

Use it to test your own iOS apps on a physical device, or to hand everyday phone tasks to the agent you already use.

> "open my app and walk through signup" · "screenshot every screen in dark mode" · "turn on Low Power Mode"

### Get started

```sh
brew install --cask zeptap/tap/zeptap
claude mcp add --transport http --scope user zeptap http://127.0.0.1:47801/mcp
```

Connect your iPhone by USB, pair Bluetooth in the setup assistant, then ask your agent to take a screenshot. Setup for Claude Desktop, Codex, Cursor and other clients is in the [docs](https://zeptap.com/docs/agents/connect).

### Repositories

| Repo | What's in it |
| --- | --- |
| [**mcp**](https://github.com/Zeptap/mcp) | MCP client configs, a Claude Code plugin, an agent skill and the `@zeptap/mcp` stdio relay |
| [**releases**](https://github.com/Zeptap/releases) | Downloads and release notes for the Mac app |
| [**homebrew-tap**](https://github.com/Zeptap/homebrew-tap) | `brew install --cask zeptap/tap/zeptap` |

### Links

[Website](https://zeptap.com) · [Docs](https://zeptap.com/docs) · [MCP tool reference](https://zeptap.com/docs/agents/tools) · [Claude + iPhone guide](https://zeptap.com/docs/guides/claude-iphone) · [Blog](https://zeptap.com/blog) · [Support](mailto:support@zeptap.com)

<sub>Requires a Mac on macOS 14 or later with Bluetooth, and an iPhone with a USB cable. The Mac app is closed source with the first hour of live use free; the repos here are MIT.</sub>
