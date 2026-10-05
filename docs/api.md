# Genory API overview

The authoritative API reference lives at:

https://genory.dev/docs

This repository only contains lightweight integration examples. If an example here differs from the live documentation, follow the live documentation.

## Authentication

Use your Genory API key as a Bearer token.

```http
Authorization: Bearer YOUR_API_KEY
```

Keep credentials outside source control.

## Example request

```bash
curl --request POST "https://genory.dev/api/profile" \
  --header "Authorization: Bearer $GENORY_API_KEY" \
  --header "Content-Type: application/json" \
  --data '{"country":"DE","amount":1,"fields":["firstName","lastName","email"]}'
```

## Recommended integration practices

- keep API keys in environment variables
- validate responses before using them in fixtures
- avoid using generated data as proof of real identities or accounts
- consult https://genory.dev/docs for current endpoints, limits and plan availability
