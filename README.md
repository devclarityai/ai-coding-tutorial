# AI Coding Tutorial

This is a website to help you learn how to use AI coding assistants.

## Walkthrough

1. Mode Explanation - Understanding & Writing/Prediction
2. Understanding - Codebase
3. Understanding - Tagging
  a. Open files, documentation, the web
4. Writing - Inline Code
5. Writing - Simple Ask
  a. The "Learn More About Our Features" button on the @index.html page doesn't animate in with the rest of the features section, so it looks weird.
6. Writing - Workflow
  a. We need to create a contact page and then also update the links on the @index.html and @features.html pages to point to this. For now, we can use the same styling we have on other pages and we can build a basic contact form that you would usually see on a website. Create the tasks for this, don't implement it yet. @task-creator.mdc
  b. markdown-file.md Great, now @implement-it.mdc

## Browser Tools MCP

**Note: you already have the BrowserTools code in this directory, so you do not need to clone them again.**

1. Starting at step 2, follow the [BrowserTools MCP server](https://browsertools.agentdesk.ai/installation) installation steps.
  a. These steps include installing a Chrome extension.
2. Start the server.
  a. npx @agentdeskai/browser-tools-server@1.2.0

### Experiment

First, go to styles.css and change `.hero h1` and `.hero p` color to `#FFFFFF`.

1. Open /web-app/index.html in your browser as the focused tab.
2. Right click and click inspect. Click "BrowserToolsMCP".
3. In Cursor/Windsurf, copy the path to your current directory. Paste this in Screenshot Settings path.
4. Open your agent chat. Say `Our text colors do not look right. Take a screenshot and fix @index.html`

## `mcp.json`

### MacOS

{
  "mcpServers": {
    "browser-tools": {
      "command": "npx",
      "args": [
        "-y",
        "@agentdeskai/browser-tools-mcp@1.2.0"
      ],
      "enabled": true
    }
  }
}

### Windows

{
  "mcpServers": {
    "browser-tools": {
      "command": "wsl",
      "args": [
        "bash",
        "-c",
        "cmd /c npx -y @agentdeskai/browser-tools-mcp@1.2.0"
      ],
      "enabled": true
    }
  }
}
