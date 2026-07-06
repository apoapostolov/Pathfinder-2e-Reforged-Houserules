<!-- markdownlint-disable MD001 MD013 MD025 -->

# Drugs

In back alleys, hidden stillrooms, ruined towers, and perfumed noble salons,
dangerous substances change hands for coin, favors, and power. Some are cheap
stimulants peddled to laborers and cutthroats. Others are dream-drugs brewed
from moonlit flowers, monster venom, or stolen occult secrets. This subsystem
covers the full life of such drugs: finding strange source material, refining
it into something usable, cooking a stable formula, and then deciding whether
to keep the recipe close or build a trade around it.

The rules below are written for fantasy crime stories and occult chemistry.
They are meant to feel methodical and material, but still belong to Pathfinder:
the process is dangerous, profitable, and tempting, and the finished product is
handled using familiar PF2e item and affliction rules.

## The Loop

1. **Collect** unusual biological, botanical, mineral, or magical samples.
2. **Extract** a usable component formula from a sample.
3. **Refine** that formula to improve purity, potency, or compatibility.
4. **Cook** a complete drug formula from a base, enhancer, and solution.
5. **Craft Drugs** for personal use or **Mass Produce** for distribution.
6. **Establish a Route**, **Move Product**, and **Lie Low** when Heat rises.

## Drug Formula Anatomy

Every finished drug should end as a normal PF2e drug item. In play, drugs work
less like simple buff items and more like dangerous poisons that begin with a
tempting high before turning against the user.

Each finished formula needs the following elements.

- **Name and Level** The item's title and item level.
- **Traits** Usually alchemical, consumable, drug, ingested, poison, plus any
  fitting descriptor traits such as magical or inhaled.
- **Price** Use the normal price for a consumable of its level as a baseline,
  then adjust for rarity, social demand, and supply scarcity.
- **Usage and Activate** Most drugs use `held in 1 hand`, Bulk `L`, and
  `Activate [one-action] Interact`.
- **Saving Throw** A Fortitude save based on the drug's level. Use the standard
  DC for that level as a baseline, adjusting by at most 2 for especially crude
  or unusually clean formulas.
- **Onset** Omit if immediate. Official drugs often use no onset, 1 minute, 10
  minutes, or 30 minutes.
- **Maximum Duration** The total time the affliction can continue before ending.
- **Stages** The stage track of the drug itself.
- **Addiction Note** Any nonstandard addiction rule, such as a lower addiction
  DC, the virulent trait, extra addiction stages, or a capped maximum stage.

### What Drugs Usually Feel Like

Most drugs follow the same broad shape.

- The first stage is the reason people take the drug in the first place.
- The second stage is often the peak, or the point where the benefits begin to
  come with an obvious price.
- Later stages are ugly. Shaking limbs, dulled senses, panic, sleep, confusion,
  or collapse are all common.
- The best drugs give a narrow but memorable edge rather than a broad boost to
  everything. A good drug might steady the nerves, numb pain, sharpen a single
  sense, or let the user brush against the supernatural for a moment.
- Addiction is tracked separately, as usual for PF2e drugs, though some drugs
  are especially habit-forming or strangely forgiving.

### Components

Every component has the following properties.

- **Role** One or more of Base, Enhancer, or Solution.
- **Tags** Stimulant, Depressant, Hallucinogen, Magical, or a more specific
  magical descriptor such as Fire or Illusion.
- **Level** The natural strength of the component.
- **Chain** A two-letter compatibility code such as `AX` or `BY`.
- **Toxicity** A base value for Bases, or a modifier for Enhancers and
  Solutions.
- **Potency** A level modifier, usually `-1`, `0`, or `+1`.
- **Signature** A short phrase describing what this component tends to do in a
  finished drug.

### Roles in a Formula

- **Base** The heart of the drug. It decides what the high feels like.
- **Enhancer** The part that pushes the experience harder, sharper, stranger,
  or more dangerous.
- **Solution** The carrier that smooths, stretches, stabilizes, or warps the
  final mixture.

### Compatibility Chains

Each component's first chain letter must match the previous component's second
chain letter in the sequence Base -> Enhancer -> Solution.

- A Base with `AX` can connect to an Enhancer whose first letter is `X`.
- An Enhancer with `XB` can connect to a Solution whose first letter is `B`.

If a component can serve multiple roles, the same chain code applies regardless
of role.

### Final Drug Statistics

When you Cook a drug, determine its final statistics as follows.

