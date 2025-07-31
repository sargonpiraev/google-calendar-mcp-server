# Google Calendar API MCP Server 🔧

![npm version](https://img.shields.io/npm/v/@sargonpiraev/google-calendar-mcp-server)
![npm downloads](https://img.shields.io/npm/dw/@sargonpiraev/google-calendar-mcp-server)
![license](https://img.shields.io/github/license/sargonpiraev/google-calendar-mcp-server)
![pipeline status](https://gitlab.com/sargonpiraev/google-calendar-mcp-server/badges/main/pipeline.svg)
![smithery badge](https://smithery.ai/badge/@sargonpiraev/google-calendar-mcp-server)
![MCP Compatible](https://img.shields.io/badge/MCP-Compatible-blue)
[![Join Discord](https://img.shields.io/discord/1331631275464671347?color=7289da&label=Discord&logo=discord)](https://discord.gg/ZsWGxRGj)



## Features

- 🔌 **Seamless AI Integration**: Direct Google Calendar API API access from Claude, Cursor, and VS Code
- 🤖 **Automated Workflows**: Automate Google Calendar API operations and data access
- 📊 **Complete API Coverage**: 37+ tools covering all major Google Calendar API features
- ⚡ **Real-time Access**: Access Google Calendar API data instantly from AI assistants
- 🔧 **Professional Integration**: Error handling, validation, and comprehensive logging

## Get Your Credentials

Before installation, you'll need a Google Calendar API API key:

1. Open Google Calendar API app or web interface
2. Go to **Settings → Account → API Access**
3. Generate new API key or copy existing one
4. Save this key for the installation steps below

## Requirements

- Node.js >= v18.0.0
- Google Calendar API API key
- Cursor, VS Code, Claude Desktop or another MCP Client

## Installation

<details>
<summary><b>Installing via Smithery</b></summary>

To install Google Calendar API MCP Server for any client automatically via [Smithery](https://smithery.ai):

```bash
npx -y @smithery/cli@latest install @sargonpiraev/google-calendar-mcp-server --client <CLIENT_NAME>
```

</details>

<details>
<summary><b>Install in Cursor</b></summary>

#### Cursor One-Click Installation

[![Install MCP Server](https://cursor.com/deeplink/mcp-install-dark.svg)](https://cursor.com/install-mcp?name=@sargonpiraev/google-calendar-mcp-server&config=)

#### Manual Configuration

Add to your Cursor `~/.cursor/mcp.json` file:

```json
{
  "mcpServers": {
    "google-calendar-mcp-server": {
      "command": "npx",
      "args": ["-y", "@sargonpiraev/google-calendar-mcp-server"],
      "env": {
        "GOOGLE-CALENDAR_CLIENT_ID": "your-google-calendar_client_id",
        "GOOGLE-CALENDAR_CLIENT_SECRET": "your-google-calendar_client_secret"
      }
    }
  }
}
```

</details>

<details>
<summary><b>Install in VS Code</b></summary>

[![Install in VS Code](https://img.shields.io/badge/VS_Code-Install_MCP-0098FF)](vscode:mcp/install?%7B%22name%22%3A%22google-calendar-mcp-server%22%2C%22command%22%3A%22npx%22%2C%22args%22%3A%5B%22-y%22%2C%22@sargonpiraev/google-calendar-mcp-server%22%5D%7D)

Or add manually to your VS Code settings:

```json
"mcp": {
  "servers": {
    "google-calendar-mcp-server": {
      "type": "stdio",
      "command": "npx",
      "args": ["-y", "@sargonpiraev/google-calendar-mcp-server"],
      "env": {
        "GOOGLE-CALENDAR_CLIENT_ID": "your-google-calendar_client_id",
        "GOOGLE-CALENDAR_CLIENT_SECRET": "your-google-calendar_client_secret"
      }
    }
  }
}
```

</details>

<details>
<summary><b>Install in Claude Desktop</b></summary>

Add to your `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "google-calendar-mcp-server": {
      "command": "npx",
      "args": ["-y", "@sargonpiraev/google-calendar-mcp-server"],
      "env": {
        "GOOGLE-CALENDAR_CLIENT_ID": "your-google-calendar_client_id",
        "GOOGLE-CALENDAR_CLIENT_SECRET": "your-google-calendar_client_secret"
      }
    }
  }
}
```

</details>

## Available Tools

- **`list-acl`**: List access control rules
- **`insert-acl`**: Create access control rule
- **`get-acl`**: Get access control rule
- **`update-acl`**: Update access control rule
- **`patch-acl`**: Patch access control rule
- **`delete-acl`**: Delete access control rule
- **`watch-acl`**: Watch for changes to ACL resources
- **`list-calendar-list`**: List calendars
- **`insert-calendar-list`**: Insert calendar into calendar list
- **`get-calendar-list`**: Get calendar from calendar list
- **`update-calendar-list`**: Update calendar in calendar list
- **`patch-calendar-list`**: Patch calendar in calendar list
- **`delete-calendar-list`**: Remove calendar from calendar list
- **`watch-calendar-list`**: Watch for changes to CalendarList resources
- **`insert-calendar`**: Create calendar
- **`get-calendar`**: Get calendar
- **`update-calendar`**: Update calendar
- **`patch-calendar`**: Patch calendar
- **`delete-calendar`**: Delete calendar
- **`clear-calendar`**: Clear primary calendar
- **`list-events`**: List events
- **`insert-event`**: Create event
- **`get-event`**: Get event
- **`update-event`**: Update event
- **`patch-event`**: Patch event
- **`delete-event`**: Delete event
- **`instances-event`**: Get event instances
- **`move-event`**: Move event
- **`import-event`**: Import event
- **`quick-add-event`**: Quick add event
- **`watch-events`**: Watch for changes to Events resources
- **`query-freebusy`**: Query free/busy information
- **`get-colors`**: Get color definitions
- **`list-settings`**: List settings
- **`get-setting`**: Get setting
- **`watch-settings`**: Watch for changes to Settings resources
- **`stop-channel`**: Stop watching resources

**Total: 37 tools available** 🎯

## Support This Project

Hi! I'm Sargon, a software engineer passionate about AI tools and automation. I create open-source MCP servers to help developers integrate AI assistants with their favorite services.

Your support helps me continue developing and maintaining these tools, and motivates me to create new integrations that make AI assistants even more powerful! 🚀

[![Support on Boosty](https://img.shields.io/badge/Support-Boosty-orange?logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZD0iTTEyIDJMMTMuMDkgOC4yNkwyMCA5TDEzLjA5IDE1Ljc0TDEyIDIyTDEwLjkxIDE1Ljc0TDQgOUwxMC45MSA4LjI2TDEyIDJaIiBmaWxsPSJ3aGl0ZSIvPgo8L3N2Zz4K)](https://boosty.to/sargonpiraev)

## Connect with Author

- 🌐 Visit [sargonpiraev.com](https://sargonpiraev.com)
- 📧 Email: [sargonpiraev@gmail.com](mailto:sargonpiraev@gmail.com)
- 💬 Join [Discord](https://discord.gg/ZsWGxRGj)
