# AI Code Lint — Catch AI-Generated Code Issues

[![Marketplace](https://img.shields.io/badge/Marketplace-ai--lint-purple)](https://github.com/marketplace/actions/ai-lint)
[![Version](https://img.shields.io/badge/version-1.0.0-green)](https://github.com/CodeGero/ai-lint/releases)

**AI writes code fast. It also hallucinates APIs, skips error handling, and over-engineers solutions.** This action catches those patterns before review.

---

## Quick Start

```yaml
- uses: CodeGero/ai-lint@v1
```

## What It Catches

- **Hallucinated APIs** — Imports for functions that don't exist
- **Missing error handling** — File/network I/O without `try/except`
- **Over-engineering** — Nested comprehensions, excessive imports
- **Unsafe defaults** — Common AI boilerplate that skips validation

## Why You Need This

AI assistants generate 40-60% of new code in many teams. Standard linters don't catch AI-specific failure modes. This fills that gap.

## Premium

https://kryptorious.gumroad.com/l/jbvet — Custom hallucination patterns, model-specific rules.

MIT License