- **Level** Highest component level, plus total Potency modifiers, to a minimum
  of the Base's level - 1 and a maximum of the highest component level + 1.
- **Toxicity** Base Toxicity plus all Enhancer and Solution Toxicity modifiers.
- **Traits** The union of all component tags. All finished drugs also gain the
  `drug` and `poison` traits. Most also have `alchemical` and `consumable`.
- **Saving Throw DC** Standard DC for the drug's final level, adjusted by
  Toxicity if desired: clean formulas often use `DC - 1`, ordinary formulas use
  the baseline DC, and brutal street formulas can use `DC + 1` or `DC + 2`.
- **Addiction DC** Based on the Toxicity table below.
- **Primary Effect** The Base usually shapes Stage 1.
- **Escalation** The Enhancer usually decides how sharply the drug peaks or
  how quickly it turns cruel.
- **Delivery and Duration** The Solution most strongly influences onset,
  maximum duration, and whether the drug feels smooth, lingering, acrid, or
  dreamlike.

If a formula includes both stimulant and depressant tags, increase Toxicity by

1. If the same non-magical tag appears on all three components, increase the
drug's level by 1, to the usual maximum, and treat the addiction as one band
worse on the Toxicity table.

## Toxicity

Toxicity measures how dirty, unstable, or self-destructive a drug is. A rare
high-level formula is not automatically worse than a common street drug; what
matters is whether the mixture is clean and deliberate or brutal and unstable.

| Toxicity | Quality | Addiction DC | Addiction Traits | Typical Drug Stages |
| --- | --- | --- | --- | --- |
| 0-1 | Clean | Drug DC - 2 | None | 2-3 stages; downside arrives late |
| 2-3 | Risky | Drug DC | None | 3-4 stages; mixed Stage 2 |
| 4-5 | Dirty | Drug DC | Virulent or +1 DC | 4-5 stages; Stage 3 is usually severe |
| 6+ | Lethal | Drug DC + 2 | Virulent | 5-6 stages; incapacitation is expected |

### Building the Stage Track

When you write a drug, let its stages grow naturally from the components rather
than adding a second subsystem on top of the affliction.

- **Stage 1** should feel attractive and usually brief.
- **Stage 2** should either heighten the experience or keep part of the high
  while introducing a clear drawback.
- **Stage 3** is the point where the consequences are no longer worth the rush.
- **Stage 4+** belong to especially filthy, addictive, or magical drugs and
  often end in stupefaction, collapse, sleep, madness, or unconsciousness.

Repeated use while already affected should not use a second separate track.
Instead, if a creature takes another dose of the same drug while still under
its effects, it attempts the new drug's initial Fortitude save and begins at
its current stage or the new result's stage, whichever is worse. Reset the
maximum duration from the new dose. In practice, taking more of the same drug
rarely makes things better for long.

### Addiction

Use the standard drug addiction rules, with the following added stages.

- **Stage 5** fatigued, drained 3, sickened 3, and stupefied 3 for 1 day
- **Stage 6** death

A drug can also bend the normal addiction rules in a few ways.

- **Capped Addiction** Particularly fashionable or diluted forms can set a
  maximum addiction stage, as pesh paste does.
- **Lower Addiction DC** A dream-drug or ritualized intoxicant can have an
  addiction DC below its main drug save DC.
- **Virulent Addiction** Dirty street stimulants and hallucinogens are strong
  candidates for virulent addiction.

## Discovery and Lab Work

### Collect

[EXPLORATION] [MANIPULATE]

You spend 10 minutes harvesting potentially useful matter from a creature,
plant, growth, mineral seam, magical residue, or similar source. Attempt a
Medicine, Nature, Survival, or applicable Lore check against a DC based on the
source's level.

Small or Medium remains usually support only 1 Collect attempt. Large remains
usually support 2. Huge or larger remains, rich growths, or stable mineral
sites might support more attempts at the GM's discretion.

**Critical Success** You collect 2 samples at the source's level. The first
attempt to Extract from one of those samples gains a +1 circumstance bonus.

**Success** You collect 1 sample at the source's level.

**Failure** You collect 1 damaged sample at the source's level - 2.

**Critical Failure** You ruin the viable material and collect nothing.

### Extract

[DOWNTIME] [MANIPULATE]

**Requirements** Alchemical Crafting; alchemist's tools or an alchemical lab

You spend 1 hour separating, testing, and identifying a sample. Attempt a
Crafting check against a DC based on the sample's level.

Each sample can withstand only 2 Extract attempts. A failed attempt does not
consume the sample, but still counts against that limit.

