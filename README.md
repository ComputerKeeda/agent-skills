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

### Method 1: Packaged `.skill` File
Download [turbo-stack.skill](./turbo-stack.skill) and run the install command in your terminal:
```bash
claude skill add ./turbo-stack.skill
```

### Method 2: Manual / Custom Lock File
You can reference the raw `SKILL.md` directly in your workspace `skills-lock.json` file:
```json
"turbo-stack": {
  "source": "ComputerKeeda/agent-skills",
  "sourceType": "github",
  "skillPath": "skills/turbo-stack/SKILL.md"
}
```
