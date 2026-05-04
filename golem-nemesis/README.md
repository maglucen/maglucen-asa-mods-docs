# Golem Nemesis

![Golem Nemesis logo](./assets/logo.png)

**Golem Nemesis** makes supported anti-golem attackers deal more meaningful damage to Rock Golems and any creature that inherits from them, with direct and parent-based whitelist or blacklist overrides.

## Overview

This mod is aimed at Rock Golems and compatible child classes such as Chalk Golems and Ice Golems.

By default, the mod uses supported `DamageType` detection to decide which attackers should deal boosted anti-golem damage.

Server owners can then refine that behavior with:

- exact dino whitelist entries
- exact dino blacklist entries
- parent whitelist entries
- parent blacklist entries

Wildcard's default anti-golem damage is often effectively much lower than normal damage against Rock Golems. This mod restores qualifying attackers to a normal-damage baseline and then applies the configured percentage on top of that baseline.

If `bUseDamageTypeDetection=false`, the base allowed attackers fall back to the classic hardcoded set:

- Doedicurus
- Ankylosaurus
- Dunkleosteus

## Affected creatures

- Rock Golem
- Chalk Golem
- Ice Golem
- Other child classes inheriting from Rock Golems

## Affected attackers

- Any attacker that qualifies through the active `DamageType` detection rules
- Exact whitelist entries configured by the server owner
- Child classes matched through parent whitelist entries

When `bUseDamageTypeDetection=false`, the default hardcoded base attackers are:

- Doedicurus
- Ankylosaurus
- Dunkleosteus

## Priority rules

When multiple rules could apply to the same attacker, the mod resolves them in this order:

1. Exact blacklist
2. Exact whitelist
3. Parent blacklist
4. Parent whitelist
5. Base detection

This means:

- direct lists have priority over parent lists
- blacklist has priority over whitelist at the same level
- an exact whitelist entry can override a parent blacklist entry
- an exact blacklist entry cannot be overridden by any whitelist

## Configuration

See [Configuration](./configuration.md) for the available settings, accepted class formats, and examples.

## Changelog

Release changelogs are available on the mod's CurseForge page.

## Community

[![Join our Discord](https://img.shields.io/badge/Join%20our%20Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/6hNubWkU)

Get updates, share suggestions, and report bugs.
