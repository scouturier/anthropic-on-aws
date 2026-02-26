# Claude Code Workshops — Additional Modules

These modules extend the [Claude Code on Amazon Bedrock](https://catalog.workshops.aws/claudecode101/en-US) workshop with additional hands-on scenarios covering real-world use cases — prompt engineering, document analysis, spreadsheet processing, and tool integrations. Each module is self-contained and can be run independently, but works best after completing the base workshop.

## Modules

| Module | Description | Key techniques |
|--------|-------------|----------------|
| [Prompt Engineering](00-prompt-engineering/) | Learn how prompt quality affects output quality, and how to use Claude to improve your own prompts | Prompt improvement, clarifying questions |
| [Document Analysis](01-document-analysis/) | Synthesize insights across multiple documents — meeting notes, research, and reports | Multi-doc synthesis, timeline building |
| [Excel Analysis](02-excel-analysis/) | Analyze spreadsheet data, flag anomalies, and build summaries using Claude Code | Cell styles, computed columns |
| [Data Analysis](03-data-analysis/) | Statistical analysis, visualization, and stakeholder-ready report generation | Outlier detection, HTML charts |
| [Cross-Reference & Compliance](04-cross-reference/) | Verify data across Word and Excel files, handle tracked changes and compliance review | Tracked changes, cross-file verification |
| [Jira MCP Integration](05-jira-integration/) | Connect Claude Code to a mock Jira server via MCP to manage tickets and workflows | MCP setup, cross-tool workflows |

## Prerequisites

- Completed the base Claude Code on Amazon Bedrock workshop setup
- Claude Code installed and configured with Amazon Bedrock

## Getting Started

1. Clone this repo and `cd` into the `claude-code-workshops` folder
2. Launch Claude Code from here: `claude`
3. Pick any module and follow its README

Each module is self-contained — sample data files live inside each module's folder. Each module's prompts use specific folder paths (e.g. `01-document-analysis/meeting-notes/`) so Claude Code stays scoped to the right files.
