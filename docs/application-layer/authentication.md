# Authentication
Cosmocloud comes with **built-in** authentication module that is a Production Grade authentication system. We let you integrate with any 3rd Party SSO / Auth Provider such as AWS Cognito, Auth0, Google Identity, Okta, etc, anything that works on **OAuth** and **JWT Tokens**.

## Setup Authentication


- Just browse to **Application Layer --> Configs**, and just enable Authentication Config.
- Once enabled, you need to add two configuration properties.
    - **JWKI URI** - This is the public URL your Authentication Provider gives you, where the public keys can be found. Docs for some of the Auth Providers are below -
        - [AWS Cognito JWKS URI](https://docs.aws.amazon.com/cognito/latest/developerguide/amazon-cognito-user-pools-using-tokens-verifying-a-jwt.html#amazon-cognito-user-pools-using-tokens-aws-jwt-verify)
        - [Auth0 JWKS URI](https://auth0.com/docs/secure/tokens/json-web-tokens/json-web-key-sets)
        - [Firebase Authentication](https://cloud.google.com/api-gateway/docs/authenticating-users-firebase#configuring_apig_to_support_client_authentication) (Check point 1)
        - [Okta JWKS Keys Endpoint](https://developer.okta.com/docs/reference/api/oidc/#keys)
        - etc...
    - **Audience (optional)** - This is the identifier created by you in the authentication provider, to identify your Backend service.

![Setup Authentication](/assets/authentication/authentication.png)
​​

## ​​FAQs
1. The above list of Authentication Providers is not an exhaustive list. You can use any Provider till the time they expose the public JWK keys on a public URL.
2. Can I use my own self-hosted Authentication Provider (like Django)? Yes! You can use any self managed user management way, provided you expose the Public Keys of your service via a Public Endpoint.
3. If you are facing any issue while connecting your Authentication Provider, you can reach out to our team via contact@cosmocloud.io.