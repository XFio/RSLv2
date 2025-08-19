# Artifact Optimization & Evaluation Guide

## Artifact Basics

### Artifact Slots and Main Stats

| Slot | Possible Main Stats | Priority Stats by Role |
|------|-------------------|----------------------|
| **Weapon** | ATK (flat) only | N/A - Always flat ATK |
| **Helmet** | HP (flat) only | N/A - Always flat HP |
| **Shield** | DEF (flat) only | N/A - Always flat DEF |
| **Gloves** | HP%, DEF%, ATK%, C.RATE, C.DMG | Nuker: C.RATE/C.DMG<br>Support: HP%/DEF% |
| **Chest** | HP%, DEF%, ATK%, ACC, RES | Nuker: ATK%<br>Support: HP%/DEF%<br>Debuffer: ACC |
| **Boots** | HP%, DEF%, ATK%, SPD | 95% of champions: SPD<br>Special cases: ATK%/DEF% |

### Substat Ranges and Roll Values

| Substat Type | Min Roll | Max Roll | God Roll (4x Max) |
|--------------|----------|----------|-------------------|
| **Speed** | 4 | 6 | 24 |
| **ATK%** | 4% | 8% | 32% |
| **HP%** | 4% | 8% | 32% |
| **DEF%** | 4% | 8% | 32% |
| **C.RATE** | 4% | 6% | 24% |
| **C.DMG** | 4% | 7% | 28% |
| **ACC** | 4 | 8 | 32 |
| **RES** | 4 | 8 | 32 |

### Flat Stats (Generally Avoid)
- HP: 100-375 per roll
- ATK: 10-25 per roll  
- DEF: 10-25 per roll

## Artifact Quality Evaluation

### Efficiency Calculation
```
Efficiency % = (Actual Substat Value / Maximum Possible Value) × 100

Example 6* Legendary Boots with Speed main:
- Main stat: 45 Speed (fixed)
- Substats: Speed cannot appear as substat
- 4 substats, 5 rolls total (1 at +4, +8, +12, +16, +20)

If substats are:
- C.RATE: 18% (3 rolls × 6% max = perfect)
- ATK%: 16% (2 rolls × 8% max = perfect)
- HP%: 8% (1 roll × 8% max = perfect)
- ACC: 8 (1 roll × 8 max = perfect)

Efficiency = 100% (perfect piece)
```

### Keep/Sell Decision Framework

#### Early Game (Account Level 1-40)
**Keep if:**
- 4* or higher with speed substat
- 5* or higher with correct main stat
- Any % main stat boots/chest/gloves
- Efficiency > 60%

**Sell if:**
- Flat stat main on gloves/chest/boots
- Wrong set for your needs
- No speed and no useful substats

#### Mid Game (Account Level 40-50)
**Keep if:**
- 5* or higher only
- Speed substat OR double/triple rolls in needed stat
- Correct main stat for role
- Efficiency > 70%

**Sell if:**
- 4* gear (except speed boots)
- Split substats (both offensive and defensive)
- Low efficiency flat stat pieces

#### Late Game (Account Level 50-60)
**Keep if:**
- 6* primarily (exceptional 5* pieces)
- High speed rolls (15+ speed)
- Triple/quad rolls in key stats
- Efficiency > 80%

**Sell if:**
- Most 5* gear
- Low roll efficiency
- Mismatched substats for set type

#### End Game (Account Level 60+)
**Keep if:**
- 6* only (rare god-tier 5* exceptions)
- 18+ speed OR triple+ rolls
- Efficiency > 85%
- Perfect set/substat combinations

## Set Optimization Priority

### Universal Top Tier Sets

1. **Speed (12% SPD)** - Best for 90% of champions
2. **Perception (40 ACC, 5% SPD)** - Speed + accuracy combo
3. **Savage (Ignore 25% DEF, 10% on bosses)** - Best damage set
4. **Stoneskin (Block 1 hit)** - Arena defense meta

### Role-Specific Set Priorities

