# AI Email Summary Automation

An n8n learning project that connects Gmail, OpenAI, and Google Sheets to record incoming emails and generate short summaries.

## What it does

- Detects incoming inbox emails, excluding emails sent by the connected account.
- Saves the date, sender, subject, message, and email ID to Google Sheets.
- Checks the month and usage count before the AI step.
- Uses OpenAI to summarize the main topic, important details, and required actions.
- Sends the summary to a configured email address.
- Updates the email record with its summary and completion status.

## Tools used

- n8n
- Gmail
- Google Sheets
- OpenAI

## What I practiced

- Connecting services through credentials
- Mapping data between workflow nodes
- Writing n8n expressions
- Building conditional branches
- Creating prompts for email summaries
- Troubleshooting missing fields and expression errors

## Current status

This is a learning prototype. Email recording and summarization have been tested during development.

The monthly usage control is incomplete: the workflow checks whether the count is below 10, but does not yet increase the counter or reset it for a new month. It should not be treated as a working monthly spending limit.

## Planned improvements

- Complete and test monthly usage tracking
- Handle multiple emails correctly in one execution
- Prevent duplicate records
- Add error handling and clearer processing statuses

## Author

Sumon Boiddo
