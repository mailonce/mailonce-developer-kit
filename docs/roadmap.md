# Developer roadmap

This file describes ideas we are exploring for MailOnce developers. It is not a promise that every item will ship, and it should not be read as API documentation for features that already exist.

## Near-term focus

- collect real developer and QA workflows
- publish small executable testing examples
- learn which manual steps are repeated most often
- identify the minimum useful public API surface

## Under consideration

### Developer API

Potential use cases include creating or managing test inboxes programmatically and reading delivery state during automated tests.

### API keys

A future developer plan would need scoped credentials, revocation, quotas, and clear separation from normal browser-session credentials.

### Webhooks

Possible events could include message receipt and extracted verification data. Event shape, security, retries, and idempotency still need design work.

### SDKs

JavaScript / TypeScript and Python are the first SDK candidates because they cover a large share of web and test-automation workflows.

### Automated email-flow testing

We are interested in workflows such as:

- create an isolated inbox
- trigger an application email
- wait for delivery
- inspect the message
- assert an OTP or verification link
- clean up automatically

## Help shape this

Open a GitHub issue with a real workflow you want to automate. Include the language or test framework you use and which steps you currently perform manually.
