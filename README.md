# nyldn Plugins

Shared Claude Code and Codex marketplace for nyldn plugins.

## Install

Add the marketplace once:

```bash
claude plugin marketplace add https://github.com/nyldn/plugins.git
```

For Codex:

```bash
codex plugin marketplace add https://github.com/nyldn/plugins.git
```

Then install the plugins you want:

```bash
claude plugin install octo@nyldn-plugins
claude plugin install img@nyldn-plugins
```

Restart Claude Code after installing or updating plugins.
Restart Codex, open `/plugins`, then install or enable the plugins you want.

## Plugins

| Plugin | Install | Description |
|---|---|---|
| Octopus | `claude plugin install octo@nyldn-plugins` or Codex `/plugins` as `claude-octopus` | Multi-LLM orchestration for Claude Code and Codex, with first-class `/octo:council`, agent summaries, prompt-size preflight, and research fanout. |
| Image Agency | `claude plugin install img@nyldn-plugins` or Codex `/plugins` as `img` | Generate and edit images with OpenAI GPT Image 2 and Gemini 3.1 Flash Image Preview. |

## Update

```bash
claude plugin marketplace update nyldn-plugins
claude plugin update octo@nyldn-plugins
claude plugin update img@nyldn-plugins
codex plugin marketplace upgrade nyldn-plugins
```

## Development

This repo is only the marketplace catalog. Plugin code lives in:

- https://github.com/nyldn/claude-octopus
- https://github.com/nyldn/img
