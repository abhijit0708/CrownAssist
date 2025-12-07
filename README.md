** Monday Email Summary – n8n Automation

This repository contains an n8n workflow that automatically collects weekend Gmail emails, summarizes the content using an AI model (OpenAI GPT-4o or Google Gemini), and sends a single concise summary email every Monday morning.

** Features

Automatic Monday morning trigger

Fetch weekend Gmail messages

Combine and clean raw email text

AI-powered email summarization using:

GPT-4o (OpenAI)

or Google Gemini (configurable in workflow)

Send summary email to your inbox



**File	Description
CrownAssist.json	Main n8n workflow export
README.md	Documentation
n8n_WORKFLOW.png  WORKFLOW 



**Requirements

To run this workflow, you need:

n8n instance (self-hosted or cloud)

Gmail API credentials

AI model API key (either one):

OpenAI API Key

Google Gemini API Key

**Setup Instructions
1. Import the workflow

Open n8n

Click "Import from file"

Select the .json file from this repo

2. Configure credentials

Gmail OAuth2 (for getAll and send operations)

AI Model key (OpenAI or Gemini) inside the "Analyze Emails" node

3. Customize your schedule

**You can modify the cron trigger to run at any interval, for example:

**Mondays at 9 AM

**Daily reminders

**Weekly summaries