**Critical Success** You identify the component and gain 2 component units. You
also record strong process notes, granting a +1 item bonus to the first Refine
or Cook attempt involving that component.

**Success** You identify the component and gain 1 component unit.

**Failure** You fail to isolate a usable component unit, but the sample remains
available if it still has attempts left.

**Critical Failure** You contaminate the sample and destroy it.

### Refine

[DOWNTIME] [MANIPULATE]

**Requirements** Alchemical Crafting; alchemist's tools or an alchemical lab

**Prerequisite** You know the component's formula and expend 1 component unit.

You spend 1 day refining a known component formula. Attempt a hard Crafting
check against a DC based on the component's level. A component formula can be
successfully Refined at most twice. If you are legendary in Crafting, you may
successfully Refine it a third time.

Choose one refinement.

- **Purify** Reduce the component's Toxicity by 1, to a minimum of 0 for Bases
  or `-2` for modifiers.
- **Potentize** Increase the component's Potency by 1, to a maximum of `+1`.
- **Recode** Change one chain letter to another letter of your choice.

**Critical Success** Make 2 different refinements.

**Success** Apply the chosen refinement.

**Failure** You learn nothing useful and waste the unit.

**Critical Failure** You waste the unit and your notes turn misleading; the
next attempt to Refine or Cook using that component takes a -1 circumstance
penalty unless you spend 1 hour correcting your notes first.

### Cook

[DOWNTIME] [MANIPULATE]

**Requirements** Alchemical Crafting; an alchemical lab

**Prerequisite** You know 3 component formulas with different names: 1 Base,
1 Enhancer, and 1 Solution, all chain-compatible in order

You spend 4 days producing a stable prototype formula. Expend 1 component unit
of each chosen component and attempt a hard Crafting check against a DC based
on the formula's final level.

**Critical Success** You create a stable formula and 4 prototype doses. Future
Craft Drugs and Mass Produce checks for that exact formula gain a +1 item
bonus.

**Success** You create a stable formula and 2 prototype doses.

**Failure** The batch fails, but you salvage 1 random component unit.

**Critical Failure** The batch spoils violently. All 3 component units are
lost.

### Gather Component Stock

[DOWNTIME] [MANIPULATE]

Once you know a component formula, you can seek that exact precursor in the
wild or through a controlled source. This usually uses the normal `Gather Raw
Materials` downtime activity, but instead of receiving generic raw materials,
you gain component units for that specific formula.

Attempt the same skill and DC the GM assigns for gathering that source, usually
at a task level equal to the component's level.

**Critical Success** Gain 2 component units.

**Success** Gain 1 component unit.

**Failure** Gain no component units.

**Critical Failure** Gain no component units and the source is spoiled,
depleted, noticed, or otherwise unavailable to you until circumstances change.

## Crafting and Production

### Craft Drugs

[DOWNTIME] [MANIPULATE]

**Requirements** Alchemical Crafting; you know the drug's formula

Crafting doses for personal use follows the normal rules for crafting
alchemical consumables in Reforged, with the following changes.

- A batch always requires 1 component unit each of the formula's Base,
  Enhancer, and Solution, unless the GM allows purchased precursors to replace
  one or more units.
- A standard successful batch produces 2 doses of the drug.
- A critical success produces 3 doses instead.
- If the formula was first Cooked with a critical success, apply that formula's
  +1 item bonus to this Crafting check.

### Mass Produce

[DOWNTIME] [MANIPULATE]

**Requirements** Alchemical Crafting; an alchemical lab; access to each
component's recurring source, supplier, or stockpile

You scale a known drug for criminal trade, military issue, or elite clientele.
Spend 4 days and expend 2 component units each of the formula's Base,
Enhancer, and Solution. Attempt a Crafting check against a DC based on the
drug's level.

Mass production creates **lots** rather than individually counted doses.
Outside of trade play, 1 lot can be treated as 8 doses.

**Critical Success** You produce 3 lots.

**Success** You produce 2 lots.

**Failure** You produce no sellable lots, but recover 1 random expended
component unit.

**Critical Failure** You produce no lots, lose all expended units, and gain
1 Heat in the settlement where the lab operates.

## Distribution and Selling

Distribution assumes there is demand for intoxicants, stimulants, dream-drugs,
or occult experiences in the region. The PCs are not selling exact doses one
at a time; they are moving lots through fences, dens, handlers, and buyers.

### Heat

Heat measures attention from guards, guilds, gangs, rivals, and frightened
clients. Track Heat separately for each settlement or district.

