# Raid Shadow Legends: Buffs and Debuffs

This document provides a Markdown-formatted list of buffs and debuffs from the game Raid: Shadow Legends, optimized for clarity and use with an LLM.

---

## Player Buffs

**Ally Protection:** The Caster Champion takes **25%** or **50%** of direct damage inflicted upon the Target Champion.
*   Self-inflicted damage and `Poison` do not trigger this effect.
*   Each Champion uses their own `DEF` value for damage mitigation.

**Block Damage:** Makes the Champion immune to all forms of damage.

**Block Debuffs:** While this buff is active, the Champion is immune to all debuffs.
*   Instant negative effects, such as `Decrease Turn Meter`, are not affected and work as normal.

**Bone Armor:** A Champion starts each Round with a number of `Bone Armor` stacks.
*   Each stack decreases the damage the recipient receives from a single hit, then disappears.
*   A Champion can have a maximum of **3** `Bone Armor` stacks at one time.

**Continuous Heal:** Heals the target Champion by **7.5%** or **15%** of their MAX HP at the beginning of their Turn.

**Counterattack:** When attacked, the Champion with this buff strikes back at their attacker using their Default Skill.
*   The counterattack deals **75%** of the normal Default Skill damage.
*   Only counterattacks once when attacked with a multi-hit Skill.
*   Does not counterattack in response to an enemy’s own counterattack.
*   Does not count as a Turn.
*   Skills that grant an Extra Turn on kill (e.g., Relickeeper's) will not grant an Extra Turn during a counterattack.

**Fervor:** Increases damage inflicted by **10%** and reduces damage received by **10%**.

**Fortify:** Reduces any enemy `Ignore DEF` effects by **15%** or **25%**.

**Increase ACC:** Increases the Champion’s ACC by **25%** or **50%**.

**Increase ATK:** Increases the Champion’s Battle ATK by **25%** or **50%**.

**Increase C.RATE:** Increases the Champion’s C.RATE by **15%** or **30%**.

**Increase C.DMG:** Increases the Champion's Critical Damage by **15%** or **30%**.

**Increase DEF:** Increases the Champion’s Battle DEF by **30%** or **60%**.

**Increase SPD:** Increases the Champion’s Battle SPD by **15%** or **30%**.

**Intercept:** Blocks attempts to apply crowd control debuffs (`Stun`, `Sleep`, `Freeze`, `Provoke`, `Fear`, `True Fear`, `Petrification`, `Sheep`), even if the debuff specifies it cannot be blocked.
*   Each stack of `Intercept` negates one attempt to apply such a debuff, after which the stack is consumed.
*   The buff has no duration and cannot be extended, reduced, or transferred.
*   **Interaction with `Block Debuffs`**:
    *   If a debuff *can* be blocked, an `Intercept` stack will not be consumed.
    *   If a debuff *cannot* be blocked, an `Intercept` stack will always be removed.
*   If a Champion with `Intercept` stacks gains another `Intercept` buff with fewer stacks, their current stack count remains unchanged.
*   If stolen, the thief gains the exact number of stacks the original Champion possessed.

**Lightning Orb (Blessing):** A stacking buff with a maximum of **3** stacks.
*   **Gaining Stacks:** Whenever an enemy receives a buff or has their Turn Meter filled, this Champion gains one `Lightning Orb` stack.
*   **Protection:** When activated, a stack randomly protects one other active buff from being removed, stolen, or transferred, then disappears.
*   **Bonus Damage:** When a Champion with **3** stacks hits an enemy, it inflicts Bonus Damage based on their MAX HP. This can occur on each hit of a Skill. After the Bonus Damage is applied, all stacks are removed.

**Magma Shield:** Reinforces the Champion's HP bar with a shield that deals damage back to the attacker.
*   Damage is first applied to the `Magma Shield` (unless the attack ignores Shields).
*   When damage is dealt to the shield, an equal amount of damage is dealt back to the attacker.
*   The buff is removed when its value reaches 0 or it expires.

**Perfect Veil:** A more powerful version of `Veil`.
*   The Champion cannot be targeted by single-target enemy skills.
*   Unlike `Veil`, this buff is **not** lost when the Champion attacks.
*   Reduces incoming AoE damage by **15%**.

**Reflect Damage:** Any Champion attacking a target with this buff sustains **15%** or **30%** of the damage they inflicted.

**Revive On Death:** If a Champion with this buff dies, they will immediately be revived with **30% HP** and **0% Turn Meter**.

**Shatter:** Increases a Champion’s `Ignore DEF` effects by **7.5%** or **15%**.

**Shield:** Reinforces the Champion's HP bar for a set number of turns.
*   Damage is first applied to the `Shield` (unless the attack ignores Shields).
*   When the buff expires or its value reaches 0, it is removed.
*   Damage dealt to a `Shield` does not count as damage to the Champion (e.g., for `Lifesteal`).

**Stone Skin:** A powerful defensive buff that provides several effects:
*   Decreases damage taken from all sources except `Bombs` and `HP Burn`.
*   Removes all debuffs except `Bombs` and `HP Burn`.
*   Grants immunity to all debuffs except `Bombs` and `HP Burn`.
*   Grants immunity to `Decrease MAX HP` and `Decrease Turn Meter` effects.
*   Provides additional `Stone Skin HP` that must be depleted before the Champion's own HP can be damaged.

**Stormcall:** A stacking buff that increases damage.
*   Each stack increases the Champion’s damage by **5%** (max 5 stacks).
*   When attacking with **5 stacks**, the Champion applies an irresistible `Stun` debuff to the target, and all `Stormcall` stacks are removed.

**Strengthen:** Decreases damage taken by **15%** or **25%**.

**Taunt:** Forces enemies to attack the Taunting Champion with their default skills.
*   Can be stolen, removed, and have its duration decreased.
*   `Petrification` on the taunting Champion will remove this buff.
*   `Provoke` has priority over `Taunt`.
*   If two Champions have `Taunt`, the enemy can target either one. If one is also under `Veil`, the unveiled Champion is targeted.

**Unkillable:** The Champion's HP cannot fall below **1** while this buff is active.

**Veil:** The Champion cannot be targeted by single-target enemy skills.
*   The buff is lost when the Champion uses a skill that deals damage. Using non-damaging skills does not remove it.
*   Reduces incoming AoE damage by **7.5%**.
*   **Exceptions:** If all living Champions on a team have `Veil` or `Perfect Veil`, or if only one Champion remains and has `Veil`, the buff is ignored and enemies can target them freely.

---

## Player Debuffs

**Berserk:** Increases damage inflicted and damage received by **50%**.

**Block Active Skills:** Prevents the Champion from using Active Skills other than their Default Skill. Skill Cooldowns refresh as normal.

**Block Buffs:** All buffs applied to the Champion are automatically blocked and have no effect.

**Block Heal:** Reduces healing received by **50%** or **100%**.

**Bomb:** When this debuff expires, the Champion suffers direct damage that ignores their `DEF`. The damage scales with a stat from the Champion who placed the debuff.

**Deathbrand:** Champions killed while under this debuff receive a `Block Revive` debuff.

**Decrease ACC:** Decreases the Champion’s Battle ACC by **25%** or **50%**.

**Decrease ATK:** Decreases the Champion’s Battle ATK by **25%** or **50%**.

**Decrease C.DMG:** Decreases the Champion's Critical Damage by **15%** or **30%**.

**Decrease C.RATE:** Decreases the Champion's Critical Rate by **15%** or **30%**.

**Decrease DEF:** Decreases the Champion’s Battle DEF by **30%** or **60%**.

**Decrease RES:** Decreases the Champion’s Battle RES by **25%** or **50%**.

**Decrease SPD:** Decreases the Champion’s Battle SPD by **15%** or **30%**.

**Enfeeble:** The Champion can only land weak hits (unless a skill states otherwise).

**Ensnare:** Reduces any Turn Meter increase effects received by **50%** or **100%**.

**Fatigue:** After using an active skill, the Champion receives a `Sleep` debuff for 1 turn. If the skill used removes debuffs, `Fatigue` is removed and `Sleep` is not applied.

**Fear:** When attempting to use a Skill, there is a **50%** chance the Skill will fail and the Champion loses their turn.

**Freeze:** The Champion is unable to act for X Turns.
*   Cooldowns are not refreshed while `Freeze` is active.
*   The Champion receives **75%** of incoming damage.

**Hex:** Champions under `Hex` take extra damage whenever their allies are attacked.
*   The extra damage ignores the `Hexed` Champion's `DEF`.
*   Takes **2%** of AoE damage and **10%** of single-target damage inflicted on their allies.
*   Does not trigger from passive damage like `Poison` or `HP Burn`.

**HP Burn:** At the start of the affected Champion’s turn, they and all their allies take damage equal to **3%** of their respective MAX HP. Only one `HP Burn` debuff can be active on a Champion at a time.

**Hunter's Gaze:** Damage dealt to a Champion under this debuff cannot be decreased, blocked, redirected, or transferred.
*   Bypasses `Unkillable`, `Block Damage`, `Shield`, `Strengthen`, `Ally Protection`, `Veil`, etc.
*   Does not bypass evasion.
*   Only applies to damage from skills, not from debuffs, passives, Masteries, or Blessings.

**Leech:** Any Champion that attacks a Champion with this debuff heals for **18%** of the damage inflicted.

**Necrosis:** A stacking debuff in certain encounters.
*   **Gaining Stacks:** When an enemy Champion dies, all surviving enemies gain one `Necrosis` stack.
*   **Damage:** At the start of their turn, a Champion takes damage equal to **5%** of their MAX HP per `Necrosis` stack.
*   **Removal:** `Stone Skin` removes all stacks. When an enemy is revived, one stack is removed from all enemies.

**Petrification:** A powerful crowd control debuff.
*   Removes all buffs and prevents the Champion from taking their next turn.
*   The Champion cannot receive buffs while petrified.
*   The Champion receives only **40%** of incoming damage.
*   Incoming damage from `Bomb` debuffs is increased by **300%**.

**Poison:** Damages the target by **2.5%** or **5%** of their MAX HP at the start of their Turn. Damage is applied to `Shields` first.

**Poison Sensitivity:** Increases damage taken from the `Poison` debuff by **25%** or **50%**.

**Provoke:** The Champion can only attack the Champion that applied the debuff, using their Default Skill.

**Seal / Master Seal:**
*   **Seal:** Blocks effects from Gear Sets and Masteries (except raw stat boosts).
*   **Master Seal:** Also blocks effects from Blessings (except raw stat boosts).
*   Does not block effects that were already active before the debuff was placed.

**Sheep:** Transforms the Champion into a sheep.
*   The Champion can only use a special "Sheep" skill.
*   The skill has a **50%** chance to remove the `Sheep` debuff after use.
*   When the debuff expires or the Sheep is defeated, the Champion returns to battle with **50% HP**.

**Sleep:** The Champion is unable to act for X Turns.
*   Cooldowns are not refreshed while `Sleep` is active.
*   Any damage received automatically removes the `Sleep` debuff.
*   Passive healing, `Continuous Heal`, and `Poison` still work.

**Smite:** When a Champion with `Smite` uses an Active Skill, they are hit by a meteorite.
*   The meteorite deals damage equal to **25%** of their MAX HP.
*   It also deals damage to all other enemies equal to **5%** of their MAX HP.
*   Only one `Smite` debuff can be active per team.

**Stun:** The Champion is unable to act for X Turns. Cooldowns are not refreshed while `Stun` is active.

**True Fear:** When attempting to use a Skill, there is a **50%** chance the Skill will fail, the Champion loses their turn, and the Skill goes on cooldown.

**Weaken:** Increases damage received by **15%** or **25%**.

---

## Special & Enemy-Specific Effects

### Amius the Lunar Archon
*   **Eclipse (Buff):** When placed, Amius transforms into his Alternate Form. When it expires, he transforms back to his Base Form.

### Hydra Clan Boss
#### Hydra Marks
*   **Mark of the Hydra:** Marks a Champion to be devoured. Cannot be removed, blocked, resisted, or have its duration changed. Ignores `Veil` and `Perfect Veil`.
*   **Digesting:** A multi-stage effect where a marked Champion is devoured. They must be freed by dealing enough damage to the digesting Hydra Head before a 5-turn countdown expires, or they are permanently removed from battle.

#### Hydra Buffs
*   **Life Barrier:** An additional HP bar that must be depleted first. Cannot be removed, stolen, or manipulated.
*   **Poison Cloud:** Blocks damage from `Poison` debuffs. Cannot be manipulated.
*   **Serpent’s Will:** Reduces all damage a newly grown Head takes by **75%** until its first turn. Cannot be manipulated.
*   **Vengeance:** Increases the Head of Wrath's damage by **300%** after it receives 15 hits. Cannot be manipulated.

#### Hydra Debuffs
*   **Decapitated:** Increases damage taken by a severed Head by **200%**. Active as long as the Head is dead. Cannot be manipulated.
*   **Pain Link:** The affected Champion receives **15%** of all damage received by the Head of Suffering. Can be blocked or removed.

### Minotaur's Labyrinth
*   **Rage (Buff):** Increases the Minotaur's damage by **400%**.
*   **Dazed (Debuff):** Increases damage the Minotaur receives by **200%**. Duration cannot be increased.
*   **Hex (Interaction):** The Minotaur’s `Tremor Stomp` skill deals double damage to Champions with `Hex`.

### Other Enemy Buffs
*   **Eternal Rage (Iragoth Buff):** Increases Iragoth’s SPD and causes his attacks to ignore `Unkillable`, `Block Damage`, `Shield` buffs, and **50%** of the target's DEF.