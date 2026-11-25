# Aider

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
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

**Areas:** Artificial Intelligence · AI Pair Programming · Developer Tools · CLI · Command Line · Coding Assistant · Code Generation · Open Source · Python · Apache 2.0 · LLM · Version Control

## Aider on APIs.io

Everything profiled for Aider is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/aider/](https://apis.io/providers/aider/)** — or go straight to one of the APIs or properties below.

### APIs (15)

- [Aider Python Module](https://apis.io/apis/aider/python-module/) — Aider exposes a Python module entrypoint (`python -m aider`) and an importable package (`aider.main.main`) so Aider can be embedded in Python scripts, CI…
- [Aider Chat API](https://apis.io/apis/aider/aider-chat-api/) — Aider Commands That Manage the Chat Session and History.
- [Aider Editing API](https://apis.io/apis/aider/aider-editing-api/) — Aider Commands That Drive Code Edits and Diffs.
- [Aider Files API](https://apis.io/apis/aider/aider-files-api/) — Aider Commands That Manage Files in the Chat Session.
- [Aider Git API](https://apis.io/apis/aider/aider-git-api/) — Aider Commands That Wrap Git Operations.
- [Aider Launch API](https://apis.io/apis/aider/aider-launch-api/) — Aider Launch-Time Configuration via Flags, YAML, and Environment Variables.
- [Aider Map API](https://apis.io/apis/aider/aider-map-api/) — Aider Repository-Map Inspection.
- [Aider Models API](https://apis.io/apis/aider/aider-models-api/) — Aider Commands That Switch or Query LLM Models.
- [Aider Modes API](https://apis.io/apis/aider/aider-modes-api/) — Aider Chat Modes (Code, Architect, Ask, Help, Context).
- [Aider Quality API](https://apis.io/apis/aider/aider-quality-api/) — Aider Commands That Run Linters and Tests.
- [Aider Session API](https://apis.io/apis/aider/aider-session-api/) — Aider Session Lifecycle Commands.
- [Aider Settings API](https://apis.io/apis/aider/aider-settings-api/) — Aider Settings, Tokens, and Reasoning Controls.
- [Aider Voice API](https://apis.io/apis/aider/aider-voice-api/) — Aider Voice-to-Code Input.
- [Aider Web API](https://apis.io/apis/aider/aider-web-api/) — Aider Commands That Pull in Web Content.
- [Aider I/O API](https://apis.io/apis/aider/aider-i-o-api/) — Aider Commands That Move Data In and Out of the Session.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Aider Agentic Access](https://apis.io/agentic-access/aider/aider-agentic-access/)

#### JSON Schema (26)

The data models the API reads and writes.

- [AddFilesRequest](https://apis.io/schemas/aider/aider-cli-add-files-request/)
- [AskRequest](https://apis.io/schemas/aider/aider-cli-ask-request/)
- [AskResponse](https://apis.io/schemas/aider/aider-cli-ask-response/)
- [ChatModeRequest](https://apis.io/schemas/aider/aider-cli-chat-mode-request/)
- [CommitRequest](https://apis.io/schemas/aider/aider-cli-commit-request/)
- [CommitResult](https://apis.io/schemas/aider/aider-cli-commit-result/)
- [DiffResult](https://apis.io/schemas/aider/aider-cli-diff-result/)
- [DropFilesRequest](https://apis.io/schemas/aider/aider-cli-drop-files-request/)
- [EditRequest](https://apis.io/schemas/aider/aider-cli-edit-request/)
- [EditResult](https://apis.io/schemas/aider/aider-cli-edit-result/)
- [FileListing](https://apis.io/schemas/aider/aider-cli-file-listing/)
- [FilePathRequest](https://apis.io/schemas/aider/aider-cli-file-path-request/)
- [LaunchConfig](https://apis.io/schemas/aider/aider-cli-launch-config/)
- [LintRequest](https://apis.io/schemas/aider/aider-cli-lint-request/)
- [ModelCatalog](https://apis.io/schemas/aider/aider-cli-model-catalog/)
- [ModelSelection](https://apis.io/schemas/aider/aider-cli-model-selection/)
- [ReasoningEffortRequest](https://apis.io/schemas/aider/aider-cli-reasoning-effort-request/)
- [RepositoryMap](https://apis.io/schemas/aider/aider-cli-repository-map/)
- [SettingsSnapshot](https://apis.io/schemas/aider/aider-cli-settings-snapshot/)
- [ShellRequest](https://apis.io/schemas/aider/aider-cli-shell-request/)
- [ShellResult](https://apis.io/schemas/aider/aider-cli-shell-result/)
- [ThinkingTokensRequest](https://apis.io/schemas/aider/aider-cli-thinking-tokens-request/)
- [TokenUsage](https://apis.io/schemas/aider/aider-cli-token-usage/)
- [VoiceTranscript](https://apis.io/schemas/aider/aider-cli-voice-transcript/)
- [WebFetchRequest](https://apis.io/schemas/aider/aider-cli-web-fetch-request/)
- …and 1 more published on APIs.io

#### JSON Structure (26)

Data models expressed in JSON Structure.

- [Aider Cli Add Files Request Structure](https://apis.io/json-structure/aider/aider-cli-add-files-request-structure/)
- [Aider Cli Ask Request Structure](https://apis.io/json-structure/aider/aider-cli-ask-request-structure/)
- [Aider Cli Ask Response Structure](https://apis.io/json-structure/aider/aider-cli-ask-response-structure/)
- [Aider Cli Chat Mode Request Structure](https://apis.io/json-structure/aider/aider-cli-chat-mode-request-structure/)
- [Aider Cli Commit Request Structure](https://apis.io/json-structure/aider/aider-cli-commit-request-structure/)
- [Aider Cli Commit Result Structure](https://apis.io/json-structure/aider/aider-cli-commit-result-structure/)
- [Aider Cli Diff Result Structure](https://apis.io/json-structure/aider/aider-cli-diff-result-structure/)
- [Aider Cli Drop Files Request Structure](https://apis.io/json-structure/aider/aider-cli-drop-files-request-structure/)
- [Aider Cli Edit Request Structure](https://apis.io/json-structure/aider/aider-cli-edit-request-structure/)
- [Aider Cli Edit Result Structure](https://apis.io/json-structure/aider/aider-cli-edit-result-structure/)
- [Aider Cli File Listing Structure](https://apis.io/json-structure/aider/aider-cli-file-listing-structure/)
- [Aider Cli File Path Request Structure](https://apis.io/json-structure/aider/aider-cli-file-path-request-structure/)
- [Aider Cli Launch Config Structure](https://apis.io/json-structure/aider/aider-cli-launch-config-structure/)
- [Aider Cli Lint Request Structure](https://apis.io/json-structure/aider/aider-cli-lint-request-structure/)
- [Aider Cli Model Catalog Structure](https://apis.io/json-structure/aider/aider-cli-model-catalog-structure/)
- [Aider Cli Model Selection Structure](https://apis.io/json-structure/aider/aider-cli-model-selection-structure/)
- [Aider Cli Reasoning Effort Request Structure](https://apis.io/json-structure/aider/aider-cli-reasoning-effort-request-structure/)
- [Aider Cli Repository Map Structure](https://apis.io/json-structure/aider/aider-cli-repository-map-structure/)
- [Aider Cli Settings Snapshot Structure](https://apis.io/json-structure/aider/aider-cli-settings-snapshot-structure/)
- [Aider Cli Shell Request Structure](https://apis.io/json-structure/aider/aider-cli-shell-request-structure/)
- [Aider Cli Shell Result Structure](https://apis.io/json-structure/aider/aider-cli-shell-result-structure/)
- [Aider Cli Thinking Tokens Request Structure](https://apis.io/json-structure/aider/aider-cli-thinking-tokens-request-structure/)
- [Aider Cli Token Usage Structure](https://apis.io/json-structure/aider/aider-cli-token-usage-structure/)
- [Aider Cli Voice Transcript Structure](https://apis.io/json-structure/aider/aider-cli-voice-transcript-structure/)
- [Aider Cli Web Fetch Request Structure](https://apis.io/json-structure/aider/aider-cli-web-fetch-request-structure/)
- …and 1 more published on APIs.io

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Aider Cli Context](https://apis.io/jsonld/aider/aider-cli-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Aider Vocabulary](https://apis.io/vocabularies/aider/aider-vocabulary/)

#### Examples (26)

Example requests and responses.

- [Aider Cli Add Files Request Example](https://apis.io/examples/aider/aider-cli-add-files-request-example/)
- [Aider Cli Ask Request Example](https://apis.io/examples/aider/aider-cli-ask-request-example/)
- [Aider Cli Ask Response Example](https://apis.io/examples/aider/aider-cli-ask-response-example/)
- [Aider Cli Chat Mode Request Example](https://apis.io/examples/aider/aider-cli-chat-mode-request-example/)
- [Aider Cli Commit Request Example](https://apis.io/examples/aider/aider-cli-commit-request-example/)
- [Aider Cli Commit Result Example](https://apis.io/examples/aider/aider-cli-commit-result-example/)
- [Aider Cli Diff Result Example](https://apis.io/examples/aider/aider-cli-diff-result-example/)
- [Aider Cli Drop Files Request Example](https://apis.io/examples/aider/aider-cli-drop-files-request-example/)
- [Aider Cli Edit Request Example](https://apis.io/examples/aider/aider-cli-edit-request-example/)
- [Aider Cli Edit Result Example](https://apis.io/examples/aider/aider-cli-edit-result-example/)
- [Aider Cli File Listing Example](https://apis.io/examples/aider/aider-cli-file-listing-example/)
- [Aider Cli File Path Request Example](https://apis.io/examples/aider/aider-cli-file-path-request-example/)
- [Aider Cli Launch Config Example](https://apis.io/examples/aider/aider-cli-launch-config-example/)
- [Aider Cli Lint Request Example](https://apis.io/examples/aider/aider-cli-lint-request-example/)
- [Aider Cli Model Catalog Example](https://apis.io/examples/aider/aider-cli-model-catalog-example/)
- [Aider Cli Model Selection Example](https://apis.io/examples/aider/aider-cli-model-selection-example/)
- [Aider Cli Reasoning Effort Request Example](https://apis.io/examples/aider/aider-cli-reasoning-effort-request-example/)
- [Aider Cli Repository Map Example](https://apis.io/examples/aider/aider-cli-repository-map-example/)
- [Aider Cli Settings Snapshot Example](https://apis.io/examples/aider/aider-cli-settings-snapshot-example/)
- [Aider Cli Shell Request Example](https://apis.io/examples/aider/aider-cli-shell-request-example/)
- [Aider Cli Shell Result Example](https://apis.io/examples/aider/aider-cli-shell-result-example/)
- [Aider Cli Thinking Tokens Request Example](https://apis.io/examples/aider/aider-cli-thinking-tokens-request-example/)
- [Aider Cli Token Usage Example](https://apis.io/examples/aider/aider-cli-token-usage-example/)
- [Aider Cli Voice Transcript Example](https://apis.io/examples/aider/aider-cli-voice-transcript-example/)
- [Aider Cli Web Fetch Request Example](https://apis.io/examples/aider/aider-cli-web-fetch-request-example/)
- …and 1 more published on APIs.io

#### Collections (15)

Postman and Open Collection request collections.

- [Aider CLI Chat API](https://apis.io/collections/aider/open-aider-chat-api/)
- [Aider CLI](https://apis.io/collections/aider/open-aider-cli/)
- [Aider CLI Chat Editing API](https://apis.io/collections/aider/open-aider-editing-api/)
- [Aider CLI Chat Files API](https://apis.io/collections/aider/open-aider-files-api/)
- [Aider CLI Chat Git API](https://apis.io/collections/aider/open-aider-git-api/)
- [Aider CLI Chat IO API](https://apis.io/collections/aider/open-aider-io-api/)
- [Aider CLI Chat Launch API](https://apis.io/collections/aider/open-aider-launch-api/)
- [Aider CLI Chat Map API](https://apis.io/collections/aider/open-aider-map-api/)
- [Aider CLI Chat Models API](https://apis.io/collections/aider/open-aider-models-api/)
- [Aider CLI Chat Modes API](https://apis.io/collections/aider/open-aider-modes-api/)
- [Aider CLI Chat Quality API](https://apis.io/collections/aider/open-aider-quality-api/)
- [Aider CLI Chat Session API](https://apis.io/collections/aider/open-aider-session-api/)
- [Aider CLI Chat Settings API](https://apis.io/collections/aider/open-aider-settings-api/)
- [Aider CLI Chat Voice API](https://apis.io/collections/aider/open-aider-voice-api/)
- [Aider CLI Chat Web API](https://apis.io/collections/aider/open-aider-web-api/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Aider — jsonschema rules](https://apis.io/rules/aider/aider-jsonschema-spectral-rules/)
- [Aider API Rules](https://apis.io/rules/aider/aider-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Aider Authentication](https://apis.io/security/aider/aider-authentication/)
- [Aider Domain Security](https://apis.io/security/aider/aider-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Moved to /providers/aider/](https://apis.io/plans/aider/aider-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Aider Rate Limits](https://apis.io/rate-limits/aider/aider-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Moved to /providers/aider/](https://apis.io/finops/aider/aider-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://aider.chat/)
- [Documentation](https://aider.chat/docs/)
- [Changelog](https://aider.chat/HISTORY.html)
- [Blog](https://aider.chat/blog/)

## API Evangelist rating

**Kin Score 26.1** — emerging · rubric 0.28.1 · scored 2026-11-21

| Facet | Score |
|---|---|
| Discoverability | 62.5 |
| Contract quality | 20.4 |
| Contract governance | 27.3 |
| Operational transparency | 26.2 |
| Developer ergonomics | 28.6 |
| Access clarity | 6.4 |

**Agent readiness 23.3** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | partial |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |
| MCP Tool Quality | na |
| Onboarding Descriptor | — |
| Dns Aid Index | na |
| Markdown Negotiation | na |

**Regulatory alignment 10.0** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/aider/](https://apis.io/providers/aider/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Aider: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/aider/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
