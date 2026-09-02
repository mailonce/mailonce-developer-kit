# Contributing

Thanks for helping improve the developer side of MailOnce.

## Good contributions

This repository is intentionally narrow. Useful contributions include:

- a small reproducible example for an email workflow
- a fix to an existing example
- clearer setup instructions
- a bug report with steps to reproduce
- a real developer or QA workflow that could inform a future API

Please avoid adding generic demo code that does not exercise an email workflow.

## Before opening a pull request

1. Keep the example small and understandable.
2. Do not commit credentials, inbox tokens, SMTP passwords, or private email content.
3. Add a `.env.example` when configuration is required.
4. Document exactly how to run the example.
5. Make sure the example works without access to MailOnce production internals.
6. Do not present planned API features as already available.

## Pull requests

Describe:

- the workflow being demonstrated or fixed
- how you tested it
- any external service required to run it

For larger additions, opening an issue first is helpful so we can agree on scope.
