---
sidebar_position: 2
---

# Sending Data for processing

Sources allow ingesting data into the platform for processing via a uniquely generated URL for each source. Data in JSON payload can be POSTed to these end points.

![Source Details](/img/source-details.png)

To send data into the platform:
1. Login to the platform.
2. Navigate to Sources in the left navigation menu.
3. Click the Source from the list.
4. The Source details page shows the required details for sending the data.
5. Copy the **Event URL**
6. If the Source is secured, primary and secondary keys are automatically generated. At least one key is required for successfully invoking the Event URL for sending the data.
:::caution
We strongly recommend using only the primary key for sending the data. Secondary keys serve unique purpose when rotating the keys. Using secondary key for sending data can can failures when keys are rotated.
:::
7. Use the following details for sending the data.

```
Method: POST
URL: <Event URL>
Headers:
  Content-Type: application/json
  Authorization: <primary key> (required, if the Source is secured)
Body:
  Event Payload in JSON format
```
8. The received event data will be sent to all configured pipelines for the Source.

:::note
We also accept sending security key as a query param named `token` if Authorization header cannot be passed for invoking the HTTP call. e.g. `https://<event url>?token=<key>`
:::

## Data retention

The default data retention interval for inbound and outbound events in the Platform is **3 days**. Ensure that events in the pipelines are processed within this default interval to avoid any data loss.

You can update the default retention interval if required. Refer Settings for more details.