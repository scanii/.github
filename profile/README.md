# Scanii

**Content security in a single API call.** Detect malware, unsafe images, and unsafe language in files, across six AWS regions worldwide.

[scanii.com](https://scanii.com) · [Documentation & support](https://docs.scanii.com) · [API reference](https://scanii.github.io/openapi/v22/) · [Status](https://status.scanii.com) · [Trust center](https://trust.scanii.com)

## Quick start

```bash
curl -u "$SCANII_KEY:$SCANII_SECRET" \
  -F "file=@./suspicious.pdf" \
  https://api.scanii.com/v2.2/files
```

Or use one of the official SDKs.

## Official SDKs

| SDK | Language | Install |
|---|---|---|
| [scanii-java](https://github.com/scanii/scanii-java) | Java | `com.scanii:scanii-java` (Maven Central) |
| [scanii-dotnet](https://github.com/scanii/scanii-dotnet) | C# / .NET | `dotnet add package Scanii` |
| [scanii-go](https://github.com/scanii/scanii-go) | Go | `go get github.com/scanii/scanii-go` |
| [scanii-node](https://github.com/scanii/scanii-node) | TypeScript / Node | `npm install @scanii/core` |
| [scanii-php](https://github.com/scanii/scanii-php) | PHP | `composer require scanii/scanii-php` |
| [scanii-rust](https://github.com/scanii/scanii-rust) | Rust | `cargo add scanii` |
| [scanii-ruby](https://github.com/scanii/scanii-ruby) | Ruby | `gem install scanii-ruby` |
| [scanii-python](https://github.com/scanii/scanii-python) | Python | `pip install scanii-python` |

## Develop and test without consuming credits

[**scanii-cli**](https://github.com/scanii/scanii-cli) is a local mock server that mirrors the Scanii API — including malware, unsafe image, and unsafe language detection responses — without making real API calls or consuming credits. Use it for local development and integration tests.

For GitHub Actions, [**setup-cli-action**](https://github.com/scanii/setup-cli-action) installs scanii-cli and starts the mock server on Linux, macOS, and Windows runners in a single step. Every official SDK uses it in CI.

## SDK principles

Every official SDK is built to the same three principles:

1. **Light.** Zero runtime dependencies, stdlib only.
2. **Up to date.** Always current with the latest Scanii API.
3. **Integration-only.** Wraps the REST API — retries, concurrency, and batching are the caller's responsibility.

## Resources

- [API versioning policy](https://docs.scanii.com/article/170-api-versioning-policy) — what to expect from our deprecation cadence.
- [Language clients overview](https://docs.scanii.com/article/146-language-clients).
- [Trust center](https://trust.scanii.com) — security and compliance documentation.

---

Apache-2.0 licensed. © Uva Software, LLC.
