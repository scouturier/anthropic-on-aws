# Claude Code Workshops — Additional Modules

Additional hands-on modules for the Claude Code on Amazon Bedrock workshop. Each module is self-contained and can be run independently.

## Modules

| Module | Description |
|--------|-------------|
| [Document Analysis](01-document-analysis/) | Synthesize insights across multiple documents — meeting notes, research, and reports |
| [Excel Analysis](02-excel-analysis/) | Analyze spreadsheet data, flag anomalies, and build summaries using Claude Code |
| [Data Analysis](03-data-analysis/) | Statistical analysis, visualization, and stakeholder-ready report generation |
| [Cross-Reference & Compliance](04-cross-reference/) | Verify data across Word and Excel files, handle tracked changes and compliance review |
| [Jira MCP Integration](05-jira-integration/) | Connect Claude Code to a mock Jira server via MCP to manage tickets and workflows |

## Prerequisites

- Completed the base Claude Code on Amazon Bedrock workshop setup
- Claude Code installed and configured with Amazon Bedrock

## Getting Started

1. Clone this repo and `cd` into the `claude-code-workshops` folder
2. Launch Claude Code from here: `claude`
3. Pick any module and follow its README

Each module's prompts use specific folder paths (e.g. `01-document-analysis/meeting-notes/`) so Claude Code stays scoped to the right files. The `static/` folder contains shared demo files (spreadsheets, documents, and the mock Jira MCP server) used across modules.
