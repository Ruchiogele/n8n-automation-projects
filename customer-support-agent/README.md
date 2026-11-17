# Customer Support AI Agent

An AI-powered customer support automation workflow built with **n8n**, designed to streamline customer enquiries, retrieve relevant account information, provide contextual responses, and support escalation to human agents.

## Project Overview

This project demonstrates how AI and workflow automation can improve customer support operations by connecting communication channels, business data sources, and knowledge management systems.

The workflow uses WhatsApp as its customer-facing communication channel. Incoming messages are processed by an AI agent that can access customer records, retrieve order and payment information, search a knowledge base, and initiate support escalation when required.

The organisation represented in this portfolio project is anonymised as **ABC Limited** to protect client confidentiality.

## Business Problem

Customer support teams often handle repetitive enquiries relating to:

- Order status and tracking
- Payment confirmation
- Customer account information
- Frequently asked questions
- Issues requiring further investigation or escalation

Handling these enquiries manually can increase response times and create additional operational workload.

This workflow demonstrates an automated approach to handling supported enquiries while maintaining access to relevant business information.

## Workflow Architecture

**Core workflow sequence:**

1. **Message Reception:** WhatsApp Trigger receives incoming customer messages.
2. **AI Processing:** An AI Agent interprets the enquiry and determines the appropriate response or information required.
3. **Customer Data Retrieval:** Airtable tools provide access to customer, order, and payment records.
4. **Knowledge Retrieval:** Pinecone provides access to relevant information from the configured knowledge base.
5. **Support Logging:** Google Sheets records support interactions.
6. **Escalation:** Gmail is used to initiate email-based support escalation.
7. **Customer Response:** The workflow sends the generated response through WhatsApp.

## Technology Stack

| Technology | Purpose |
|---|---|
| n8n | Workflow orchestration and automation |
| OpenAI GPT-4.1 mini | AI-powered enquiry processing |
| WhatsApp | Customer communication |
| Airtable | Customer, order and payment data retrieval |
| Pinecone | Knowledge base retrieval |
| Google Sheets | Support interaction logging |
| Gmail | Support escalation |

## Key Capabilities

- Automated WhatsApp enquiry handling
- AI-assisted customer response generation
- Customer record lookup
- Order and payment information retrieval
- Knowledge-base-assisted responses
- Support interaction logging
- Email-based escalation

## Setup Requirements

To configure this workflow in your own environment, you will need:

- An n8n instance
- An OpenAI API connection
- WhatsApp Business Platform credentials
- Airtable account and configured base/tables
- Pinecone account and configured index
- Google Sheets access
- Gmail account or supported email connection

The exported workflow uses placeholders for account-specific identifiers and does not include the original credential configurations.

## Configuration

Before executing the workflow:

1. Import the JSON workflow into n8n.
2. Configure the required credentials for each integration.
3. Replace the placeholder identifiers with your own account-specific values.
4. Configure the Airtable base and tables.
5. Connect the appropriate Pinecone index and namespace.
6. Configure the Google Sheets document and support email recipient.
7. Verify the WhatsApp trigger and outgoing message configuration.
8. Test each integration before enabling the workflow.

## Security and Privacy

This portfolio version uses an anonymised organisation name and sanitised configuration values.

- Client identity and business-specific information are anonymised.
- Credential configurations have been removed.
- Account-specific identifiers have been replaced with placeholders.
- Users must configure their own credentials before execution.

Never commit API keys, access tokens, passwords, private customer records, or production credentials to a public repository.

## Project Scope and Limitations

This repository contains an exported workflow configuration for demonstration and technical portfolio purposes.

The workflow's behaviour depends on the external services, credentials, data structures, prompts, and configurations supplied during deployment.

The published export should therefore be treated as a configurable project template, not a ready-to-run production deployment.

## Author's Focus

This project demonstrates practical experience with:

- AI agent workflow design
- Business process automation
- API and third-party service integration
- Retrieval-augmented information access
- Customer support automation
- Workflow orchestration using n8n

---

**Project:** Customer Support AI Agent  
**Platform:** n8n  
**Organisation:** ABC Limited (Anonymised)
