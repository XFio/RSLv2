# Raid Shadow Legends Calculation Formulas & Speed Tuning Guide

## Core Combat Formulas

### Damage Calculation
```
Base Damage = ATK * Skill Multiplier * (1 + Critical Damage%) * Enemy DEF Mitigation

DEF Mitigation = DEF / (DEF + 60 * Attacker Level)

Critical Damage% = Base Crit Damage + Gear Crit Damage (when crit occurs)
```

### Effective HP Calculation
```
Effective HP = HP * (1 + (DEF / (DEF + 60 * Level)))

Shield Value = Champion HP * Shield Multiplier * (1 + Shield Set Bonus)
```

### Accuracy vs Resistance
```
Chance to Land Debuff = Skill Chance * (1 - MAX(0, Target Resistance - Attacker Accuracy) / 100)

Minimum 3% chance to resist (cannot be reduced below this)
Maximum 97% chance to land (cannot exceed this)
```

### Turn Meter and Speed
```
Turn Meter Fill Rate = Speed * Speed Modifier
Base Speed Modifier = 1.0
Increase Speed Buff = +30% (1.3x modifier)
Decrease Speed Debuff = -30% (0.7x modifier)

Effective Speed = Base Speed * (1 + Speed Sets/Bonuses) * Speed Aura * Speed Buff/Debuff
```

## Clan Boss Speed Tuning

### Speed Requirements by Difficulty

| Difficulty | CB Speed | 1:1 Ratio Range | 2:1 Ratio Range | 3:1 Ratio Range |
|------------|----------|-----------------|-----------------|-----------------|
| Brutal     | 160      | 161-170        | 241-255        | 361-382        |
| Nightmare  | 170      | 171-189        | 256-284        | 384-426        |
| Ultra NM   | 190      | 191-209        | 286-314        | 429-471        |

### Speed Tuning Formulas

#### 1:1 Ratio (Standard)
```
Minimum Speed = (CB Speed + 1)
Maximum Speed = Floor(CB Speed * 1.3) - 1

Example for UNM:
Min: 191
Max: Floor(190 * 1.3) - 1 = 246
```

#### 2:1 Ratio (Speed Teams)
```
Minimum Speed = Floor(CB Speed * 1.5) + 1
Maximum Speed = Floor(CB Speed * 1.7)

Exact 2:1 Speed = CB Speed * 1.5
```

#### Speed Calculator with Turn Meter Boost
```
Effective Speed = Actual Speed + (Turn Meter Boost% * CB Speed)

For 30% TM Boost:
Required Speed = Target Speed - (0.3 * CB Speed)
```

### Unkillable Team Speed Requirements

#### Budget Unkillable (Maneater + Painkeeper)
```
Maneater: 241-245 speed (3 turn cooldown)
Painkeeper: 221-225 speed (3 turn cooldown)
DPS Champions: 177-180 speed
Slow Champion: 114-119 speed
```

#### Tower (Skullcrusher + Roshcard)
```
Roshcard: 248-252 speed
Skullcrusher: 173-177 speed
DPS: 171-172 speed
```

## Arena Speed Calculations

### Turn Order Determination
```
Turn Order Priority = Speed * (1 + Random(0 to 0.05))

This means a 5% speed variation, so:
To guarantee going first: Your Speed > Enemy Speed * 1.05
```

### Speed Lead Calculations
```
Total Speed = Base Speed * (1 + Gear%) * (1 + Speed Lead%)

Example:
Arbiter (110 base) with 200% gear speed and 30% lead:
Total = 110 * (1 + 2.0) * (1 + 0.3) = 429 speed
```

### Cut-in Prevention
```
To prevent cut-in, second champion needs:
Speed2 >= Speed1 * 0.7

Example:
If Speed Lead has 300 speed, nuker needs at least 210 speed
```

## Dungeon Mechanics

### Spider Den HP Scaling
```
Spiderling HP by Stage:
Stage 20: ~17,000 HP
Stage 25: ~25,000 HP

HP Burn Damage = 3% of MAX HP per tick
AOE HP Burn effectiveness threshold = Can kill spiderlings in 2 ticks
```

### Fire Knight Shield
```
Shield Hit Requirements:
Stage 20: 10 hits
Stage 25: 12 hits

Multi-hit Efficiency = Number of Hits * Speed
Optimal: 3+ hits per skill with 200+ speed
```

### Dragon Poison Damage
```
Poison Tick Damage = 2.5% or 5% of MAX HP
Dragon 25 HP = ~4,000,000
5% Poison = 200,000 per tick
2.5% Poison = 100,000 per tick

Poison Cap = 10 debuffs maximum
Max Poison Damage = 10 * 5% = 50% MAX HP per turn
```

## Resource Efficiency Calculations

### Energy Efficiency
```
Energy per Shard (Mystery):
Campaign 12-3 Brutal: ~1.5 energy per shard
Campaign 12-6 Brutal: ~1.3 energy per shard

Energy per XP:
12-3 Brutal Solo: ~110 XP per energy
12-6 Brutal Solo: ~105 XP per energy

Silver per Energy:
Spider 20: ~3,000 silver per energy
Spider 25: ~4,500 silver per energy
```

### Champion Investment ROI
```
6-Star Cost:
5x 5-star food = 25x 4-star = 100x 3-star
Energy Cost: ~2,000 energy
Silver Cost: ~2,000,000

Book Value Calculation:
Damage Increase per Book = (New Multiplier - Old Multiplier) / Old Multiplier
Cooldown Reduction Value = Turns Saved / Original Cooldown

ROI Score = (Performance Increase % * Content Weight) / Resource Cost
```