| Heat | State | Effect |
| --- | --- | --- |
| 0 | Quiet | No modifier. |
| 1 | Rumors | No modifier, but people are talking. |
| 2 | Attention | `Move Product` checks take a -1 circumstance penalty. |
| 3 | Pressure | `Move Product` checks take a -2 circumstance penalty. |
| 4 | Crackdown | The first failure on `Move Product` each week becomes a critical failure. |
| 5 | Bust | You lose all unsold lots in that settlement and one route there collapses. Heat drops to 2 after you Lie Low for 1 week or relocate. |

Heat rises and falls only through actions that would reasonably change local
attention. A single quiet district can sit at Heat 0 while another one burns.

### Establish a Route

[DOWNTIME] [LINGUISTIC] [SECRET]

You cultivate a neighborhood, den, courier chain, noble salon, arena circuit,
dock route, or similar channel for future sales. Attempt Society, Deception,
Thievery, or Underworld Lore against a DC based on the settlement's level.

**Critical Success** You establish a strong route with capacity 2 lots per week
and gain a +1 circumstance bonus to your first `Move Product` check through it
each week.

**Success** You establish a route with capacity 1 lot per week.

**Failure** You fail to establish a safe route.

**Critical Failure** You offend, alarm, or attract the wrong people. Gain
1 Heat.

### Move Product

[DOWNTIME] [LINGUISTIC] [SECRET]

**Prerequisite** You have at least 1 lot to sell and a route with remaining
capacity this week.

You spend 1 day moving 1 lot through a route. Attempt Society, Deception,
Thievery, or Underworld Lore against a DC based on the higher of the
settlement's level or the drug's level.

On a success or critical success, gain income as though you had Earned Income
for a day at the drug's level. On a critical success, treat the task level as
1 higher. Selling a level 7 drug in a level 3 town is still a level 7 task.

**Critical Success** You sell the lot cleanly, gain income as above, and Heat
does not rise.

**Success** You sell the lot and gain income as above. If the drug's level is
5 or higher, or its Toxicity is 4 or higher, gain 1 Heat.

**Failure** The lot does not move. It remains unsold, the route's weekly
capacity is spent, and Heat does not change.

**Critical Failure** The lot is seized, spoiled, or stolen. You lose it and
gain 1 Heat.

### Lie Low

[DOWNTIME] [SECRET]

You cool attention by shutting down, feeding false rumors, burning evidence,
changing handlers, or leaning on frightened associates. Attempt Deception,
Society, Stealth, or Underworld Lore against a DC based on the settlement's
level.

**Critical Success** Reduce Heat by 2.

**Success** Reduce Heat by 1.

**Failure** No change.

**Critical Failure** Gain 1 Heat.

## Creating New Drugs

Once a formula is successfully cooked, the GM can write it up as a proper item
entry. The easiest way is to give the drug a short bit of street reputation,
set its save DC and duration, then write a stage track that follows naturally
from its ingredients.

### Drug Stat Block Template

Use the following template.

```text
[Drug Name] Item [Level]
[Rarity] Alchemical Consumable Drug [Delivery] Poison [Optional Tags]
Price [price]
Usage held in 1 hand; Bulk L
Activate [one-action] Interact

Formula [base] + [enhancer] + [solution]
Chain [base chain] -> [enhancer chain] -> [solution chain]
Formula Level [level]; Toxicity [final toxicity]; Addiction DC [DC];
Component Tags [tags]

[One or two lines of fiction and street reputation.]
The save for addiction to [drug name] is DC [DC]. [Any special addiction note.]

Saving Throw DC [DC] Fortitude; [Onset X;] Maximum Duration [duration];
Stage 1 [tempting upside] ([stage duration]);
Stage 2 [peak or mixed state] ([stage duration]);
Stage 3 [serious drawback] ([stage duration]);
[Stage 4+ as needed]
```

### Keeping the Drug in Bounds

- Stage 1 should feel worthwhile, but it should not outshine a same-level
  alchemical consumable without asking a price later.
- Drugs should almost never improve attack rolls, spell DCs, or every part of
  a character's performance at once.
- Small item bonuses, temporary Hit Points, narrow resistances, altered fear,
  strange senses, and brief occult twists are all safer choices.
- By Stage 3, the drug should have become a real liability.
- If a drug brushes against spell-like effects, keep that effect brief,
  personal, and weaker than a dedicated magical consumable of the same level.

### Shaping the Drug by Tag

