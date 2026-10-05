# Synthetic test-data guidance

Synthetic data is useful when developers and QA teams need realistic-looking fixtures without copying real customer records into development environments.

## Good uses

- local development
- QA and staging environments
- UI demos
- automated tests
- seed data
- API prototyping

## Avoid common mistakes

Generated values may match real-world formats without representing real entities.

A syntactically valid IBAN, phone number, address, identifier or profile should not be interpreted as verified, assigned or usable in the real world.

For current Genory generators, visit:

https://genory.dev/tools
