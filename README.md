Monday Email Summary – n8n Automation

This repository contains an n8n workflow that automatically collects weekend Gmail emails, summarizes the content using an AI model (OpenAI GPT-4o or Google Gemini), and sends a single concise summary email every Monday morning.

Features

Automatic Monday morning trigger

Fetch weekend Gmail messages

Combine and clean raw email text

AI-powered email summarization using:

GPT-4o (OpenAI)

or Google Gemini (configurable in workflow)

Send summary email to your inbox

Workflow Diagram (High-Level)

Monday Morning Trigger

Get Weekend Emails (Gmail)

Combine Email Data

Analyze Email Content with AI

Send Summary Email (Gmail)

All nodes and connections are stored in the *.json workflow file.

Files
File	Description
monday-email-summary.json	Main n8n workflow export
README.md	Documentation

If your file has a different name, update it above accordingly.

Requirements

To run this workflow, you need:

n8n instance (self-hosted or cloud)

Gmail API credentials

AI model API key (either one):

OpenAI API Key

Google Gemini API Key

Setup Instructions
1. Import the workflow

Open n8n

Click "Import from file"

Select the .json file from this repo

2. Configure credentials

Gmail OAuth2 (for getAll and send operations)

AI Model key (OpenAI or Gemini) inside the "Analyze Emails" node

3. Customize your schedule

You can modify the cron trigger to run at any interval, for example:

Mondays at 9 AM

Daily reminders

Weekly summaries
