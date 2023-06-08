---
sidebar_position: 3
---

# Available Apps

## Destinations

- **AWS - Write to S3 Bucket**
    Allows batch processing and writing batch of events to an AWS bucket
- **GCP - Write to bucket**
    Allows batch processing and writing batch of events to an GCP bucket
- **MongoDB - Write to collection**
    Allows writing events to MongoDB
- **MySQL - Write to table**
    Write data to configured any MySQL table
- **Postgres - Write to table**
    Allows batch processing and writing batch of events to Postgres database table.
- **Sendgrid - Send an email**
    Send an email via Sendgrid
- **Sendgrid - Send email using template**
    Send an email via Sendgrid using templates defined
- **Sendgrid - Add user to Contacts**
    Add user to Contacts in Sendgrid.
- **ServiceNow - Add work notes to Incident**
    Adds provided text as work notes to an incident
- **ServiceNow - Create an Incident**
    Creates an incident in ServiceNow
- **Slack - Send message to a Channel**
    Send a message to a Slack channel or user using webhooks
- **Snowflake - Write to Table**
    Sample implementation to write batch of events to a Snowflake table
- **Stripe - Create Customer**
    Create a customer entity in Stripe
- **Teams - Send a message**
    Send message to Microsoft Teams using webhooks
- **Twilio - Send Text Message**
    Send text message using Twilio
- **Twilio - Send Whatsapp message**
    Send Whatsapp message using Twilio
- **Webhooks - Send event to URL**
    Setup any URL as a web hook to receive events from Pipelines


## Transformers
- **Clear null props**
    Clears out any null properties from the ingested event
- **Drop events from pipeline**
    Drop events from the pipeline
- **IP to Location**
    Use geoip-lite to resolve IP address to a physical location
- **OpenAI - Extract keywords**
    Extract keywords from provided text
- **OpenAI - TL;DR Summary**
    Create TL;DR summary for provided text    
- **OpenAI - Analyze Incident**
    Analyze provided text/logs and explain in simple terms
- **Redact SSN from event**
    Checks all properties in the event and redacts any SSN numbers using regex
- **Sample 5% events**
    Allows ~5% of the events to pass through the pipeline.


