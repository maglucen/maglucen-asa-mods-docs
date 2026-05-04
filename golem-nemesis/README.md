# Golem Nemesis

![Golem Nemesis logo](./assets/logo.png)

**Golem Nemesis** makes supported anti-golem attackers deal more meaningful damage to Rock Golems and any creature that inherits from them, with direct and parent-based whitelist or blacklist overrides.

## Overview

This mod is aimed at Rock Golems and compatible child classes such as Chalk Golems and Ice Golems.

By default, the mod uses supported `DamageType` detection to decide which attackers should deal boosted anti-golem damage. Server owners can override that behavior with exact and parent-based white or blacklists.

By default, Rock Golems heavily reduce incoming damage from most sources. This mod restores qualifying attackers to a normal-damage baseline against Rock Golems and then applies the configured percentage on top of that baseline.

If `bUseDamageTypeDetection=false`, the base allowed attackers fall back to the classic hardcoded set: Doedicurus, Ankylosaurus, and Dunkleosteus. Whitelist and blacklist rules still apply on top of that base set.

## Affected creatures

- Rock Golem
- Chalk Golem
- Ice Golem
- Other child classes inheriting from Rock Golems

## Affected attackers

- Any attacker that qualifies through the active `DamageType` detection rules
- Exact whitelist entries configured by the server owner
- Child classes matched through parent whitelist entries

## Priority rules

Direct rules override parent rules, and blacklist rules override whitelist rules at the same level.

## Configuration

See [Configuration](./configuration.md) for the full priority order, available settings, accepted class formats, and examples.

## Changelog

Release changelogs are available on [CurseForge](https://www.curseforge.com/ark-survival-ascended/mods/golem-nemesis).

## Community

[![Join our Discord](https://img.shields.io/badge/Join%20our%20Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/6hNubWkU)

Get updates, share suggestions, and report bugs.
