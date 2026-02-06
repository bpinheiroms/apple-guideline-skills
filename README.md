# Apple App Store Review Guidelines - Claude Code Skill

A comprehensive reference of the [Apple App Store Review Guidelines](https://developer.apple.com/app-store/review/guidelines/) packaged as a Claude Code skill. Invoke it when building features, screens, or functionality for iOS apps to ensure compliance and avoid rejections.

## Guidelines

The full guidelines are available in English:

- [APPLE_GUIDELINES.md](./APPLE_GUIDELINES.md)

## What's Covered

| Section | Topics |
|---------|--------|
| **1. Safety** | Objectionable content, UGC, Kids Category, physical harm, data security |
| **2. Performance** | App completeness, beta testing, metadata, hardware compatibility, software requirements |
| **3. Business** | In-App Purchase, subscriptions, payment methods, cryptocurrencies, business models |
| **4. Design** | Copies, minimum functionality, spam, extensions, login services, Apple Pay |
| **5. Legal** | Privacy, data collection, health research, kids privacy, IP, gambling, VPN, MDM |

## Usage as a Claude Code Skill

To use this as a [Claude Code](https://docs.anthropic.com/en/docs/claude-code) skill, copy the contents of `APPLE_GUIDELINES.md` into a skill file at:

```
~/.claude/skills/apple-guidelines/SKILL.md
```

With the following frontmatter:

```yaml
---
name: apple-guidelines
description: Apple App Store Review Guidelines. Invoke when creating features, screens, or functionality for iOS apps to ensure compliance and avoid rejections.
user-invocable: true
---
```

Then invoke it with `/apple-guidelines` in Claude Code before implementing any iOS feature.

## Verification Checklist

The guidelines include a quick checklist covering: UGC, Privacy, Payments, Kids, Login, Metadata, Content, Performance, Design, Location, Health, Ads, Push Notifications, Account Deletion, and Intellectual Property.
