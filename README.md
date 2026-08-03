# Aider (aider)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Aider is an open-source, terminal-based AI pair programmer that edits code directly inside a developer's local Git repository. Written in Python and distributed via PyPI under the Apache 2.0 license, Aider is a BYO-LLM tool: the user supplies API keys for hosted models (Anthropic Claude, OpenAI, DeepSeek, Google Gemini, OpenRouter, Mistral, xAI, GROQ, Cohere, GitHub Copilot, Azure OpenAI, Amazon Bedrock, Vertex AI) or points it at local models running through Ollama, LM Studio, or any OpenAI-compatible endpoint. Distinguishing capabilities include a repository-wide codebase map that lets the model reason about files it has not been shown, multi-file architectural edits with diff-based patching, automatic Git commits with conventional commit messages, a lint/test/repair loop, image and URL context, voice-to-code, and an IDE bridge via `--watch-files` that picks up `AI!` / `AI?` comments written from any editor. Aider supports 100+ programming languages via tree-sitter, publishes a public LLM coding leaderboard (the polyglot benchmark across C++, Go, Java, JavaScript, Python, Rust), and has accumulated 45K+ GitHub stars with 4.5K+ forks. The product surface is a rich CLI (40+ in-chat slash commands across four chat modes: code, architect, ask, help) plus a Python module entrypoint (`python -m aider`); there is no hosted SaaS, no Aider-operated REST API, and no app-level rate-limiting or billing — all model inference is delegated to the user's chosen provider, and any pricing, rate limits, and FinOps surface live with that provider.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Provider
- **Access:** Open Source

## Tags

- AI
- AI Pair Programming
- Developer Tools
- CLI
- Command Line
- Coding Assistant
- Code Generation
- Open Source
- Python
- Apache 2.0
- LLM
- Git
- BYO LLM
- Terminal
- Polyglot
- Tree Sitter
- Repository Map
- Pair Programming

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-30

## APIs

### Aider CLI

Open-source terminal AI pair programmer distributed as the `aider-chat` PyPI package (entrypoint `aider`). Federates to user-supplied LLM providers (Anthropic, OpenAI, DeepSeek, Google Gemini, OpenRouter, Mistral, xAI, GROQ, Cohere, GitHub Copilot, Azure, Bedrock, Vertex, or any OpenAI-compatible endpoint including local models via Ollama and LM Studio). Provides four chat modes (code, architect, ask, help), 40+ in-chat slash commands, a repository-wide codebase map built with tree-sitter, multi-file diff-based edits in several edit formats (diff, whole, udiff, editor-diff), Git auto-commit with conventional commit messages, lint/test/repair loop, image and URL context, voice-to-code via the `/voice` command, and an IDE bridge via `--watch-files` that picks up `AI!` / `AI?` comments written from any editor. Configuration via command-line flags, environment variables (`AIDER_*`), `.env`, or `.aider.conf.yml`.

