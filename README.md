# mobilewright-skill

A skill that teaches AI agents how to use [mobilewright](https://github.com/niceguydave/mobilewright) for mobile device automation, testing, and development verification.

## Installation

Copy the skill into your Claude Code skills directory:

```bash
cp -r skills/mobilewright ~/.claude/skills/mobilewright
```

Or reference it directly in your project's `.claude/` directory.

## What It Does

When activated, this skill teaches the agent to:

- Inspect the device's UI tree before writing any locators
- Choose the most stable locator strategy (testId > role > label > text)
- Write mobile tests using `@mobilewright/test` (Playwright Test fixtures)
- Write standalone automation scripts using the `mobilewright` API
- Verify UI implementation during mobile app development
- Avoid common pitfalls (raw coordinates, hardcoded timeouts, brittle locators)

## Supported Platforms

- iOS (simulators and real devices)
- Android (emulators and real devices)
