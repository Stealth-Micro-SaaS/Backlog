# Kanban Management Instructions

This guide explains how to manage tickets using GitHub Projects in this repository, whether you are a human or an AI agent.

## Core Operations

### 1. View Tickets
To view the current state of the board:
- **Web Interface**: Navigate to the "Projects" tab in the GitHub organization or repository.
- **AI/CLI**: Use the GitHub MCP server or `gh project item-list` to fetch the current status of all items.

### 2. Create a Ticket
Tickets should be created as **Issues** first and then added to the Project board.
- **Human**: Create a new issue on GitHub and assign it to the Project.
- **AI**: 
    1. Create an issue via the `create_issue` tool.
    2. Add the issue to the project using the `add_project_item` tool (requires `GITHUB_PROJECT_NUM`).

### 3. Move/Update Ticket Status
The Kanban board typically has columns: `Todo`, `In Progress`, `Done`.
- **Human**: Drag and drop cards between columns.
- **AI**: Use the `update_project_item_field` tool to change the "Status" field of a project item.

### 4. Edit Tickets
- Always keep the description updated with progress.
- Use labels (e.g., `bug`, `feature`, `priority`) to categorize tasks.

## Workflow Conventions

- **Atomic Tasks**: Each ticket should represent a single, actionable unit of work.
- **Status Updates**: When work begins, move the ticket to `In Progress`.
- **Completion**: Move to `Done` only after verification/testing is complete.

## Automation with MCP

The `.github/mcp-server/config.json` file allows AI agents to perform these actions automatically. Ensure the agent has a PAT with `repo` and `project` scopes.