#### Nukers
1. Savage + Cruel/Lethal
2. Lethal + Instinct  
3. Destroy + Cruel
4. Fatal + Cruel
5. Offense + Offense + Offense

#### Support/Healers
1. Speed + Speed + Perception/Immortal
2. Relentless + Speed
3. Regeneration + Immortal
4. Shield + Speed

#### Debuffers
1. Speed + Perception + Perception
2. Accuracy + Speed + Perception
3. Speed + Speed + Accuracy

#### Tanks
1. Stoneskin + Perception
2. Stalwart + Immortal
3. Shield + Speed
4. Regeneration + Immortal

#### Clan Boss Specific
1. Lifesteal + Speed (early/mid game)
2. Stalwart + Speed/Perception (late game)
3. Toxic + Speed (poisoners)
4. Reflex + Speed (cooldown dependent)

## Advanced Optimization Strategies

### Speed Tuning Priority
```
Arena Speed Order Requirements:
1. Speed Lead: Maximum possible speed
2. Decrease DEF: Lead Speed × 0.95
3. Nuker 1: Lead Speed × 0.75
4. Nuker 2: Lead Speed × 0.70

Example with 300 speed lead:
- Lead: 300
- Decrease DEF: 285
- Nuker 1: 225
- Nuker 2: 210
```

### Broken Set Optimization

**When to use broken sets:**
- Speed requirements > set bonuses
- Quad roll pieces too good to ignore
- Specific stat thresholds needed

**Broken Set Value Calculation:**
```
Compare: Set Bonus vs Lost Substats

Speed Set = 12% speed
On 250 base speed = 30 speed
Equivalent to 5-7 speed rolls

If broken pieces give 8+ more speed in substats = worth it
```

### Artifact Upgrade Strategy

#### Efficient Silver Usage
1. **Preview at +4** - See first substat/roll
2. **Evaluate at +8** - 2 rolls visible
3. **Commit at +12** - 3 rolls, decide to continue
4. **Complete at +16** - Only for great pieces

#### Upgrade Priority Order
1. Boots with speed main stat
2. Chest/Gloves with correct % main
3. Speed set pieces with speed substats
4. Perception pieces with speed/acc
5. Damage pieces with crit substats
6. Everything else

### Faction Guardian Optimization

**Ring Priority:**
1. ATK/DEF/HP rings by champion role
2. Keep 4-5 of each for different builds

**Amulet Priority:**
1. C.DMG for nukers (very rare)
2. DEF/HP for supports
3. Faction-specific for Faction Wars

**Banner Priority:**
1. Speed substats
2. Accuracy (for debuffers)
3. Resistance (for cleansers)

## Content-Specific Gearing

### Clan Boss Requirements

| Difficulty | DEF | HP | Speed | Accuracy |
|------------|-----|-----|-------|----------|
| Brutal | 2500+ | 25k+ | 171-189 | 150+ |
| Nightmare | 3000+ | 30k+ | 171-189 | 180+ |
| UNM | 3500+ | 35k+ | 191-209 | 220+ |

### Arena Requirements

| Tier | Speed Lead | Nuker C.Rate | Nuker C.DMG | Accuracy |
|------|------------|--------------|-------------|----------|
| Bronze-Silver | 200+ | 70%+ | 150%+ | 150+ |
| Gold I-IV | 250+ | 85%+ | 200%+ | 200+ |
| Platinum | 330+ | 100% | 250%+ | 250+ |

### Dungeon Requirements

| Dungeon | Stage 20 ACC | Stage 25 ACC | Special Requirements |
|---------|--------------|--------------|---------------------|
| Dragon | 200 | 250 | Poison/HP Burn helpful |
| Spider | 200 | 250 | AOE HP Burn crucial |
| Fire Knight | 200 | 250 | Multi-hit essential |
| Ice Golem | 200 | 250 | Block revive needed |

### Doom Tower Requirements

| Content | Normal ACC | Hard ACC | Speed | Other |
|---------|------------|----------|-------|-------|
| Waves | 250+ | 350+ | 200+ | High damage |
| Bosses | 250+ | 350+ | 200+ | Specific counters |
| Secret Rooms | Varies | Varies | Varies | Faction specific |

