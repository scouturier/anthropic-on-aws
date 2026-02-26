# Data Analysis

In this module, you'll learn how to use Claude Code for statistical analysis, interactive chart generation, cross-source pattern detection, and producing stakeholder-ready reports — no BI tools or Python required.

**Files used:** `static/bank_demo.xlsx`, `01-document-analysis/meeting-notes/customer-feedback-summary.md`
**Prerequisite:** Base workshop setup complete

## How this works

Claude Code doesn't just generate code — it executes it. When you ask it to analyze data, it installs the necessary npm packages, writes a script, runs it, and gives you the results, all in one conversation. Output files like HTML charts are saved directly to your working directory. You're essentially getting a data analyst that writes and runs its own code.

## Step 1: Statistical Analysis

Point Claude at the broader dataset:

```
Open static/bank_demo.xlsx and give me a statistical breakdown: averages, medians, standard deviations, and any outliers in the transaction amounts. Break it down by category if the data supports it. Use npm packages.
```

Try pushing it further:

```
Are there any correlations between transaction time of day and transaction amount? What about day of week patterns?
```

## Step 2: Generate a Visualization

Ask Claude to create an HTML chart you can open in your browser:

```
Create an HTML file called analysis.html with charts showing: 1) transaction amounts over time, 2) a breakdown by category, and 3) a histogram of transaction amounts. Use inline JavaScript so it works standalone.
```

Open the file:

```
! open analysis.html
```

> **Tip:** Don't like the colors? Want a different chart type? Just tell Claude: "Make the bar chart horizontal" or "Add a trend line to the time series." It regenerates the file.

## Step 3: Combine Multiple Sources

Bring in qualitative data alongside the financial data:

```
Read both static/bank_demo.xlsx and the customer feedback summary. Are there any patterns that connect the financial transaction data with the customer satisfaction trends? Write up your findings.
```

## Step 4: Generate a Stakeholder Report

Turn everything into a deliverable:

```
Based on all the analysis we've done in this session, generate a professional executive summary report and save it as executive-summary.md. Include: key findings, statistical highlights, risk flags, and recommended next steps. Format it so I could paste it into an email to leadership.
```

## What You Learned

- Claude Code can perform statistical analysis, identify outliers, and find correlations
- You can generate interactive visualizations as standalone HTML files
- Cross-source analysis (quantitative + qualitative) works in a single conversation
- No BI tools, Python environments, or SQL queries required

---

[← Previous: Excel Analysis](../02-excel-analysis/README.md) | [Next: Cross-Reference & Compliance →](../04-cross-reference/README.md)
