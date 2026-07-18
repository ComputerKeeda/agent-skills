# Agent Skills

A collection of custom skills for AI coding assistants.

## Included Skills

### 🚀 turbo-stack
Act as a rigorous performance engineer to analyze code bases, architecture plans, or specific code snippets to catch and eliminate latency bottlenecks.

#### Features
1. **Synchronous UI Blocking**: Refactors to Optimistic UI patterns for instantaneous user updates.
2. **Uncompressed Data Transfer**: Recommends payload compression (Gzip/Brotli) or binary serialization (gRPC/Protobuf).
3. **Row-by-Row Database Inserts**: Optimizes loops into batch/bulk inserts or single-transaction executions.
4. **Hidden Dependency Bottlenecks**: Decouples slow third-party services into background tasks and updates UI status.
5. **Redundant Server Rendering**: Implements caching (Redis/reverse-proxy) or static pre-rendering.

---

## Installation

You can install skills from this repository into any of the 18+ supported AI coding assistants (like Claude Code, Cursor, Codex, Windsurf, or Cline) using Vercel Labs' universal `skills` CLI.

### Universal CLI Installation (Recommended)
Run the following command at the root of your project:
```bash
npx skills add ComputerKeeda/agent-skills --skill turbo-stack
```

To install all skills currently available in this repository:
```bash
npx skills add ComputerKeeda/agent-skills --skill '*'
```

### Manual Installation
You can reference the skill directly in your workspace `skills-lock.json` file:
```json
{
  "skills": {
    "turbo-stack": {
      "source": "ComputerKeeda/agent-skills",
      "sourceType": "github",
      "skillPath": "skills/turbo-stack/SKILL.md"
    }
  }
}
```