### Gear Efficiency Score
```
Gear Score = Main Stat Value + (Substat Values * Roll Quality)

Roll Quality:
- Flat stats: 50-100% of max
- Percentage stats: 5-8% per roll
- Speed: 4-6 per roll

Efficiency % = Actual Rolls / Maximum Possible Rolls * 100

Keep Threshold:
- Early Game: 60% efficiency
- Mid Game: 70% efficiency  
- Late Game: 80% efficiency
- End Game: 85%+ efficiency
```

## Artifact Optimization

### Stat Priority Values
```
1 Speed = ~2% Crit Rate = ~4% Crit Damage
1% HP = ~1% DEF (for survivability)
1% ATK = ~2% Crit Damage (for consistent damage)

Accuracy Requirements:
- Dungeon 20: 200-220
- Dungeon 25: 250-280
- Doom Tower Normal: 250+
- Doom Tower Hard: 350+
- Hydra: 400+
```

### Set Bonus Efficiency
```
Offensive Sets (by priority):
1. Savage (Ignore 25% DEF) = ~30% damage increase
2. Lethal (10% Crit Rate, 15% on first hit) = ~20% damage increase
3. Cruel (15% ATK, 5% Ignore DEF) = ~18% damage increase

Defensive Sets:
1. Stoneskin (1 hit block) = Invaluable in Arena
2. Regeneration (15% heal) = ~30% effective HP increase
3. Stalwart (-30% damage from AOE) = Situational 30% mitigation

Speed Sets:
Speed Set (12% speed) on fast champion (200 base):
= 24 speed = Often worth 2-3 substat rolls
```

## Masteries Optimization

### Damage Masteries (T6)
```
Warmaster: 60% chance for 10% MAX HP (capped at 100k on bosses)
Giant Slayer: 30% chance per hit for 5% MAX HP (better for 3+ hit A1)
Helmsmasher: 50% chance to ignore 25% DEF

Damage Comparison vs Clan Boss:
Warmaster = 60,000 average per proc
Giant Slayer (3 hits) = 90,000 average per turn
```

### Support Masteries Value
```
Lore of Steel (Set bonus +15%):
Speed Set: 12% -> 13.8% = +1.8% speed
Divine Speed: 15% -> 17.25% = +2.25% speed

Master Hexer (Debuff extension):
Value = (Extra Turn Duration / Original Duration) * Debuff Value
Example: Extending 2-turn decrease DEF to 3 turns = 50% value increase
```

## Special Mechanics

### Decrease Turn Meter
```
Actual TM Reduction = Base Reduction * (1 - Target Resistance Effect)
Cannot reduce below 0%
Cannot reduce champions with Increase Turn Meter buff by some abilities
```

### Buff/Debuff Interactions
```
Buff Override Priority:
- Higher value buffs override lower (60% DEF > 30% DEF)
- Same buffs don't stack, refresh duration
- Block Debuffs prevents all debuff application
- Immunity removes existing debuffs when applied

Debuff Limits:
- Maximum 10 debuffs per champion
- Newest debuff replaces oldest when at cap
```

### Passive Skill Interactions
```
Passive Priority Order:
1. Reaction to direct damage (Counterattack, Reflect)
2. Reaction to debuffs (Cleanse, Transfer)
3. Turn-based effects (Healing, TM boost)
4. Conditional triggers (Low HP, Ally death)

Multiple Passive Resolution:
- Resolved in speed order when simultaneous
- Each passive completes before next triggers
```

## Advanced Speed Tuning Scenarios

### Myth-Fu Composition
```
Mythical Champion Requirements:
- Demytha: 280-294 speed (Myth-Fu)
- Fushan: 251-265 speed
- Seeker: 182-186 speed
- DPS 1: 177-181 speed
- DPS 2: 172-176 speed

Turn Order Sequence:
1. Demytha extends buffs
2. Fushan places block debuffs
3. Seeker TM boost
4. DPS champions
5. Repeat maintaining buff coverage
```

### Batman Forever
```
Requirements:
- Tower: 248-249 speed
- Batman (Seeker): 246-247 speed
- DPS: 175-178 speed

This maintains permanent unkillable with 2 champions
```

## Optimization Algorithms

### Team Power Calculation
```
Team Power = Σ(Champion Power * Role Multiplier * Synergy Bonus)

Role Multipliers:
- Damage Dealer: 1.2
- Support/Healer: 1.0
- Tank: 0.9
- Debuffer: 1.1

Synergy Bonus:
- Matching Affinity: +5%
- Complementary Roles: +10%
- Aura Leader: +15%
```

### Investment Priority Score
```
Priority = (Content Importance * Performance Gap * Champion Versatility) / Resource Cost

Where:
- Content Importance: User-defined weight (0-10)
- Performance Gap: Current vs Potential (0-100%)
- Champion Versatility: Number of content areas used (1-10)
- Resource Cost: Books + Potions + Silver (normalized)
```

## Usage Notes

1. **Always verify speeds in-game** - Displayed speed may differ from effective speed
2. **Account for latency** in speed calculations (especially for unkillable teams)
3. **Test compositions** before committing resources
4. **RNG affects outcomes** - Calculate probabilities, not certainties
5. **Meta changes** may affect optimal calculations - stay updated

These formulas form the mathematical foundation for all strategic decisions in RSL. When combined with champion-specific data and player constraints, they enable optimal team building and resource allocation.