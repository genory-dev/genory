# Genory

**Free online generators, synthetic test data, validators and developer tools.**

Genory helps developers, QA engineers and technical teams generate practical test data, inspect formats and create repeatable fixtures without using real customer data.

- Website: https://genory.dev
- Tools: https://genory.dev/tools
- API documentation: https://genory.dev/docs
- Blog: https://genory.dev/blog

## What is Genory?

Genory currently provides 25 online tools for generation, validation, developer workflows, text utilities and synthetic test data.

Popular tools include:

- UUID v4 and v7 generation
- Synthetic profile generation
- Custom test-data datasets
- Address and phone test data
- Synthetic IBAN generation and IBAN validation
- Card-format and BIN test data
- Password generation
- MAC and IMEI test data
- Random-data utilities
- Emoji and text tools

Generated data is intended for development, QA, demos and testing. It does not prove that an identity, bank account, phone number or other real-world entity exists.

## API

Developer-plan users can access supported Genory generators through the API using Bearer authentication.

Example:

```bash
curl --request POST "https://genory.dev/api/profile" \
  --header "Authorization: Bearer $GENORY_API_KEY" \
  --header "Content-Type: application/json" \
  --data '{"country":"DE","amount":1,"fields":["firstName","lastName","email"]}'
```

See the complete and current API documentation at:

https://genory.dev/docs

## Documentation and examples

- [Getting started](docs/getting-started.md)
- [API overview](docs/api.md)
- [Test-data guidance](docs/test-data.md)
- [cURL example](examples/curl.md)
- [JavaScript example](examples/javascript.md)
- [Python example](examples/python.md)

## About this repository

This is the public documentation and examples repository for Genory.

The production application source code, infrastructure configuration, credentials and private implementation details are **not published here**.

For the product itself, visit https://genory.dev.
