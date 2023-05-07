---
sidebar_position: 1
---

# Create Users

When a new platform instance is created, the instance supports logging in with following default credentials. The default credentails could be changed by updating `SETUP_DEFAULT_PASSWORD` property in .env file.

```
username: foo@example.com
password: bar
```
At least one user must be created in the platform instance to disable the access for the default credentials.

:::danger
We recommend immediately creating a new user record upon setting up a platform instance.
:::

To create a new user:

1. Login to the Platform instance. If this the first user being created, login with default credentials.
2. Click **New User**
3. Provide Email Address, user details and setup a password for the user.
4. Click Submit to create the user.

## Roles

The platform currently does not have roles. 

Every user is an admin user. Take this into consideration when creating new user accounts in the Platform.

Roles will be introduced in the future releases.

## Change Password

Since we only support creating admin users, any user will be able to update the password for other users. In the event, a user has forgotten the password or has an account locked out, other users will be able to unlock or change the user's password.