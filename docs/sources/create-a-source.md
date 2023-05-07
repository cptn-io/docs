---
sidebar_position: 1
---

# Create a Source

A Source is the point of entry for data into the platform for processing and delivery to a Destination. Every Source created will have a unique HTTP data ingestion end point for sending the data from services.

To create a new Source:

1. Login to your instance of the platform
2. Click **Sources** in the left navigation.
3. Click **New Source**.
![Create Source](/img/create-source.png)
4. Provide a name for the Source.
5. Optionally, define Response Headers for the end point. These headers will be returned when the ingestion end point is called for sending the events.
6. Set **Secured** property to ON for protecting the end point with a security token.
7. Click Submit.
8. A new source will be created.