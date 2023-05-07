---
sidebar_position: 1
---

# Platform Settings

The platform ships with default settings that can be updated if required.

### Event Data Retention Interval

Inbound and Outbound event data is purged at regular intervals from the database. The default data retention interval is **3 days**. 

This interval can be changed as below:
1. Login to the docker container running PostgreSQL database.
```
docker exec -it <container-id> /bin/sh
```
2. Execute the following command to login to the database.
```
psql -h localhost -U postgres -d elcptn
```
3. Once logged in, execute the following query to change the interval. `86400000` in the query below represents 24 hour interval in milliseconds. Change this value as per your needs.
```
INSERT INTO settings (key, value, system_managed) VALUES ('data.storage.interval', '86400000', false)
```
4. Logout from the container.

### Event Processing Batch Size

Event processor reads queued outbound events in batches for processing. The default batch size for querying the events is **100**.

The default batch size can be changed by setting an environment variable in the Processor service.

Update docker-compose.yml to set QUERY_BATCH_SIZE environment variable with the required batch size value and restart the processor service.