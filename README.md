# homebrew-tap

Homebrew tap for projects by [Felix Stubner](https://github.com/fstubner).

## Usage

```bash
brew tap fstubner/tap
brew install <formula>
```

## Formulae

| Formula | Description |
|---------|-------------|
| [`netscli`](./Formula/netscli.rb) | Network scanner with CLI, TUI, desktop app, and MCP server. https://netscli.com |

## How it's maintained

Each formula installs a prebuilt binary from the project's GitHub
release and generates shell completions + man page by shelling out to
the just-installed binary (so completions never drift from the CLI
surface).

Version bumps land as single commits: edit `version` and the four
`sha256` values to match the new release's `.sha256` files, then
`brew install --build-from-source ./Formula/<name>.rb` to verify.

## License

MIT.
