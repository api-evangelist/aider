# Aider (aider)
Aider is an open-source, terminal-based AI pair programmer that edits code directly inside a developer's local Git repository. Written in Python and distributed via PyPI under the Apache 2.0 license, Aider is a BYO-LLM tool: the user supplies API keys for hosted models (Anthropic Claude, OpenAI, DeepSeek, Google Gemini, OpenRouter, Mistral, xAI, GROQ, Cohere, GitHub Copilot, Azure OpenAI, Amazon Bedrock, Vertex AI) or points it at local models running through Ollama, LM Studio, or any OpenAI-compatible endpoint. Distinguishing capabilities include a repository-wide codebase map that lets the model reason about files it has not been shown, multi-file architectural edits with diff-based patching, automatic Git commits with conventional commit messages, a lint/test/repair loop, image and URL context, voice-to-code, and an IDE bridge via `--watch-files` that picks up `AI!` / `AI?` comments written from any editor. Aider supports 100+ programming languages via tree-sitter, publishes a public LLM coding leaderboard (the polyglot benchmark across C++, Go, Java, JavaScript, Python, Rust), and has accumulated 45K+ GitHub stars with 4.5K+ forks. The product surface is a rich CLI (40+ in-chat slash commands across four chat modes: code, architect, ask, help) plus a Python module entrypoint (`python -m aider`); there is no hosted SaaS, no Aider-operated REST API, and no app-level rate-limiting or billing — all model inference is delegated to the user's chosen provider, and any pricing, rate limits, and FinOps surface live with that provider.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - AI, AI Pair Programming, Developer Tools, CLI, Command Line, Coding Assistant, Code Generation, Open Source, Python, Apache 2.0, LLM, Git, BYO LLM, Terminal, Polyglot, Tree Sitter, Repository Map, Pair Programming

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-30

## APIs

### Aider CLI
Open-source terminal AI pair programmer distributed as the `aider-chat` PyPI package (entrypoint `aider`). Federates to user-supplied LLM providers (Anthropic, OpenAI, DeepSeek, Google Gemini, OpenRouter, Mistral, xAI, GROQ, Cohere, GitHub Copilot, Azure, Bedrock, Vertex, or any OpenAI-compatible endpoint including local models via Ollama and LM Studio). Provides four chat modes (code, architect, ask, help), 40+ in-chat slash commands, a repository-wide codebase map built with tree-sitter, multi-file diff-based edits in several edit formats (diff, whole, udiff, editor-diff), Git auto-commit with conventional commit messages, lint/test/repair loop, image and URL context, voice-to-code via the `/voice` command, and an IDE bridge via `--watch-files` that picks up `AI!` / `AI?` comments written from any editor. Configuration via command-line flags, environment variables (`AIDER_*`), `.env`, or `.aider.conf.yml`.

