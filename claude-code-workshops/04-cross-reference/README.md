# Cross-Reference & Compliance

| | |
|---|---|
| **What you'll learn** | How to use Claude Code to verify data across files and handle tracked changes in Word documents |
| **Time** | ~10 minutes |
| **Prerequisites** | Claude Code running from the `claude-code-workshops` root folder, document skills installed (see module 02) |

## Step 1: Cross-Reference the Files

Ask Claude to compare data across Excel and Word:

```
Does the disputed amount in static/dispute_letter.docx match the total disputed transactions in static/dispute_transactions.xlsx? If not, update the letter with the correct amount. Use npm packages.
```

Claude reads both files, compares the amounts, and fixes any discrepancy — the kind of cross-file verification that's error-prone when done manually.

## Step 2: Review Compliance Feedback

The letter has been through compliance review. See what they said:

```
Show me all tracked changes and comments in static/dispute_letter.docx
```

## Step 3: Accept Changes and Respond

Handle the feedback:

```
Accept all tracked changes in static/dispute_letter.docx
```

Then address the compliance comments:

```
Update static/dispute_letter.docx: add a sentence mentioning that we've filed a fraud report with the card network, then reply to the compliance reviewer's comment confirming it's been addressed. Save the file.
```

## Step 4: Final Verification

Confirm everything is consistent:

```
Verify that the letter includes all disputed transactions listed in the spreadsheet and that the timeline is consistent between both files
```

## What You Learned

- Claude Code can work across multiple file types (Excel + Word) simultaneously
- Tracked changes and inline comments in Word documents can be reviewed, accepted, and responded to
- Cross-file data verification that typically takes 30+ minutes per case becomes a conversation
