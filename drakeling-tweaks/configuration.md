# Drakeling Tweaks Configuration

Add the following section to `GameUserSettings.ini`.

```ini
[DrakelingTweaks]
NonWildKillXPPercent=100
BreathCooldownMultiplierPercent=100
BiomeBoostCooldownMultiplierPercent=100
GiftOfFortuneCooldownMultiplierPercent=100
ShowBuffInfo=False
DisableHoardChests=False
```

## Settings

### `NonWildKillXPPercent`

Controls how much stored XP is restored from tamed and unclaimed creature kill XP.

- Values above `100` increase the restored stored XP above the current default amount.
- `100` = current default restored XP.
- `50` = half of the current restored XP.
- `1` = 1% of the current restored XP.
- `0` = current/default Wildcard value.
- Values below `0` are capped to `0`.

### `BreathCooldownMultiplierPercent`

Controls Breath cooldown as a percentage of its current default cooldown.

### `BiomeBoostCooldownMultiplierPercent`

Controls Biome Boost cooldown as a percentage of its current default cooldown.

### `GiftOfFortuneCooldownMultiplierPercent`

Controls Gift of Fortune cooldown as a percentage of its current default cooldown.

## Cooldown notes

- Values above `100` increase the cooldown duration.
- `200` = twice the current default cooldown.
- `100` = current default cooldown.
- `50` = half of the current cooldown.
- `1` = 1% of the current cooldown.
- `0` is not recommended unless you explicitly want effectively no cooldown.
- Values below `0` are capped to `0`.

### `ShowBuffInfo`

When set to `True`, shows a 5-second info display whenever stored XP is earned from a tamed or unclaimed creature kill.

### `DisableHoardChests`

When set to `True`, no Hoard Chest will be granted when stored XP is awarded.

## Important update note

The config category name changed from `[DrakelingTamedXPMultiplier]` to `[DrakelingTweaks]`.

If you are updating from an older version, move your settings to the new category. Settings left under the old category name are no longer used.