**Human URL:** [https://aider.chat/](https://aider.chat/)

#### Tags:

 - CLI, Open Source, AI Pair Programming, BYO LLM, Python, Tree Sitter, Repository Map

#### Properties

- [Documentation](https://aider.chat/docs/)
- [GitHub](https://github.com/Aider-AI/aider)
- [PyPI](https://pypi.org/project/aider-chat/)
- [Installation](https://aider.chat/docs/install.html)
- [UsageGuide](https://aider.chat/docs/usage.html)
- [Commands](https://aider.chat/docs/usage/commands.html)
- [ChatModes](https://aider.chat/docs/usage/modes.html)
- [Configuration](https://aider.chat/docs/config.html)
- [ConfigOptions](https://aider.chat/docs/config/options.html)
- [ConfigYAML](https://aider.chat/docs/config/aider_conf.html)
- [ConfigEnv](https://aider.chat/docs/config/dotenv.html)
- [APIKeys](https://aider.chat/docs/config/api-keys.html)
- [SupportedModels](https://aider.chat/docs/llms.html)
- [ModelWarnings](https://aider.chat/docs/llms/warnings.html)
- [EditFormats](https://aider.chat/docs/more/edit-formats.html)
- [Leaderboard](https://aider.chat/docs/leaderboards/)
- [ChangeLog](https://aider.chat/HISTORY.html)
- [License](https://github.com/Aider-AI/aider/blob/main/LICENSE.txt)
- [SourceCode](https://github.com/Aider-AI/aider)
- [IssueTracker](https://github.com/Aider-AI/aider/issues)
- [Tutorials](https://aider.chat/docs/usage/tutorials.html)
- [WatchFilesGuide](https://aider.chat/docs/usage/watch.html)
- [VoiceGuide](https://aider.chat/docs/usage/voice.html)
- [ConventionsGuide](https://aider.chat/docs/usage/conventions.html)
- [OpenAPI](openapi/aider-cli-openapi.yml)
- [NaftikoCapability](capabilities/aider-cli.yaml)

### Aider Python Module
Aider exposes a Python module entrypoint (`python -m aider`) and an importable package (`aider.main.main`) so Aider can be embedded in Python scripts, CI workflows, and other agents. The same flags and configuration that drive the CLI apply to module invocation. There is no documented stable Python SDK contract beyond `main()` — the internal `Coder`, `Model`, `IO`, and `Commands` classes are public but versioned with the CLI and may change between releases.

**Human URL:** [https://github.com/Aider-AI/aider/blob/main/aider/main.py](https://github.com/Aider-AI/aider/blob/main/aider/main.py)

#### Tags:

 - Python, Library, Embedding, Open Source

#### Properties

- [SourceCode](https://github.com/Aider-AI/aider/blob/main/aider/main.py)
- [PyPI](https://pypi.org/project/aider-chat/)
- [Documentation](https://aider.chat/docs/scripting.html)
- [Scripting](https://aider.chat/docs/scripting.html)

## Common Properties

- [Website](https://aider.chat/)
- [Documentation](https://aider.chat/docs/)
- [GitHub](https://github.com/Aider-AI/aider)
- [GitHubOrg](https://github.com/Aider-AI)
- [Issues](https://github.com/Aider-AI/aider/issues)
- [Discussions](https://github.com/Aider-AI/aider/discussions)
- [PyPI](https://pypi.org/project/aider-chat/)
- [Installation](https://aider.chat/docs/install.html)
- [UsageGuide](https://aider.chat/docs/usage.html)
- [Configuration](https://aider.chat/docs/config.html)
- [SupportedModels](https://aider.chat/docs/llms.html)
- [Leaderboard](https://aider.chat/docs/leaderboards/)
- [Blog](https://aider.chat/blog/)
- [ChangeLog](https://aider.chat/HISTORY.html)
- [License](https://github.com/Aider-AI/aider/blob/main/LICENSE.txt)
- [Discord](https://discord.gg/Tv2uQnR88V)
- [Twitter](https://twitter.com/paulgauthier)
- [Conventions](https://github.com/Aider-AI/conventions)
- [Benchmarks](https://github.com/Aider-AI/polyglot-benchmark)
- [Tools — aider-install Bootstrapper](https://github.com/Aider-AI/aider-install)
- [Tools — grep-ast Repository Map Helper](https://github.com/Aider-AI/grep-ast)
- [Tools — Polyglot Benchmark Suite](https://github.com/Aider-AI/polyglot-benchmark)
- [Tools — Refactor Benchmark Suite](https://github.com/Aider-AI/refactor-benchmark)
- [Tools — SWE-Bench Harness](https://github.com/Aider-AI/aider-swe-bench)
- [Tools — MCP Server (Community — disler/aider-mcp-server)](https://github.com/disler/aider-mcp-server)
- [Tools — MCP Server (Community — sengokudaikon/aider-mcp-server)](https://github.com/sengokudaikon/aider-mcp-server)
- [Tools — MCP Package Manager for Aider (mcpm-aider)](https://github.com/lutzleonhardt/mcpm-aider)
- [Integrations — NeoVim Plugin (aider.nvim)](https://github.com/joshuavial/aider.nvim)
- [Rules](rules/aider-rules.yml)
- [Vocabulary](vocabulary/aider-vocabulary.yml)
- [RateLimits](rate-limits/aider-rate-limits.yml)
- [JSONLD](json-ld/aider-cli-context.jsonld)

## Features

| Name | Description |
|------|-------------|
| Repository Map | Aider builds a tree-sitter-powered map of the entire repository so the LLM can reason about files that haven't been explicitly added to the chat. The map is automatically refreshed and can be inspected via `/map` or rebuilt via `/map-refresh`. |
| Architect / Editor Split | Architect mode pairs a reasoning-strong model (planning) with a separate editor model (file edits). This separates the cost of thinking from the cost of writing diffs and lets weaker editor models execute plans from stronger architects. |
| Watch Files Mode | `--watch-files` lets aider sit in a terminal alongside any editor; it reacts to `AI!` and `AI?` comments authored from VS Code, Cursor, JetBrains, Vim, or any other editor. |
| Voice to Code | `/voice` records microphone input, transcribes it (Whisper-style), and feeds it into the chat as a prompt. Optional PortAudio install required on Mac/Linux. |
| Auto Git Commits | Every AI-applied change is automatically committed with a conventional commit message. `/undo` rolls back the last commit; `/diff` shows what changed since the last message. |
| Lint and Test Repair Loop | `--auto-lint` and `--auto-test` re-run linters and tests after every edit; failures are fed back into the LLM so it can self-repair until the suite passes. |
| Polyglot Benchmark | Aider publishes a public leaderboard scoring frontier LLMs against 225 Exercism exercises across C++, Go, Java, JavaScript, Python, and Rust — separating edit-format accuracy from raw correctness. |
| BYO LLM | No vendor lock-in. The user supplies the API key for any of 15+ supported providers (or points at a local Ollama / LM Studio endpoint). Pricing, rate limits, and billing live entirely with the upstream provider. |
| Multiple Edit Formats | Aider supports `diff`, `whole`, `udiff`, and `editor-diff` edit formats so the LLM can apply changes in whatever shape it executes most reliably. Edit format is auto-selected per model and can be overridden via `--edit-format`. |

## Use Cases

| Name | Description |
|------|-------------|
| Multi-File Refactor | Use architect mode with a reasoning model to plan a cross-cutting refactor, then have aider apply the edits across dozens of files in one pass, with each edit auto-committed. |
| Test-Driven Bug Fixing | `/test` runs the suite, the failure goes back to the model, the model proposes a fix, `/test` re-runs until green. The whole loop happens without leaving the terminal. |
| Editor-Bridged Pair Programming | Run `aider --watch-files` in one pane and any editor in another; drop `# AI! make this idempotent` into the source file and aider picks it up, edits, and commits. |
| Local Model Coding | Point aider at an OpenAI-compatible Ollama or LM Studio endpoint to get a fully offline coding workflow with no data ever leaving the developer's machine. |
| Benchmark Authoring | Use the polyglot, refactor, and SWE-Bench harnesses (in the Aider-AI GitHub org) to benchmark a new model or new prompt strategy against a reproducible, published scoreboard. |

## Integrations

| Name | Description |
|------|-------------|
| Anthropic Claude | First-class support for Claude Sonnet, Opus, and Haiku via Anthropic direct API or Bedrock / Vertex. `--model claude-...` or `ANTHROPIC_API_KEY` in the environment. |
| OpenAI | Support for GPT-4.1, o3, o4-mini, GPT-5 family, and Responses API models (o1-pro, o3-pro). `--model gpt-...` or `OPENAI_API_KEY`. |
| Google Gemini | Gemini 2.5 Pro and Flash via direct API or Vertex. Free tier available through `gemini-2.5-pro-exp`. |
| DeepSeek | DeepSeek R1 (reasoner) and V3 via the DeepSeek API or third-party providers. |
| OpenRouter | Unified gateway to dozens of frontier and open models, with daily free quota. |
| xAI Grok | Grok-4 and earlier Grok models via xAI API. |
| Mistral | Mistral hosted models via Mistral La Plateforme. |
| Ollama | Local model execution for fully offline coding workflows. |
| LM Studio | Local OpenAI-compatible endpoint for self-hosted models. |
| Azure OpenAI | Enterprise OpenAI deployments via Azure with custom endpoint support. |
| Amazon Bedrock | Claude and other Bedrock-hosted models via AWS credentials. |
| Vertex AI | Gemini and partner models via Google Cloud Vertex AI. |
| GROQ | Fast inference for Llama and Mixtral via GROQ Cloud. |
| GitHub Copilot | Aider can route through a GitHub Copilot subscription as the model backend. |
| Cohere | Cohere Command-family models for chat and code completion. |
| Git | Aider requires a Git repo by default; every applied edit is committed automatically. Configurable via `--git` / `--auto-commits` / `--dirty-commits`. |
| NeoVim (aider.nvim) | Community NeoVim plugin pairs aider with an in-editor experience. |
| VS Code Terminal | No official extension; runs natively in VS Code's integrated terminal. `--watch-files` makes the IDE pairing work via AI! / AI? comments. |

## Solutions

| Name | Description |
|------|-------------|
| Offline Coding Assistant | Run aider against a local Ollama or LM Studio server to get AI-assisted refactoring, test repair, and architectural edits with no data ever leaving the developer's machine. |
| Cross-Model Benchmarking | Use Aider's polyglot benchmark harness to score any new LLM against a reproducible 225-task suite across six languages, with per-language and edit-format-accuracy breakdowns. |
| Editor-Native AI Workflow | Pair `--watch-files` with VS Code, JetBrains, NeoVim, or any editor to drive aider from inline `AI!` / `AI?` comments — no extension required. |
| MCP-Wrapped Aider | Community MCP servers (`disler/aider-mcp-server`, `sengokudaikon/aider-mcp-server`) expose aider AS an MCP tool, letting Claude Code, Cursor, or any MCP client offload editing work to aider. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Aider CLI OpenAPI](openapi/aider-cli-openapi.yml) — 39 paths, 40 operations, 28 schemas across 14 tags modeling the aider CLI command surface as REST.

### JSON Schema

26 standalone JSON Schema files (one per component schema) in [`json-schema/`](json-schema/). Highlights:

- [EditRequest](json-schema/aider-cli-edit-request-schema.json), [EditResult](json-schema/aider-cli-edit-result-schema.json)
- [AddFilesRequest](json-schema/aider-cli-add-files-request-schema.json), [FileListing](json-schema/aider-cli-file-listing-schema.json)
- [LaunchConfig](json-schema/aider-cli-launch-config-schema.json), [SettingsSnapshot](json-schema/aider-cli-settings-snapshot-schema.json)
- [ModelSelection](json-schema/aider-cli-model-selection-schema.json), [ModelCatalog](json-schema/aider-cli-model-catalog-schema.json)
- [DiffResult](json-schema/aider-cli-diff-result-schema.json), [CommitResult](json-schema/aider-cli-commit-result-schema.json)
- [RepositoryMap](json-schema/aider-cli-repository-map-schema.json), [TokenUsage](json-schema/aider-cli-token-usage-schema.json)
- [ShellRequest](json-schema/aider-cli-shell-request-schema.json), [ShellResult](json-schema/aider-cli-shell-result-schema.json)
- [VoiceTranscript](json-schema/aider-cli-voice-transcript-schema.json), [WebFetchRequest](json-schema/aider-cli-web-fetch-request-schema.json), [WebFetchResult](json-schema/aider-cli-web-fetch-result-schema.json)

### JSON Structure

26 JSON Structure (json-structure.org draft) files in [`json-structure/`](json-structure/), one per schema, with strict typing applied (datetime, int32, double, uri, uuid).

### JSON-LD

- [Aider CLI Context](json-ld/aider-cli-context.jsonld) — 1 context document with 26 type declarations and 63 property term mappings linking aider's vocabulary to `schema.org`, `dcterms`, and XSD datatypes.

### Examples

26 representative request/response example payloads in [`examples/`](examples/), one per schema, deterministically generated from the OpenAPI components.

## Capabilities

Naftiko capabilities organized as self-contained workflow files. Each file is fully inline (consumes + REST + MCP exposers) with no shared subfolder.

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Aider CLI — Full Command Surface](capabilities/aider-cli.yaml) | aider-cli | 40 | Pair Programmer / Agent Runtime |

## Vocabulary

- [Aider Vocabulary](vocabulary/aider-vocabulary.yml) — Unified taxonomy mapping 16 resources, 26 actions, 1 workflow, and 3 personas across operational (OpenAPI) and capability (Naftiko) dimensions.

## Rules

- [Aider Spectral Rules](rules/aider-rules.yml) — 38 rules across 13 categories enforcing aider's CLI-as-API conventions (kebab-case paths, Title Case summaries with "Aider " prefix, camelCase operationIds, snake_case schema properties, JSON content type, Apache 2.0 license, BYO-LLM security scheme).

## Rate Limits

- [Aider Rate Limits](rate-limits/aider-rate-limits.yml) — Documents that aider has no app-level rate limit; all throttling is delegated to the upstream LLM provider bound via API key. Includes the repo-map and chat-history token budget context-window controls.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
