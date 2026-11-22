# Trimlet Tools

The small things you would otherwise search the web for, in a small window driven only by the keyboard.

- **Security:** random strings and passwords, hashes, SSH key pair (Ed25519, saved in `~/.ssh`), decode a JWT.
- **Network:** my IP address, ping, check a website, DNS lookup, IP info, port check.
- **JSON/XML:** validate, view with colors, structure and skeleton of a document, JSON examples from
  an OpenAPI spec, XML example from an XSD schema.

It saves nothing of its own. "My IP address" asks api.ipify.org, "IP info" ipinfo.io and rdap.org;
nothing else leaves your computer unless you ask for it (a ping, a website check, a DNS lookup).

## Build

Written in Go with [Fyne](https://fyne.io), for macOS and Windows. Ready-made downloads are not
published yet. To build it, with Go installed (and on a Mac the Xcode command line tools):

```
go run fyne.io/tools/cmd/fyne@v1.7.3 package --release
```

or `go run .` to try it. The console window comes from [trimlet/gui](https://github.com/trimlet/gui),
which `go` fetches by itself.

## How it is made

The code is written with Claude Opus (Anthropic), under the direction and review of a developer with
almost 30 years of experience. Every feature starts from a real, repeated need, and most ideas are
turned down: the goal is to stay small.

## License

GPL-3.0, see [LICENSE](LICENSE).
