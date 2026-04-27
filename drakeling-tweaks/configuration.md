# Drakeling Tweaks Configuration

Add the following section to `GameUserSettings.ini`.

```ini
[DrakelingTweaks]
NonWildKillXPPercent=100
BreathCooldownMultiplierPercent=100
BiomeBoostCooldownMultiplierPercent=100
GiftOfFortuneCooldownMultiplierPercent=100
ShowXPInfo=true
```

## Settings

### `NonWildKillXPPercent`

Controls the percentage of stored XP granted from tamed and unclaimed creature kills.

- `100` = default/full value.
- `0` = disabled.
- Values above `100` increase the amount.

### `BreathCooldownMultiplierPercent`

Controls the Breath cooldown percentage.

- `100` = default cooldown.
- `50` = half cooldown.
- `200` = double cooldown.

### `BiomeBoostCooldownMultiplierPercent`

Controls the Biome Boost cooldown percentage.

- `100` = default cooldown.
- `50` = half cooldown.
- `200` = double cooldown.

### `GiftOfFortuneCooldownMultiplierPercent`

Controls the Gift of Fortune cooldown percentage.

- `100` = default cooldown.
- `50` = half cooldown.
- `200` = double cooldown.

### `ShowXPInfo`

Controls whether XP info is displayed when stored XP is granted.

- `true` = show XP info.
- `false` = hide XP info.

## Important update note

The config category name changed from `[DrakelingTamedXPMultiplier]` to `[DrakelingTweaks]`.

If you are updating from an older version, move your settings to the new category. Settings left under the old category name are no longer used.
