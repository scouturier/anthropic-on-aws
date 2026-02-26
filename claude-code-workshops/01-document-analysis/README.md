# Document Analysis

In this module, you'll learn how to point Claude Code at a folder of documents and extract insights you'd normally spend hours reading for — timelines, cross-document connections, stakeholder perspectives, and structured deliverables.

## The Scenario

Your `01-document-analysis/meeting-notes` folder contains 7 documents from a fictional fintech company working through a rewards program restructuring — product reviews, customer research, vendor evaluations, decision meetings, compliance reviews, a kickoff, and customer feedback.

You haven't read any of them. That's the point.

## Step 1: Build a Timeline

Point Claude at the full set of documents:

```
Read all the files in 01-document-analysis/meeting-notes and give me a timeline of what happened with this project
```

Claude reads all 7 files and gives you a chronological narrative — context that would take 30+ minutes of reading to build manually.

## Step 2: Cross-Document Synthesis

The real value is connecting information *across* documents. Try this:

```
The vendor evaluation recommended Vendor B, but the team chose Vendor A. What was the reasoning, and do you think it was the right call based on all the evidence?
```

The answer lives in *two different documents* — the vendor evaluation and the decision meeting. Claude connects them without being told which files to look at.

## Step 3: Ask Questions Like a Stakeholder

Try different perspectives:

```
I'm briefing the CEO. Give me a 5-bullet summary of where this project stands, what's at risk, and what needs attention this month.
```

```
What's still unresolved that could block the Q2 launch?
```

```
What's the total financial picture here? Include the vendor costs, churn impact, and any budget allocations mentioned across all documents.
```

```
Who are the key people involved in this project, what are their roles, and where do they disagree?
```

## Step 4: Generate a Deliverable

Turn the documents into a structured output:

```
Based on all the meeting notes, create a project status report in markdown that I could send to leadership. Include timeline, budget, risks, and open action items.
```

You just turned 7 scattered documents into a structured deliverable in seconds.

## What You Learned

- Claude Code can read and synthesize across multiple documents at once
- You don't need to tell it which file contains which detail — it finds connections automatically
- Any file-based content (meeting notes, research, policy docs, RFPs) can be analyzed this way
