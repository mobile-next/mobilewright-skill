# mobilewright-skill

A skill that teaches AI agents how to use [mobilewright](https://github.com/mobile-next/mobilewright) for mobile device automation, testing, and development verification.

## Installation

**Option 1** — download directly:

```bash
mkdir -p ~/.claude/skills/mobilewright
curl -fsSL https://raw.githubusercontent.com/mobile-next/mobilewright-skill/main/skills/mobilewright/SKILL.md \
  -o ~/.claude/skills/mobilewright/SKILL.md
```

**Option 2** — clone and copy:

```bash
git clone https://github.com/mobile-next/mobilewright-skill.git
cp -r mobilewright-skill/skills/mobilewright ~/.claude/skills/mobilewright
```

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