The dominant tag usually tells you what the arc of the drug should look like.

- **Stimulant** Stage 1 usually grants speed, initiative, Reflex, temporary Hit
  Points, a fear benefit, or an extra mobility option. Later stages lean toward
  clumsy, drained, stupefied, or confusion.
- **Depressant** Stage 1 usually grants calm, pain dulling, resistance, or a
  bonus against mental pressure. Later stages lean toward fatigued, slowed,
  off-guard, stupefied, asleep, or unconscious.
- **Hallucinogen** Stage 1 usually alters fear, perception, sensation, or one
  occult angle of reality. Later stages lean toward dazzled, stupefied,
  frightened, clumsy, confusion, or unconsciousness.
- **Magical** Add one strange but focused effect. Good magical drug effects
  feel uncanny and intimate: glimpses of fate, altered weight, thin-matter
  sight, shadow blur, and other sensory or bodily distortions.

### Let the Ingredients Speak

The three ingredients should each leave a clear mark on the finished drug.

- **Base** Usually writes Stage 1.
- **Enhancer** Either improves Stage 1 and carries that improvement into Stage
  2, or it pushes Stage 2 sharply upward while worsening Stage 3.
- **Solution** Decides whether the drug is immediate or delayed, smooth or
  jagged, short-lived or lingering.

### Choosing Onset and Duration

The following ranges fit most drugs well.

- **Immediate onset or no onset line** Violent stimulants, sharp combat drugs,
  and fast magical rushes.
- **1 minute onset** Smoked or quickly ingested highs that need a brief rise.
- **10 minute onset** Herbal, mellow, or body-heavy substances.
- **30 minute onset** Ritualized teas, dream-drugs, and slow-bloom narcotics.

- **Maximum Duration 1 minute** Pure combat spikes.
- **Maximum Duration 30 minutes** Intense but short occult or sensory highs.
- **Maximum Duration 4 hours** Street narcotics, social highs, and habitual
  recreational drugs.
- **Maximum Duration 6 hours** Especially persistent drugs or substances with a
  long comedown.

### Tone at the Table

If you want the subsystem to feel like fantasy underworld chemistry, keep the
logic practical and material even when the ingredients are impossible.

- Distinguish between raw source, usable component, formula, dose, lot, and
  route.
- Make rare sources matter. A dragon gland, moon fungus, or cursed spring
  should change what is possible.
- Let PCs build operations. A hidden lab, a supplier, a courier, and a route
  are all adventure hooks.
- Keep supernatural effects sensory and bodily before they become world-shaking.
  Most drugs should sharpen, numb, distort, embolden, or unmoor rather than
  duplicate full spellcasting.

## Sample Finished Drugs

The following examples show what a finished drug can look like once written up
for play.

### Iron Mercy Item 2

Alchemical Consumable Drug Ingested Poison Stimulant
**Price** 6 gp
**Usage** held in 1 hand; **Bulk** L
**Activate** [one-action] Interact

**Formula** pesh + qat + calmleaf extract
**Chain** `AA -> AX -> XX`
**Formula Level** 2; **Toxicity** 4; **Addiction DC** 16; **Component Tags**
Stimulant, Stimulant, Depressant

Iron mercy is a bitter green paste wrapped in wax paper or packed into small
pellets. Teamsters, enforcers, and desperate watchmen prize it for the way it
steadies the nerves before it starts to wear on the body. The save for
addiction to iron mercy is DC 16, and the addiction has the virulent trait.

**Saving Throw** DC 16 Fortitude; **Onset** 1 minute; **Maximum Duration**
4 hours; **Stage 1** +2 item bonus to saves against fear and 1 temporary Hit
Point per level the first time you reach this stage (10 minutes); **Stage 2**
+2 item bonus to saves against fear and +1 item bonus to Reflex saves, but you
become clumsy 1 (1 hour); **Stage 3** clumsy 2 and stupefied 1 (1 hour);
**Stage 4** fatigued, clumsy 2, and stupefied 2 (1 hour)

### Velvet Drop Item 3

Alchemical Consumable Drug Ingested Poison Hallucinogen
**Price** 10 gp
**Usage** held in 1 hand; **Bulk** L
**Activate** [one-action] Interact

**Formula** crystal veil + shiver oil + blood dew
**Chain** `BA -> AY -> YA`
**Formula Level** 3; **Toxicity** 2; **Addiction DC** 18; **Component Tags**
Hallucinogen, Hallucinogen

