# Platform Adapters

Platform-specific configuration files and instructions to connect the Tanasub Open writing system (`SKILL.md`) to various AI platforms and chatbots.

| Platform | Config mechanism | Adapter file |
|---|---|---|
| Aider | CLI flag (`--read`) or `.aider.conf.yml` | [aider-conventions.md](aider-conventions.md) |
| Antigravity | Skill directory (`.agents/skills/`) | [antigravity.md](antigravity.md) |
| ChatGPT | Custom GPT instructions / Project Knowledge | [chatgpt-custom-gpt.md](chatgpt-custom-gpt.md) |
| Claude Chat | Projects / attachments | [claude-chat.md](claude-chat.md) |
| Claude Code | `CLAUDE.md` / `~/.claude/CLAUDE.md` | [claude-code.md](claude-code.md) |
| Cursor | `.cursor/rules/*.mdc` | [cursor-rules.md](cursor-rules.md) |
| GitHub Copilot | `.github/copilot-instructions.md` | [copilot-instructions.md](copilot-instructions.md) |
| Grok Build | `AGENTS.md` / `.grok/config.toml` | [grok-build.md](grok-build.md) |
| OpenAI Codex CLI | `AGENTS.md` / `~/.codex/AGENTS.md` | [codex-cli.md](codex-cli.md) |
| OpenCode | `AGENTS.md` / `~/.config/opencode/AGENTS.md` | [opencode.md](opencode.md) |
| OpenHands | `.openhands/microagents/` | [openhands.md](openhands.md) |
| Z.ai / ZCode | `AGENTS.md` | [z-ai.md](z-ai.md) |
| Generic LLM | System prompt / developer instructions | [generic-system-prompt.md](generic-system-prompt.md) |
