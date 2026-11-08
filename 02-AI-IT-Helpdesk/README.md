# AI IT Helpdesk Ticket Automation

## Project Overview

An AI-powered IT helpdesk ticket automation workflow built using n8n, OpenAI GPT-4.1, Gmail, and Google Sheets.

The workflow monitors incoming IT support emails, checks for duplicate tickets, analyzes technical issues using AI, and records structured tickets in Google Sheets.

## Key Features

- **Automated Email Monitoring:** Detects incoming IT support requests through Gmail.
- **Duplicate Ticket Checking:** Checks existing records using the Gmail message ID.
- **AI Issue Classification:** Categorizes issues as Hardware, Software, Network, Account, or Other.
- **Priority Assignment:** Assigns Low, Medium, or High priority based on the reported issue.
- **AI Summary:** Generates a short description of the technical problem.
- **Suggested Solutions:** Provides initial troubleshooting recommendations.
- **Human Review:** Flags issues that may require manual review.
- **Ticket Logging:** Saves ticket information automatically in Google Sheets.

## Technologies Used

- n8n – Workflow automation
- OpenAI GPT-4.1 – AI issue analysis
- Gmail – Email monitoring
- Google Sheets – Ticket storage
- JSON – Workflow configuration

## Workflow Process

1. Gmail Trigger detects a new IT support email.
2. Google Sheets checks whether the email has already been recorded.
3. An IF node filters duplicate records.
4. GPT-4.1 analyzes the email and generates classification, priority, summary, and suggested solution.
5. Google Sheets records the ticket with an Open status.
6. Another IF node checks whether human review is required.

## Project Status

**Working prototype – Core workflow implemented and tested.**

Future improvements:
- Automatic notification to IT support staff
- Ticket assignment to support agents
- Ticket status updates
- Improved error handling and monitoring

## Workflow File

`AI_IT_Helpdesk_GitHub_Safe.json`

This file contains a sanitized version of the n8n workflow for portfolio demonstration. Credentials and Google Sheets configuration must be set up before use.

## Author

Sumon Boiddo

Electronic Engineering Student | IT Support & AI Automation Enthusiast
