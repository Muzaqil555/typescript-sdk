---
'@modelcontextprotocol/client': minor
---

Add an optional `issuerValidator` predicate to `discoverAuthorizationServerMetadata()`, `discoverOAuthServerInfo()`, and `AuthOptions`, along with a `createEntraIssuerValidator()` helper for multi-tenant Microsoft Entra ID endpoints (`/organizations/v2.0`, `/common/v2.0`) that return the literal `{tenantid}` template in OIDC discovery metadata (`https://login.microsoftonline.com/{tenantid}/v2.0`). Default RFC 8414 §3.3 exact-match validation is unchanged.
