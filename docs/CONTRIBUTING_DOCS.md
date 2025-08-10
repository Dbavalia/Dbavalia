# Contributing to Documentation

Scope
- This guide explains how to document public APIs, functions, classes, and components.

General rules
- Document only public, supported surfaces. Mark experimental with clear labels.
- Keep examples runnable and minimal.
- Document error conditions and edge cases.
- Update docs in the same change as code when behavior changes.

Style
- Use clear, active voice. Prefer short sentences.
- Use language-native doc comments plus dedicated markdown pages when needed.
- Provide both a quick-start example and an advanced usage example for complex APIs.

Structure for each API item
- Summary
- Detailed behavior
- Parameters and types
- Returns
- Errors
- Examples
- Since / Deprecated

Verification checklist for PRs
- [ ] New/changed APIs are documented
- [ ] Examples compile/run
- [ ] Links updated (TOC, cross-references)
- [ ] Breaking changes called out