## Gear Farming Efficiency

### Where to Farm

| Priority | Location | Target | Energy Efficiency |
|----------|----------|--------|-------------------|
| 1 | Dragon 20/24/25 | Speed, Lifesteal, Accuracy | Highest |
| 2 | Spider 20/24/25 | Accessories, Silver | High |
| 3 | Fire Knight 20/24/25 | Savage, Stun, Immunity | Medium |
| 4 | Ice Golem 20/24/25 | Reflex, Regeneration | Low |

### Farming Strategy

#### Campaign Farming (Speed/Lifesteal)
- Stage 6 of each area
- 5* common/uncommon gear
- Most energy efficient for specific pieces
- Good for early game speed boots

#### Dungeon Farming Priorities
1. **Dragon**: Until core teams built
2. **Spider**: For accessories and silver
3. **Fire Knight**: For Savage sets (end game)
4. **Ice Golem**: Only during tournaments

### Event Efficiency

**Artifact Enhancement Events:**
- Save 15M+ silver
- Pre-farm artifacts to upgrade
- Focus on guaranteed upgrades (boots, chest)

**Dungeon Diver Events:**
- 4000-7000 energy typically needed
- Best value: Dragon during 2x speed
- Stack with champion training when possible

## Optimization Tools & Tracking

### Gear Score Formula
```
Gear Score = Main Stat Weight + Σ(Substat Values × Role Weights)

Weights by Role:
- Nuker: Speed=3, C.Rate=3, C.DMG=4, ATK%=2
- Support: Speed=4, HP%=2, DEF%=2, RES=1
- Debuffer: Speed=3, ACC=3, HP%=2, DEF%=1
```

### Minimum Viable Stats by Progression

| Role | Early Game | Mid Game | Late Game | End Game |
|------|------------|----------|-----------|----------|
| **Nuker** |
| Speed | 150+ | 170+ | 190+ | 200+ |
| C.Rate | 70%+ | 85%+ | 95%+ | 100% |
| C.DMG | 120%+ | 180%+ | 220%+ | 250%+ |
| **Support** |
| Speed | 170+ | 200+ | 230+ | 250+ |
| HP | 30k+ | 45k+ | 60k+ | 80k+ |
| DEF | 2k+ | 2.5k+ | 3k+ | 3.5k+ |
| **Debuffer** |
| Speed | 170+ | 200+ | 220+ | 240+ |
| ACC | 150+ | 200+ | 250+ | 350+ |

## Common Mistakes to Avoid

1. **Overvaluing Set Bonuses** - Stats > Sets in most cases
2. **Ignoring Speed** - Speed is king in 90% of content
3. **Hoarding Bad Gear** - Sell aggressively, vault space is limited
4. **Upgrading Everything** - Be selective, silver is precious
5. **Neglecting Accessories** - Often bigger upgrades than armor
6. **Flat Stats on Bottom Row** - Almost never worth it
7. **Mismatched Substats** - Don't put ATK% on support champions
8. **Ignoring Glyphs** - Can add 20+ speed to a build
9. **Not Farming Enough** - Gear is 80% of champion power
10. **Perfect or Nothing** - Good enough gear > waiting for perfect

## Quick Reference: Stats per Content

### Universal Minimums
- **Speed**: 170+ for any content
- **Accuracy**: Match the content requirement
- **Crit Rate**: 70%+ for any damage dealer
- **HP**: 30k+ for survivability
- **Defense**: 2k+ minimum for non-glass cannons

### Content Specific Targets
- **Clan Boss**: Max DEF/HP, speed tuned precisely
- **Arena**: Max speed on lead, max damage on nukers
- **Dungeons**: Balance of speed, accuracy, and damage
- **Doom Tower**: High accuracy (350+) and survivability
- **Hydra**: Extreme stats - 400+ accuracy, high resistance

Remember: These are guidelines. Your specific team composition and strategy may require different optimization priorities.