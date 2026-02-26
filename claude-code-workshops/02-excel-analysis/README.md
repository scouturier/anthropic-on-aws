# Excel Analysis

In this module, you'll learn how to use Claude Code to read Excel files, identify suspicious data using cell styles, add computed columns, and build summary tables — all without writing a single formula.

## Setup: Install Document Skills

Before starting, install the document skills in Claude Code:

1. Add the skills marketplace:
```
/plugin marketplace add anthropics/skills
```

2. Install the document skills:
```
/plugin install document-skills@anthropic-agent-skills
```

3. Exit and restart Claude Code to load the skills:
```
/quit
claude
```

> **Note:** If Claude tries to use Python for document processing, tell it to use npm/Node.js instead.

## The Scenario

The `static/dispute_transactions.xlsx` file contains 10 transactions from Robert Chen's account between February 14-17, 2026. Some are legitimate. Some aren't. Let's find out which.

## Step 1: Calculate the Disputed Total

```
Open static/dispute_transactions.xlsx and calculate the total of all transactions that are highlighted in red (suspicious ones). Use npm packages.
```

Watch how Claude unpacks the Excel file, reads the cell styles to identify highlighted rows, and computes the total. No formulas to write, no manual selection.

## Step 2: Flag Unusual Activity

Fraudulent transactions often happen at odd hours. Add an analysis column:

```
Add a column that flags any transaction occurring between 1 AM and 5 AM as "Unusual Time"
```

Claude identifies the time data, adds a new column, and applies the logic — the kind of analysis that takes 10 minutes manually.

## Step 3: Build a Summary Table

```
Create a summary table showing the count and total amount for legitimate vs disputed transactions
```

> **Try Your Own Analysis**
>
> The spreadsheet has TODO items marked in it. Try asking Claude to complete them, or come up with your own analysis — "Which merchant categories appear in the disputed transactions?" or "Are there any duplicate amounts?"

## What You Learned

- Claude Code can read Excel files including cell styles and formatting
- You can add computed columns and summaries conversationally
- Analysis that takes 20-30 minutes manually can be done in about 3 minutes
