# Jira MCP Integration

In this module, you'll learn how to connect Claude Code to external tools using Model Context Protocol (MCP). You'll set up a mock Jira server, search and update tickets, and run cross-tool workflows — all from the terminal.

## Setup: Install the Mock Jira Server

Exit Claude Code if it's running:

```
/quit
```

Install dependencies and register the MCP server:

```
cd 05-jira-integration/mock-jira-mcp
npm install
cd ../..
claude mcp add jira -- node 05-jira-integration/mock-jira-mcp/server.js
```

Start Claude Code to load the MCP server:

```
claude
```

> **What is MCP?**
>
> Model Context Protocol (MCP) is an open standard that lets AI assistants connect to external tools and data sources. When you add an MCP server to Claude Code, it gains new capabilities — in this case, the ability to search, create, and update Jira issues.

## Step 1: Explore Existing Tickets

```
Search for all Jira issues in the FRAUD project
```

You should see:
- **FRAUD-101** — The main investigation ticket (In Progress)
- **FRAUD-102** — Cross-reference task from compliance (To Do)
- **FRAUD-103** — File fraud report with card network (To Do)

Get details on the main ticket:

```
Show me the full details and comments on FRAUD-101
```

## Step 2: Update the Investigation

Add findings to the main ticket:

```
Add a comment to FRAUD-101 summarizing what we found: 4 suspicious transactions totaling $1,247.85, all occurring between 1-4 AM from unusual locations. Transaction analysis complete in dispute_transactions.xlsx.
```

Transition the verification task:

```
Move FRAUD-102 to "Done" and add a comment that the letter amount has been verified and corrected to match the spreadsheet total of $1,247.85
```

## Step 3: Cross-Tool Workflow

Ask Claude to work across files and Jira together:

```
Based on the analysis we did in dispute_transactions.xlsx, create a new Jira task in the FRAUD project to follow up with the customer within 5 business days. Include the disputed amount and number of suspicious transactions in the description.
```

> **Try More!**
>
> - "Transition FRAUD-103 to In Progress and add a comment that we're filing the report today"
> - "Search for all high priority issues assigned to Jane Smith"
> - "Create a subtask for FRAUD-101 to archive the investigation documents"

## What You Learned

- MCP servers let Claude Code connect to external tools like Jira
- You can search, create, update, and transition tickets conversationally
- Cross-tool workflows (files + Jira) work in a single session
- MCP servers exist for thousands of tools: [community sources](https://github.com/modelcontextprotocol/servers) and third-party repositories
