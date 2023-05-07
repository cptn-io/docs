---
sidebar_position: 3
---

# Rotating Keys

Secured Source will have primary and secondary keys automatically generated. At least one key is required for sending data into the platform for the Source.

We strongly recommend only using the primary key for invoking the HTTP end point for sending the data into the platform.

To rotate the keys:
1. Login to the platform.
2. Navigate to Sources in the left navigation menu.
3. Click the Source from the list.
4. Click **Rotate keys** button to rotate the keys.
5. The current primary key will be changed to secondary key.
6. A new primary key will be generated.
7. Your data source currently sending data will continue to work using the older primary key.
8. Update your data source to use the newly generated primary key.

:::info
In the event you want to change both the keys, perform **Rotate keys** operation twice. This will change both the primary and secondary keys. Any data sources that use the older keys must be updated to use the newly generated keys for sending events into the platform.
:::