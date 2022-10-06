# 💊 nginx-plus-oidc-troubleshooting

NGINX Plus OIDC troubleshooting for Identity Providers.

> **Note:**
>
> Please update any questions and answers whenenver anyone get customers' issues or questions.

- [Common Troubleshooting for NGINX OIDC and All IdPs](#common-troubleshooting-for-nginx-plus-oidc-and-all-idps)
- [Troubleshooting for NGINX OIDC and Amazon Cognito](#troubleshooting-for-nginx-plus-oidc-and-amazon-cognito)
- [Troubleshooting for NGINX OIDC and Auth0](#troubleshooting-for-nginx-plus-oidc-and-auth0)
- [Troubleshooting for NGINX OIDC and Azure AD](#troubleshooting-for-nginx-plus-oidc-and-azure-ad)
- [Troubleshooting for NGINX OIDC and Keycloak](#troubleshooting-for-nginx-plus-oidc-and-keycloak)
- [Troubleshooting for NGINX OIDC and Kubernetes](#troubleshooting-for-nginx-plus-oidc-and-kubernetes)
- [Troubleshooting for NGINX OIDC and Okta](#troubleshooting-for-nginx-plus-oidc-and-okta)
- [Troubleshooting for NGINX OIDC and OneLogin](#troubleshooting-for-nginx-plus-oidc-and-onelogin)
- [Troubleshooting for NGINX OIDC and Ping Identity](#troubleshooting-for-nginx-plus-oidc-and-ping-identity)

## 🔧 Troubleshooting

### Common Troubleshooting for NGINX OIDC and All IdPs

Any errors generated by the OpenID Connect flow are logged to the error log, `/var/log/nginx/error.log`. Check the contents of this file as it may include error responses received by the IdP. The level of detail recorded can be modified by adjusting the severity level of the `error_log` directive.

- 400 error from IdP
- 500 error from nginx after successful authentication
- Authentication is successful but browser shows too many redirects
- Logged out but next request does not require authentication
- Failed SSL/TLS handshake to IdP

### Troubleshooting for NGINX Plus OIDC and Amazon Cognito

- [How to ensure that Amazon Cognito correctly set up before configuring your app or NGINX Dev Portal?](./amazon-cognito/001-ensure-cognito-setup-before-your-app.md)
- How to troubleshoot when PKCE is not working with Amazon Cognito?
- How to troubleshoot when none-PKCE is not working with Amazon Cognito?
- How to troubleshoot when logout is not working with Amazon Cognito?
- How to troubleshoot when dns server is not responding?
- How to troubleshoot when logout is not working with Amazon Cognito?
- [How to troubleshoot when `prefered_username` is not shown in Dev Portal UI?](./amazon-cognito/006-prefered-username-not-shown.md)
- How to troubleshoot when a frontend OIDC simulation tool is not working with `X-Client-Id should be in cookie`. when signing-in after signed-out?
- How to troubleshoot when `_codexch` returns `error_description=invalid_scope`?

### Troubleshooting for NGINX Plus OIDC and Auth0

- [How to ensure that Auth0 correctly set up before configuring your app or NGINX Dev Portal?](./auth0/001-ensure-auth0-setup-before-your-app.md)
- How to troubleshoot when PKCE is not working with Auth0?
- How to troubleshoot when none-PKCE is not working with Auth0?
- How to troubleshoot when logout is not working with Auth0?
- How to troubleshoot when dns server is not responding?
- How to troubleshoot when a frontend OIDC simulation tool is not working with `X-Client-Id should be in cookie`. when signing-in after signed-out?

### Troubleshooting for NGINX Plus OIDC and Azure AD

- [How to ensure that Azure AD correctly set up before configuring your app or NGINX Dev Portal?](./azure-ad/001-ensure-azure-ad-setup-before-your-app.md)
- How to troubleshoot when PKCE is not working with Azure AD?
- How to troubleshoot when none-PKCE is not working with Azure AD?
- How to troubleshoot when logout is not working with Azure AD?
- How to troubleshoot when dns server is not responding?
- How to troubleshoot when a frontend OIDC simulation tool is not working with `X-Client-Id should be in cookie`. when signing-in after signed-out?
- [How to troubleshoot for the Azure AD's error response with `AADSTS9002327` (Tokens issued for the 'Single-Page Application' client-type may only be redeemed via cross-origin requests)?](./azure-ad/007-token-endpoint-single-page-app-cross-origin.md)

### Troubleshooting for NGINX Plus OIDC and Keycloak

- [How to ensure that Keycloak correctly set up before configuring your app or NGINX Dev Portal?](./keycloak/001-ensure-keycloak-ad-setup-before-your-app.md)
- How to troubleshoot when PKCE is not working with Keycloak?
- How to troubleshoot when none-PKCE is not working with Keycloak?
- How to troubleshoot when logout is not working with Keycloak?
- How to troubleshoot when dns server is not responding?
- How to troubleshoot when a frontend OIDC simulation tool is not working with `X-Client-Id should be in cookie`. when signing-in after signed-out?

### Troubleshooting for NGINX Plus OIDC and Kubernetes

### Troubleshooting for NGINX Plus OIDC and Okta

- [How to ensure that Okta correctly set up before configuring your app or NGINX Dev Portal?](./okta/001-ensure-okta-ad-setup-before-your-app.md)
- How to troubleshoot when PKCE is not working with Okta?
- How to troubleshoot when none-PKCE is not working with Okta?
- How to troubleshoot when logout is not working with Okta?
- How to troubleshoot when dns server is not responding?
- How to troubleshoot when a frontend OIDC simulation tool is not working with `X-Client-Id should be in cookie`. when signing-in after signed-out?

### Troubleshooting for NGINX Plus OIDC and OneLogin

- [How to ensure that OneLogin correctly set up before configuring your app or NGINX Dev Portal?](./onelogin/001-ensure-onelogin-ad-setup-before-your-app.md)
- How to troubleshoot when PKCE is not working with OneLogin?
- How to troubleshoot when none-PKCE is not working with OneLogin?
- How to troubleshoot when logout is not working with OneLogin?
- How to troubleshoot when dns server is not responding?
- How to troubleshoot when a frontend OIDC simulation tool is not working with `X-Client-Id should be in cookie`. when signing-in after signed-out?

### Troubleshooting for NGINX Plus OIDC and Ping Identity

## 📚 References

- [NGINX Plus OIDC v1 Troubleshooting](https://github.com/nginxinc/nginx-openid-connect#troubleshooting)
- [NGINX Plus OIDC for Amazon Cognito](https://github.com/nginx-openid-connect/nginx-oidc-amazon-cognito)
- [NGINX Plus OIDC for Auth0](https://github.com/nginx-openid-connect/nginx-oidc-auth0)
- [NGINX Plus OIDC for Azure AD](https://github.com/nginx-openid-connect/nginx-oidc-azure-ad)
- [NGINX Plus OIDC for Keycloak](https://github.com/nginx-openid-connect/nginx-oidc-keycloak)
- [NGINX Plus OIDC for Kubernetes](https://github.com/nginx-openid-connect/nginx-oidc-kubernetes)
- [NGINX Plus OIDC for Okta](https://github.com/nginx-openid-connect/nginx-oidc-okta)
- [NGINX Plus OIDC for OneLogin](https://github.com/nginx-openid-connect/nginx-oidc-onelogin)
- [NGINX Plus OIDC for Ping Identity](https://github.com/nginx-openid-connect/nginx-oidc-ping-identity)
