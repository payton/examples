# Example: Web3 File Sharing Portal
## Instructions

1. Register With IdP: `curl -X POST https://oidc.login.xyz/register -H 'Content-Type: application/json' -d '{"redirect_uris": []}'`
2. ``
3. Update Redirect URI: `curl -X POST http://oidc.login.xyz/client/<CLIENT_ID> -H 'Content-Type: application/json' -H 'Authorization: Bearer <REGISTRATION_ACCESS_TOKEN>' -d '{"redirect_uris": ["<REDIRECT_URI>"]}'`
4. Verify Updated Redirect URI: `curl http://oidc.login.xyz/client/<CLIENT_ID> -H 'Authorization: Bearer <REGISTRATION_ACCESS_TOKEN>'`