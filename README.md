# Backlog

A human-AI collaborative workspace for managing project tasks using GitHub Projects as a Kanban board.

## Overview

This repository serves as the central hub for project tracking. It is designed to work seamlessly with AI agents using the Model Context Protocol (MCP) to automate ticket management and workflow transitions.

## Features

- **GitHub Projects Integration**: Uses GitHub's native Kanban boards for visual task management.
- **AI-Ready**: Includes pre-configured MCP server settings for AI agent interaction.
- **Secure**: Pre-configured `.gitignore` to prevent token leakage.

## Setup

1.  **Clone the repository**:
    ```bash
    git clone https://github.com/Stealth-Micro-SaaS/Backlog.git
    cd Backlog
    ```
2.  **Configure Environment**:
    ```bash
    cp .env.example .env
    ```
    Edit `.env` and provide your `GITHUB_PAT_TOKEN` and `GITHUB_PROJECT_NUM`.

3.  **Documentation**:
    See [INSTRUCTIONS.md](./INSTRUCTIONS.md) for details on managing tickets.

## License

MIT
