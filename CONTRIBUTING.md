# Contributing to FireMQ

Thanks for helping. This guide applies to every repository in the FireMQ organization.

## Report a bug or ask for a feature

Open an issue in the repository it concerns. For a bug, include the FireMQ version (`firemq --version`), the client library and version, what you did, what you expected, and what happened. Broker logs help; run with `--log debug` to get more.

Report security problems privately instead; see [SECURITY.md](SECURITY.md).

## Send a change

1. For anything larger than a small fix, open an issue first so we can agree on the approach.
2. Fork the repository and create a branch.
3. Make the change with tests. Each repository's README explains how to build and test it.
4. Open a pull request that says what changed and why, and links the issue.

CI must pass before a pull request is merged. SDK repositories run the shared [conformance suite](https://github.com/FireMQ/firemq/blob/main/spec/conformance.md) against a real broker, so a change in behavior shows up there.

## Protocol changes

The FireMQ protocol is specified in [`spec/fire-protocol.md`](https://github.com/FireMQ/firemq/blob/main/spec/fire-protocol.md), with test vectors every SDK checks. A change to the protocol starts as an issue in the main repository and lands there first, with updated vectors, before SDKs follow.

## License

By contributing, you agree that your contributions are licensed under the Apache License 2.0.
