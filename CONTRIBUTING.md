# Contributing to Hermes IDE

Thank you for your interest in contributing. Hermes IDE is a focused, minimal
AI-native terminal and IDE. We welcome contributions that align with our vision.

## Before You Start

**Read first:**
- [Design Principles](https://github.com/hermes-hq/hermes-ide/blob/main/DESIGN_PRINCIPLES.md)

**The #1 rule:** Open an issue or discussion BEFORE writing code for any new
feature. We will tell you upfront if it fits the project's scope. Unsolicited
feature PRs that were not discussed first will be closed.

Bug fixes and documentation improvements do not require prior discussion.

## Contributor License Agreement (CLA)

All contributors must sign our CLA before their first PR can be merged. This is
automated — you will be prompted on your first pull request. The CLA grants the
project the right to use your contributions under any license terms. You retain
your own copyright.

## What We Accept

- Bug fixes (always welcome)
- Performance improvements
- Documentation improvements
- Accessibility improvements
- Features that are on the roadmap or have been approved in a discussion

## What We Do Not Accept

- Features that expand scope beyond our design principles
- Large refactors without prior discussion
- Changes that add significant new dependencies
- Anything that can be provided by a plugin or extension instead of core
- PRs without tests for non-trivial changes

## Development Setup

```bash
# Clone the repo
git clone https://github.com/hermes-hq/hermes-ide.git
cd hermes-ide

# Install dependencies
npm install

# Run the dev server (frontend only)
npm run dev

# Run the full Tauri app in dev mode
npm run tauri dev

# Run tests
npm run test

# Type check
npx tsc --noEmit
```

### Prerequisites

- Node.js 20+
- Rust (stable)
- Platform-specific Tauri dependencies: https://v2.tauri.app/start/prerequisites/

## Submitting a Pull Request

1. Fork the repository
2. Create a branch from `main` (`feat/`, `fix/`, `docs/` prefix)
3. Make your changes with clear, atomic commits
4. Ensure tests pass: `npm run test`
5. Ensure type checking passes: `npx tsc --noEmit`
6. Submit your PR using the PR template

## PR Review Process

- All PRs require at least one maintainer approval
- Feature PRs require owner final approval
- Bug fix PRs can be merged by any maintainer
- Expect initial feedback within 7 days
- PRs with no response for 14 days will be closed

## Code Style

- TypeScript strict mode
- CSS Modules (no CSS-in-JS)
- Rust 2021 edition
- No unnecessary dependencies — justify any new dependency in your PR

## Questions?

Use [GitHub Discussions](https://github.com/hermes-hq/hermes-ide/discussions) for questions, ideas, and general conversation.
