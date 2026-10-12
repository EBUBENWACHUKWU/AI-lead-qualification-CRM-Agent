# AI Lead Qualification & CRM Agent

An AI-powered lead qualification and follow-up automation built with **n8n, OpenRouter, Webhooks, Google Sheets, and Gmail**.

## Project Overview

This project automates the initial qualification of sales leads. It receives lead information through a webhook, uses an AI model to assess the lead, calculates a lead score, assigns a lead temperature, and stores the results in Google Sheets.

The workflow routes Hot, Warm, and Cold leads differently to help prioritize sales follow-up.

## Business Problem

Manually reviewing incoming leads, prioritizing prospects, updating spreadsheets, and sending follow-up emails can be repetitive and time-consuming.

This project demonstrates how AI and workflow automation can streamline those tasks.

## Workflow

1. Receive lead details through a webhook.
2. Process lead information using an AI Agent connected to OpenRouter.
3. Generate a lead score, temperature, qualification reason, recommended action, and follow-up priority.
4. Store lead information and qualification results in Google Sheets.
5. Send a Gmail alert for Hot leads.
6. Send a follow-up email for Warm leads.
7. Store Cold leads without sending immediate sales emails.

## Technologies Used

- **n8n:** Workflow orchestration and automation
- **OpenRouter:** AI model integration
- **Webhooks:** Incoming lead data
- **Google Sheets:** Lead records and qualification results
- **Gmail:** Automated email notifications and follow-ups

## Testing

The workflow was tested using sample lead data:

| Sample Lead | Temperature | Score | Expected Action |
|---|---|---:|---|
| Sarah Johnson | Hot | 90 | Save to Sheets and send Hot Lead Alert |
| David Miller | Warm | 75 | Save to Sheets and send follow-up email |
| Emily Carter | Cold | 40 | Save to Sheets without immediate email |

All three lead categories were tested successfully in the development workflow.

## Skills Demonstrated

- AI automation and workflow design
- Webhook integrations
- Prompt-based lead qualification
- Conditional routing
- Google Sheets integration
- Gmail automation
- Workflow testing and troubleshooting

## Future Improvements

- Duplicate lead detection
- More robust error handling and notification testing
- Lead nurturing sequences
- A dashboard for lead analytics
- Secure deployment for external webhook access

## Project Status

Working prototype tested locally using n8n. Public deployment and production use are not yet claimed.

## Workflow Architecture

The diagram below shows the n8n workflow for AI-powered lead qualification, conditional routing, Google Sheets record keeping, and automated Gmail notifications.

![AI Lead Qualification CRM Workflow](workflow-architecture.png)
