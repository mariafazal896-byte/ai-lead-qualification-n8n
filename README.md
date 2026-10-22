# Multi-Source Lead Routing & Instant AI Qualification

## Overview
An AI-powered lead qualification workflow built using n8n. It receives lead information through a webhook, evaluates the lead using an AI Agent, stores the results in Airtable, and sends a notification to the sales team through Slack.

## Problem
Sales teams can spend significant time manually reviewing incoming leads, assessing their suitability, and preparing follow-up questions.

## Solution
This workflow automates lead evaluation and helps sales teams prioritize prospects using AI-generated qualification results.

## Workflow
Webhook → Edit Fields → AI Agent → Airtable → Slack

## Tools & Technologies
- n8n — workflow automation
- Webhook — receives incoming lead data
- AI Agent — evaluates lead information
- Structured Output Parser — structures AI results
- Airtable — stores lead records
- Slack — sends sales notifications

## Key Features
- Automated lead intake
- AI-generated lead score from 1–100
- High, Medium, or Low qualification
- Qualification reasoning
- Personalized sales talking points
- Airtable record creation
- Slack sales alerts

## How to Test
1. Import the workflow JSON into an n8n instance.
2. Configure the required AI model and credentials.
3. Configure Airtable and Slack credentials.
4. Send a test POST request to the webhook with sample lead data.
5. Verify the qualification output, Airtable record, and Slack notification.

## Security & Requirements
Credentials must be configured separately in n8n. Never publish API keys, access tokens, passwords, or confidential lead data in this repository.

A publicly reachable webhook and an appropriate hosting setup are required for production use.

## Project Status
Completed prototype; production deployment requires environment-specific configuration and testing.