Velvet drop is sold in tiny glass phials and favored by courtesans, spies, and
the sort of people who need to smile through dread. It fills the body with a
light, floating calm before the senses begin to slip. The addiction to velvet
drop has the virulent trait.

**Saving Throw** DC 18 Fortitude; **Maximum Duration** 4 hours; **Stage 1**
whenever you would become frightened, reduce that condition's value by 1; you
also gain a +1 item bonus to saves against fear (10 minutes); **Stage 2**
clumsy 1 and stupefied 1 (1 hour); **Stage 3** clumsy 2 and stupefied 2
(1 hour); **Stage 4** asleep (1 hour)

### Witchlight Syrup Item 8

Alchemical Consumable Drug Ingested Poison Hallucinogen Magical
**Price** 100 gp
**Usage** held in 1 hand; **Bulk** L
**Activate** [one-action] Interact

**Formula** wyrmwood essence + malevolent fey flesh + blood dew
**Chain** `AX -> XY -> YA`
**Formula Level** 8; **Toxicity** 4; **Addiction DC** 25; **Component Tags**
Hallucinogen, Hallucinogen, Magical, Illusion

Witchlight syrup is dense, black, and threaded with prismatic sheen when held
to a flame. Those who traffic in occult contraband whisper that it lets the
mind bite into the hidden shape of things, though many who chase that vision
never wake cleanly from it. The save for addiction to witchlight syrup is
DC 25, and the addiction has the virulent trait.

**Saving Throw** DC 24 Fortitude; **Onset** 10 minutes; **Maximum Duration**
30 minutes; **Stage 1** you can see through cloth, paper, and similarly thin
material, and you ignore concealed from such barriers (1 minute); **Stage 2**
as stage 1, and you gain a +1 item bonus to Reflex saves, but become stupefied
1 (1 minute); **Stage 3** stupefied 2 and clumsy 1 (10 minutes); **Stage 4**
stupefied 2, clumsy 2, and slowed 1 (10 minutes); **Stage 5** unconscious
(remaining duration)

## Known Components

These are example components for starting play. Add more as the campaign grows.

| Name | Roles | Tags | Lv | Chain | Toxicity | Potency | Signature |
| --- | --- | --- | --- | --- | --- | --- | --- |
| pesh | Base | Stimulant | 2 | AA | 3 | 0 | Courage rush; drugs built from it usually resist fear and grant a short burst of temporary Hit Points. |
| qat | Base, Enhancer | Stimulant | 2 | AX | +2 | 0 | Wired focus; often sharpens initiative, Reflex, or fine motor speed. |
| shiver oil | Enhancer, Solution | Hallucinogen | 3 | AY | +1 | +1 | Fear inversion; often turns panic into icy calm or reckless detachment. |
| blood dew | Solution | - | 2 | YA | -2 | -1 | Gentle carrier; softens crash, lowers Toxicity, and reduces onset harshness. |
| darkwood bark | Enhancer | Depressant | 2 | BX | 0 | +1 | Pain blunting; often grants resistance against blunt trauma or ignores minor pain penalties. |
| calmleaf extract | Base, Solution | Depressant | 1 | XX | -1 | 0 | Soft sedation; often lowers a formula's level by 1 but makes it cleaner and easier to distribute. |
| black pudding ooze | Base | Depressant | 6 | BX | 9 | 0 | Caustic numbness; grants heavy pain suppression at the cost of catastrophic internal damage. |
| malevolent fey flesh | Enhancer, Solution | Hallucinogen, Magical, Illusion | 8 | XY | +2 | +1 | Emotion bleed; euphoria, terror, and false beauty spill into sensory distortion. |
| basilisk blood | Enhancer | Magical, Transmutation | 5 | BA | +1 | 0 | Hardening spasm; drugs built from it often stiffen the body, steady aim, or threaten partial petrification on overdose. |
| wyrmwood essence | Base | Hallucinogen | 5 | AX | 4 | 0 | Penetrating sight; thin matter, weak concealment, and surface structure become visible. |
| shroom crystalshine | Base, Solution | Hallucinogen | 6 | AY | +2 | +1 | Gravity slip; air feels dense, falls feel slow, and distance becomes unreliable. |
| crystal veil | Base, Enhancer | Hallucinogen | 4 | BA | 3 | -1 | Floating analgesia; pain and fear blur into manic weightlessness. |
| umbral elixir | Enhancer | Depressant, Magical, Shadow | 4 | BY | +2 | -1 | Grave pull; earth hunger, shadow quiet, and a desire to become still and unseen. |
