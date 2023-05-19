---
sidebar_position: 2
---

# Single Sign-On

Single Sign-On can optionally be enabled for signing into platform via your enterprise identity providers (IdP). Any IdP that supports OAuth + OpenID Connect (OIDC) can be configured as an SSO provider. Most modern identity providers support OIDC authentication mechanism.

## Enabling SSO

1. Login to your instance and navigate to **Settings** page.
2. Click **Single Sign On** tab.
3. Copy the **Redirect URI** from the page. This URL is required for defining SSO configuration with your identity provider.
4. Login to your identity provider and define the required OIDC configuration. Copy the Client ID, Client Secret, Well-Known URL from your IdP.
5. Navigate back to your cptn.io instance.
6. Provide the **Client ID**, **Client Secret** and the **Well-Known URL**.
7. Toggle **Active** to ON
8. Toggle **Auto Create User on Login** to ON for dynamically creating users in cptn.io on first login via SSO.
9. Toggle **Allow login only with SSO** to ON for restricting login only via SSO.

:::warning
Do not set **Allow login only with SSO** to ON until you have completed testing your SSO configuration. If this flag is set to true with incorrect SSO configuration, none of the users will be able to login to the platform. 
:::

## Testing SSO

Once the SSO configuration is defined in your cptn.io instance, logout from your current session.

The login page will now show **Sign In with SSO** button. Clicking this button will automatically navigate you to configured identity provider to login. 

On successful login, you will be redirected to your cptn.io instance and will be automatically logged in.

:::info
We do not support Single Logout for SSO. Logging out from cptn.io instance will not automatically log you out from your identity provider.
:::

## Details instructions for integrating with IdPs

- [Integrate with Okta](./sso_providers/Okta.md)
- [Integrate with Azure AD](./sso_providers/azuread.md)
- [Integrate with Google Workspace](./sso_providers/google_workspace.md)

If you need instructions for integrating with other IdPs, send an email to support@devraven.io.