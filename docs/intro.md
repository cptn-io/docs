---
sidebar_position: 1
---

# Introduction

cptn.io is an integration and data platform that helps setup integrations between services quickly and easily. Data from Source systems can be sent via simple HTTP calls to be processed in one or multiple pipelines. Each pipeline can be composed of javascript based Transformations to mutate or enrich the data and then be sent to Destination services.


## Getting Started

To setup the platform on your local machine:

Prerequisites:
- Docker installed and running.

1. Run `git clone https://github.com/cptn-io/el-cptn.git`
2. Update the property values in .env file. Ensure that secrets, crypto keys, passwords you use are complex, random and secure.
3. Run `docker compose up` to start the platform.
4. Required docker images will be downloaded and the server will start up in few mins.
5. Access the service at http://localhost/

:::info
APP_URL value in .env defines the default port for running the service. If port 80 is not available, change the value to a different value in .env file.
:::

### Setting up on DigitalOcean

1. Login to your DigitalOcean account.
2. Create a new droplet and login to the server.
3. Install docker on the server.
4. Run `git clone https://github.com/cptn-io/el-cptn.git`
5. Update the property values in .env file.
6. Run `docker compose up -d` to start the platform.
7. The server should be accessible at `http://<your droplet ip>`

#### To setup a custom domain for accessing your service.
8. Login to your DNS configuration and create a new A record for a domain e.g. `cptn.example.com` to map to your droplet's IP address.
9. Update .env file in your droplet. Change `APP_URL` property value to your domain `cptn.example.com`
10. Run `docker compose restart`
12. If the service is accessible, SSL certificates would automatically be provisioned for the domain and the service will be accessible via the domain url at `https://cptn.example.com`

### Login
Login to your Service using the following default credentials. Update the .env file to change the default setup password.

```
Username: foo@example.com
Password: bar
```

Navigate to Users page and create a new user in your instance.

:::danger
The default credentials will only work during the initial setup until at least one user record is created. The service will no longer be accessible via the default credentials once a user record is created.

We strongly recommend immediately creating a new user as soon as a platform instance is setup.
:::