- **Human URL:** [https://aider.chat/](https://aider.chat/)
- **Base URL:** `https://aider.chat`

#### Tags

- CLI
- Open Source
- AI Pair Programming
- BYO LLM
- Python
- Tree Sitter
- Repository Map

#### Properties

- [Documentation](https://aider.chat/docs/)
- [Git Hub](https://github.com/Aider-AI/aider)
- [Py P I](https://pypi.org/project/aider-chat/)
- [Installation](https://aider.chat/docs/install.html)
- [Usage Guide](https://aider.chat/docs/usage.html)
- [Commands](https://aider.chat/docs/usage/commands.html)
- [Chat Modes](https://aider.chat/docs/usage/modes.html)
- [Configuration](https://aider.chat/docs/config.html)
- [Config Options](https://aider.chat/docs/config/options.html)
- [Config Y A M L](https://aider.chat/docs/config/aider_conf.html)
- [Config Env](https://aider.chat/docs/config/dotenv.html)
- [A P I Keys](https://aider.chat/docs/config/api-keys.html)
- [Supported Models](https://aider.chat/docs/llms.html)
- [Model Warnings](https://aider.chat/docs/llms/warnings.html)
- [Edit Formats](https://aider.chat/docs/more/edit-formats.html)
- [Leaderboard](https://aider.chat/docs/leaderboards/)
- [Changelog](https://aider.chat/HISTORY.html)
- [License](https://github.com/Aider-AI/aider/blob/main/LICENSE.txt)
- [Source Code](https://github.com/Aider-AI/aider)
- [Issue Tracker](https://github.com/Aider-AI/aider/issues)
- [Tutorials](https://aider.chat/docs/usage/tutorials.html)
- [Watch Files Guide](https://aider.chat/docs/usage/watch.html)
- [Voice Guide](https://aider.chat/docs/usage/voice.html)
- [Conventions Guide](https://aider.chat/docs/usage/conventions.html)
- [OpenAPI](openapi/aider-cli-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/aider-cli.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/aider-cli.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Aider Python Module

Aider exposes a Python module entrypoint (`python -m aider`) and an importable package (`aider.main.main`) so Aider can be embedded in Python scripts, CI workflows, and other agents. The same flags and configuration that drive the CLI apply to module invocation. There is no documented stable Python SDK contract beyond `main()` — the internal `Coder`, `Model`, `IO`, and `Commands` classes are public but versioned with the CLI and may change between releases.

- **Human URL:** [https://github.com/Aider-AI/aider/blob/main/aider/main.py](https://github.com/Aider-AI/aider/blob/main/aider/main.py)
- **Base URL:** `https://github.com/Aider-AI/aider`

#### Tags

- Python
- Library
- Embedding
- Open Source

#### Properties

- [Source Code](https://github.com/Aider-AI/aider/blob/main/aider/main.py)
- [Py P I](https://pypi.org/project/aider-chat/)
- [Documentation](https://aider.chat/docs/scripting.html)
- [Scripting](https://aider.chat/docs/scripting.html)
- [Postman Collection](collections/aider-cli.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/aider-cli.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://aider.chat/)
- [Documentation](https://aider.chat/docs/)
- [Git Hub](https://github.com/Aider-AI/aider)
- [Git Hub Org](https://github.com/Aider-AI)
- [Issues](https://github.com/Aider-AI/aider/issues)
- [Discussions](https://github.com/Aider-AI/aider/discussions)
- [Py P I](https://pypi.org/project/aider-chat/)
- [Installation](https://aider.chat/docs/install.html)
- [Usage Guide](https://aider.chat/docs/usage.html)
- [Configuration](https://aider.chat/docs/config.html)
- [Supported Models](https://aider.chat/docs/llms.html)
- [Leaderboard](https://aider.chat/docs/leaderboards/)
- [Blog](https://aider.chat/blog/)
- [Changelog](https://aider.chat/HISTORY.html)
- [License](https://github.com/Aider-AI/aider/blob/main/LICENSE.txt)
- [Discord](https://discord.gg/Tv2uQnR88V)
- [Twitter](https://twitter.com/paulgauthier)
- [Conventions](https://github.com/Aider-AI/conventions)
- [Benchmarks](https://github.com/Aider-AI/polyglot-benchmark)
- [Tools](https://github.com/Aider-AI/aider-install)
- [Tools](https://github.com/Aider-AI/grep-ast)
- [Tools](https://github.com/Aider-AI/polyglot-benchmark)
- [Tools](https://github.com/Aider-AI/refactor-benchmark)
- [Tools](https://github.com/Aider-AI/aider-swe-bench)
- [Tools](https://github.com/disler/aider-mcp-server)
- [Tools](https://github.com/sengokudaikon/aider-mcp-server)
- [Tools](https://github.com/lutzleonhardt/mcpm-aider)
- [Integrations](https://github.com/joshuavial/aider.nvim)
- [Rules](rules/aider-rules.yml)
- [Vocabulary](vocabulary/aider-vocabulary.yml)
- [Rate Limits](rate-limits/aider-rate-limits.yml)
- [JSON-LD](json-ld/aider-cli-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
