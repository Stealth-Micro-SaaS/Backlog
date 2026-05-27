# GitHub MCP Automation Setup

This directory contains the configuration for the GitHub Model Context Protocol (MCP) server. 
The MCP server allows external AI agents to interact with GitHub's GraphQL and REST APIs.

## Configuration

The `config.json` file defines how to start the GitHub MCP server. 

### Prerequisites

- A GitHub Personal Access Token (PAT) with `repo`, `project`, and `workflow` scopes.
- Node.js installed on your machine.

### Usage

1. Copy your PAT into the `GITHUB_PAT_TOKEN` field in your local `.env` file (see `.env.example`).
2. AI agents can use the configuration in `config.json` to initialize the connection.
