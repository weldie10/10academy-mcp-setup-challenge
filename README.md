# MCP Setup Challenge - 10 Academy

This repository contains the setup and configuration for the 10 Academy MCP (Model Context Protocol) challenge, including the Tenx MCP server configuration and optimized agent rules.

## Repository Structure

```
.
├── .cursor/
│   ├── mcp.json              # MCP server configuration
│   └── rules/
│       ├── agent.mdc         # Final AI agent rules (v3)
│       ├── agent.mdc.v1      # Initial rules iteration
│       └── agent.mdc.v2      # Enhanced rules iteration
├── README.md                 # This file
├── DOCUMENTATION.md          # Detailed documentation of the setup process
├── RESEARCH_NOTES.md         # Research findings and sources
├── EXPERIMENT_LOG.md         # Rules iteration tracking
├── MCP_CONNECTION_LOG.md     # Connection attempts and troubleshooting
├── MCP_EVIDENCE.md          # Evidence capture for tool calls
├── COMMIT_HISTORY.md        # Git commit history showing iterations
└── SETUP_SUMMARY.md         # Quick reference summary
```

## Quick Start

### Prerequisites
- Cursor IDE (latest version)
- GitHub account for authentication

### Setup Steps

1. **MCP Server Configuration**
   - The `.cursor/mcp.json` file is already configured with the Tenx MCP server
   - Device type is set to "linux" (update if using a different OS)
   - Server URL: `https://mcppulse.10academy.org/proxy`

2. **Enable MCP Server in Cursor**
   - Open Cursor settings
   - Navigate to MCP servers section
   - Enable the `tenxfeedbackanalytics` server toggle
   - Click "Connect" to authenticate with GitHub
   - Complete the OAuth flow in your browser

3. **Agent Rules**
   - The agent rules are configured in `.cursor/rules/agent.mdc`
   - These rules guide the AI assistant's behavior and coding style
   - Rules are automatically applied when using Cursor's AI features

## Files

- **`.cursor/mcp.json`**: MCP server configuration for Tenx Analytics
- **`.cursor/rules/agent.mdc`**: Comprehensive agent rules based on best practices
- **`DOCUMENTATION.md`**: Detailed documentation of the setup process, challenges, and insights

## MCP Server Details

- **Name**: tenxfeedbackanalytics
- **Type**: HTTP
- **URL**: https://mcppulse.10academy.org/proxy
- **Purpose**: Logs and analyzes developer interactions with the coding agent for feedback and assessment

## Notes

- The MCP connection must remain active throughout the assessment period
- All interactions with the coding agent are automatically logged by the Tenx MCP server
- The agent rules file can be customized based on your coding preferences and project requirements
