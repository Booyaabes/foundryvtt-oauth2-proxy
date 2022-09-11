# Foundry VTT stack

Foundry VTT stack with an Oauth2 proxy restricting access to it. Keycloak is used as identity provider.

## Installation

Create a `.env` file containing something similar to :

```shell
KEYCLOAK_DB_PASSWORD=XXXXXXXXXXXXXXXXXXXXX
KEYCLOAK_ADMIN_PASSWORD=XXXXXXXXXXXXXXXXXX
KEYCLOAK_ADDRESS=idp.my-domain.com
OAUTH2_PROXY_COOKIE_SEED=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
OAUTH2_PROXY_COOKIE_DOMAIN=fvtt.my-domain.com
OAUTH2_PROXY_WHITELIST_DOMAIN=fvtt.my-domain.com
OAUTH2_PROXY_CLIENT_ID=foundryvtt
OAUTH2_PROXY_CLIENT_SECRET=XXXXXXXXXXXXXXXXXXXXXXXXX
OAUTH2_PROXY_REDIRECT_URL=https://fvtt.my-domain.com/oauth2/callback
OAUTH2_PROXY_OIDC_ISSUER_URL=https://idp.my-domain.com/realms/foundryvtt
```

I included a great Foundry VTT Keycloak theme coming from [here](https://github.com/patrick246/keycloak-foundryvtt-theme).
