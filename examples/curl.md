# cURL example

Set your API key as an environment variable:

```bash
export GENORY_API_KEY="your_api_key"
```

Then call a supported endpoint:

```bash
curl --request POST "https://genory.dev/api/profile" \
  --header "Authorization: Bearer $GENORY_API_KEY" \
  --header "Content-Type: application/json" \
  --data '{"country":"DE","amount":1,"fields":["firstName","lastName","email"]}'
```

For the current API reference, see https://genory.dev/docs.
