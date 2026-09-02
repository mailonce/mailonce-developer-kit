# MailOnce Developer Kit

Practical examples for testing email-based product flows with [MailOnce](https://mailonce.org).

MailOnce gives you short-lived inboxes that are useful when you need to test signup emails, one-time passwords, verification links, passwordless login, and other flows without using a personal inbox.

This repository is developer-facing tooling and examples. It is **not** the source code for the MailOnce production service.

## Start here

The first executable example sends a real test email through **your own SMTP provider** to a MailOnce inbox.

```bash
cd examples/email-flow-smoke-test
npm install
cp .env.example .env
npm run send -- --to YOUR_MAILONCE_ADDRESS --type both
```

Create a temporary inbox at https://mailonce.org, copy its address, and use that address as `--to`.

The example can send:

- an OTP code
- a verification link
- both in one message

See [`examples/email-flow-smoke-test`](./examples/email-flow-smoke-test) for setup details.

## What this repo is for

We want the public developer side of MailOnce to be useful before there is a public API. The examples here focus on workflows that developers and QA teams can run today.

Useful cases include:

- signup and email-verification testing
- OTP delivery checks
- verification-link checks
- passwordless authentication emails
- isolated inboxes for QA
- basic email-delivery smoke tests

## Current MailOnce product

MailOnce currently focuses on the hosted inbox experience, including temporary addresses, real-time delivery, OTP detection, verification-link detection, multiple temporary-email domains, custom temporary addresses, inbox extension, and device linking.

Try it at https://mailonce.org.

## Developer roadmap

The following are planned or under consideration; they are **not presented as available APIs today**:

- Developer API
- API keys
- webhooks
- JavaScript / TypeScript SDK
- Python SDK
- automated email-flow testing
- multi-inbox developer workflows

The roadmap is tracked in [`docs/roadmap.md`](./docs/roadmap.md).

## Feedback wanted

If you use MailOnce in a real development or QA workflow, open an issue and tell us about the workflow itself:

- What are you testing?
- What is awkward or missing?
- Would an API remove manual steps?
- Which SDK would you actually use?
- Which webhook events would matter?

Concrete workflows are more useful than feature wishlists because they help us design the developer platform around real use.

## About the project

MailOnce is the first product I built and shipped as a developer. I started it because temporary-email tools often felt cluttered or awkward when I only needed a fast inbox for verification and testing.

I am improving it based on real usage. Feedback from developers is especially valuable because it can shape the API and tooling we build next.

If this repository or MailOnce is useful in your workflow, a star helps other developers discover it.

## Contributing

Small examples, bug reports, and reproducible developer workflows are welcome. Read [`CONTRIBUTING.md`](./CONTRIBUTING.md) before opening a pull request.

For security issues, follow [`SECURITY.md`](./SECURITY.md) instead of opening a public issue.

## License

MIT. See [`LICENSE`](./LICENSE).
