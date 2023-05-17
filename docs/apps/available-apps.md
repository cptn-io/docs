---
sidebar_position: 3
---

# Available Apps

## Destinations

- **AWS - Write to S3 Bucket**
    Allows batch processing and writing batch of events to an AWS bucket
- **Snowflake - Write to Table**
    Sample implementation to write batch of events to a Snowflake table
- **Sendgrid - Send email using template**
    Send an email via Sendgrid using templates defined
- **Sendgrid - Send an email**
    Send an email via Sendgrid
- **Sendgrid - Add user to Contacts**
    Add user to Contacts in Sendgrid.
- **GCP - Write to bucket**
    Allows batch processing and writing batch of events to an GCP bucket
- **Teams - Send a message**
    Send message to Microsoft Teams using webhooks
- **Postgres - Write to table**
    Allows batch processing and writing batch of events to Postgres database table.
- **Twilio - Send Text Message**
    Send text message using Twilio
- **Stripe - Create Customer**
    Create a customer entity in Stripe
- **Slack - Send message to a Channel**
    Send a message to a Slack channel or user using webhooks


## Transformers

- **IP to Location**
    Use geoip-lite to resolve IP address to a physical location
- **Clear null props**
    Clears out any null properties from the ingested event
- **Sample 5% events**
    Allows ~5% of the events to pass through the pipeline.
- **Drop events from pipeline**
    Drop events from the pipeline
- **Redact SSN from event**
    Checks all properties in the event and redacts any SSN numbers using regex
