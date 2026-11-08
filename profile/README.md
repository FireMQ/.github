# FireMQ

A lean, fast message broker written in Rust that speaks RabbitMQ's AMQP 0-9-1, so your existing RabbitMQ clients connect unchanged.

```bash
curl -fsSL https://raw.githubusercontent.com/FireMQ/firemq/main/install.sh | sh
firemq
```

```bash
docker run -p 5672:5672 -p 5673:5673 -p 15672:15672 ghcr.io/firemq/firemq
```

FireMQ also has its own small protocol, built on MessagePack over TCP and WebSocket, with SDKs that share one API across languages. Every SDK runs the same conformance suite against the broker in CI.

| Repository | What it is |
|---|---|
| [firemq](https://github.com/FireMQ/firemq) | The broker, the `firemq` CLI, the Rust SDK, the protocol spec and the docs |
| [firemq-go](https://github.com/FireMQ/firemq-go) | Go SDK |
| [firemq-js](https://github.com/FireMQ/firemq-js) | TypeScript SDK for Node.js and browsers |
| [firemq-java](https://github.com/FireMQ/firemq-java) | Java SDK with Kotlin coroutine extensions |
| [firemq-dotnet](https://github.com/FireMQ/firemq-dotnet) | .NET SDK |
| [firemq-elixir](https://github.com/FireMQ/firemq-elixir) | Elixir client |
| [firemq-php](https://github.com/FireMQ/firemq-php) | PHP client |
| [setup-firemq](https://github.com/FireMQ/setup-firemq) | GitHub Action that starts a broker for CI |
| [homebrew-tap](https://github.com/FireMQ/homebrew-tap) | `brew install firemq/tap/firemq` |

Python, Ruby, Swift, Kotlin Multiplatform, Dart and C bindings over the Rust SDK live in the main repository.

[Documentation](https://firemq.github.io/firemq/) · [Roadmap](https://github.com/FireMQ/firemq/issues/23) · Apache-2.0
