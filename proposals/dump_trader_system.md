<!-- markdownlint-disable MD013 -->

# Caravan Trade Subsystem

This subsystem models caravans as recurring mobile businesses rather than as
static merchants. It is intended for GM use. Players should usually see only
the results: what a caravan has for sale, how much coin it can spend, what
goods are in demand, and whether a familiar caravan has prospered or fallen on
hard times since the last time the party met it.

This subsystem serves four purposes.

- It determines how much coin a caravan can spend when the PCs want to sell.
- It determines what kinds of supplies and items a caravan currently offers.
- It gives the GM a simple way to resolve off-screen trade journeys.
- It allows recurring caravans to grow, suffer losses, and feel like part of a
  living world.

Use [Assess Value or Negotiate](../rules/06-exploration-actions.md) whenever
the PCs haggle over prices. This subsystem does not replace that activity; it
supplies the business logic behind it.

## Using This Subsystem

The subsystem is intentionally abstract. Do not track individual crates,
inventory manifests, or pack animals unless they are story-relevant.

For most caravans, the GM only needs to record the following.

- Name
- Level
- Profile
- Mercantile Lore
- Trade DC
- Current Working Capital
- Current Stock Pools
- Invested Cargo
- Caravan XP

When a caravan first appears, or after it completes a trade journey, follow
this procedure.

1. Choose the caravan's level and profile.
2. Note its base statistics from the Caravan Progression table.
3. Roll for its current liquidity to determine its current Working Capital.
4. Adjust its stock pools for its profile.
5. If it is a recurring caravan, also note any active route, debts, losses, or
   recent successes that matter.

## Caravan Statistics

Every caravan has the following statistics.

| Statistic | Description |
| --- | --- |
| Level | Overall business size, reputation, logistics, and commercial reach. |
| Profile | The caravan's trade identity, such as provisioner, outfitter, or luxury broker. |
| Mercantile Lore | Skill modifier used for trade checks, market analysis, and commercial decisions. |
| Trade DC | Equal to 10 + Mercantile Lore. Use this when the caravan haggles as an organized business. |
| Working Capital | Coinage, letters of credit, and readily available assets the caravan can presently use to buy goods. This does not represent the caravan's total wealth, wagons, warehouses, or existing cargo. |
| Provision Stock | The value of common travel staples the caravan currently has available for sale. |
| General Stock | The value of ordinary common goods the caravan currently has available for sale. |
| Specialty Stock | The value of goods tied to the caravan's profile. |
| Invested Cargo | The value of goods the caravan has already purchased and is carrying for resale. |
| Caravan XP | Experience earned through completed trade journeys. |

## Caravan Progression

This subsystem assumes that caravans important enough to matter in play begin
at 3rd level. Smaller peddlers, isolated drovers, and one-wagon traders usually
work better as ordinary merchants without subsystem tracking.

| Level | Mercantile Lore | Trade DC | Base Working Capital | Provision Stock | General Stock | Specialty Stock |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| 3 | +10 | 20 | 280 gp | 40 gp | 80 gp | 40 gp |
| 4 | +12 | 22 | 420 gp | 60 gp | 120 gp | 60 gp |
| 5 | +14 | 24 | 700 gp | 100 gp | 180 gp | 120 gp |
| 6 | +16 | 26 | 900 gp | 120 gp | 260 gp | 160 gp |
| 7 | +18 | 28 | 1,120 gp | 160 gp | 360 gp | 240 gp |
| 8 | +20 | 30 | 1,600 gp | 220 gp | 500 gp | 320 gp |
| 9 | +22 | 32 | 2,400 gp | 320 gp | 700 gp | 480 gp |
| 10 | +24 | 34 | 3,600 gp | 450 gp | 1,000 gp | 700 gp |

These numbers represent a healthy baseline, not a promise. A caravan that was
raided last week, recently made a major investment, or is flush with coin from
a spectacular run can vary significantly.

## Current Liquidity

When a caravan first appears in play, or after it completes a trade journey,
roll 1d6 and apply the result to its Base Working Capital.

| d6 | Liquidity | Working Capital |
| --- | --- | ---: |
| 1 | Depleted | 70% of base |
| 2 | Lean | 85% of base |
| 3-4 | Normal | 100% of base |
| 5 | Flush | 115% of base |
| 6 | Exceptionally Flush | 130% of base |

Round the final amount to the nearest 5 gp.

Liquidity changes how much coin the caravan can spend right now. It does not
change its level, routes, or total assets.

### VTT Working Capital Table

If you use a VTT and want a single roll formula for a caravan's available funds
 on arrival, use the following table instead of the liquidity table above.

These formulas intentionally produce a spread around the same baseline values
used by this subsystem while keeping results easy to roll in Foundry or a
similar VTT.

| Level | VTT Working Capital Formula |
| --- | --- |
| 3 | `/r 280 + (10d10 - 55)` |
| 4 | `/r 420 + (12d10 - 66)` |
| 5 | `/r 700 + (16d10 - 88)` |
| 6 | `/r 900 + (18d10 - 99)` |
| 7 | `/r 1120 + (20d10 - 110)` |
| 8 | `/r 1600 + (24d10 - 132)` |
| 9 | `/r 2400 + (30d10 - 165)` |
| 10 | `/r 3600 + (36d10 - 198)` |

Use either the liquidity table or the VTT formula table for a given arrival,
not both.

## Caravan Profiles

Choose or roll a profile for each caravan. A profile changes the feel of the
caravan, what it tends to carry, and what it prefers to buy.

Round adjusted stock pools to the nearest 5 gp.

| Profile | Preferred Goods | Stock Adjustment |
| --- | --- | --- |
| General Trader | Mixed cargo, common tools, cloth, household goods, basic imports | No adjustment |
| Provisioner | Food, fodder, water, lamp oil, rope, camping goods, ammunition | Provision Stock × 1.5; General Stock × 0.75; Specialty Stock × 0.5 |
| Outfitter | Weapons, armor, tools, repair materials, kits, travel gear | Provision Stock × 0.75; General Stock × 1.25; Specialty Stock × 1 |
| Luxury Broker | Jewelry, fine clothing, spices, art objects, rare curios | Provision Stock × 0.5; General Stock × 0.75; Specialty Stock × 1.5 |
| Salvage Dealer | Scrap, trophies, monster parts, reclaimed gear, alchemical salvage | Provision Stock × 0.75; General Stock × 1; Specialty Stock × 1.25 |

Profiles do not change the caravan's level or Working Capital. They change the
kind of business the caravan does.

## Stock Pools and Item Availability

Stock pools are not exact inventories. They are spending limits for the GM.

When the PCs want to buy something from a caravan, determine whether the item
fits one of the stock pools below. If it does, subtract the item's price from
that pool.

### Provision Stock

Provision Stock represents the caravan's current supply of routine travel and
camping staples.

This usually includes the following.

- Rations and preserved food
- Fodder and feed
- Waterskins, sacks, blankets, tents, rope, torches, and lamp oil
- Common ammunition and simple replacement supplies
- Other common mundane gear that a traveling company would reasonably keep in
  ready quantity

As long as the caravan still has at least 10 gp of Provision Stock, assume it
can fill any reasonable purchase of common staples without the GM tracking
individual bundles.

### General Stock

General Stock represents ordinary trade goods not tied to a special market.

General Stock can supply common items up to item level equal to the caravan's
Market Level - 1, minimum 1. This includes mundane gear, common consumables,
and routine permanent items that make sense for the caravan's route.

### Specialty Stock

Specialty Stock represents the caravan's distinctive goods.

Specialty Stock can supply common items matching the caravan's profile up to
item level equal to the caravan's Market Level. With GM approval, it can also
include a small number of uncommon goods that strongly fit the caravan's route,
patrons, or profile.

Rare and unique items should never appear from stock pools unless their
presence is story-important.

## Market Level

Whenever stock, resale value, or trade reach matters, determine the caravan's
Market Level.

The Market Level is the lower of the following.

- Caravan Level
- Settlement Level of the place where the caravan is currently trading

This represents the scale of the market the caravan can currently exploit.

## Buying from a Caravan

Ordinary purchases can be resolved at listed price. If haggling matters, use
[Assess Value or Negotiate](../rules/06-exploration-actions.md).

Use the following guidelines.

- If the desired goods fit Provision Stock, deduct their price from Provision
  Stock.
- If the desired goods fit General Stock, deduct their price from General Stock.
- If the desired goods fit the caravan's profile, deduct their price from
  Specialty Stock first.
- Once a stock pool is depleted, the caravan cannot provide more of that type
  of good until it resupplies.

The GM should not let PCs strip a caravan of all mundane necessities unless the
price paid and the fiction support it. A caravan still needs enough of its own
provisions to stay on the road.

## Selling to a Caravan

When the PCs sell to a caravan, use [Assess Value or
Negotiate](../rules/06-exploration-actions.md) to determine the final price.
This subsystem answers three additional questions.

### Can the caravan afford the purchase?

The caravan cannot buy more than its current Working Capital allows.

If the caravan lacks sufficient Working Capital, it can do one of the
following.

- Refuse the purchase
- Buy only part of the lot
- Offer delayed payment, letters of credit, or barter if the campaign supports
  such arrangements

### Is the cargo a good fit?

Assign the cargo one broad tag or two at most.

- Provisions
- General Goods
- Arms and Armor
- Alchemical and Medical
- Luxury
- Salvage and Curios

If the goods match the caravan's profile or the destination market's demand,
apply one favorable market modifier before negotiation, usually +10%.

If the goods are a poor fit for the caravan's route, bulky with weak demand, or
already oversupplied, apply one unfavorable market modifier before negotiation,
usually -10%.

Do not stack multiple special demand modifiers unless the circumstance is
exceptional.

### What happens after the purchase?

Subtract the final purchase price from the caravan's Working Capital and add
that amount to its Invested Cargo.

The caravan has now converted liquid buying power into cargo it intends to
resell elsewhere.

## Destination Demand

To make the world feel alive, assign settlements and routes one or two strong
demand tags. This affects both what caravans carry into an area and what they
prefer to buy before leaving it.

| Destination or Route | Usually High Demand | Usually Weak Demand |
| --- | --- | --- |
| Frontier Village | Provisions, General Goods, Arms and Armor | Luxury |
| Mining Camp | Provisions, General Goods, Alchemical and Medical | Luxury |
| Military Post | Provisions, Arms and Armor, Alchemical and Medical | Luxury |
| Pilgrimage Route | Provisions, Alchemical and Medical, Luxury | Salvage and Curios |
| Market Town | General Goods, Provisions | None by default |
| Noble Enclave | Luxury, Alchemical and Medical | Salvage and Curios |
| Ruin Fringe | Provisions, Salvage and Curios, Alchemical and Medical | Luxury |
| River Port or Trade Hub | General Goods, Luxury, mixed imports | None by default |

This table is guidance, not a restriction. A famine, war, plague, festival, or
recent monster attack can change demand immediately.

## Trade Journeys

A trade journey represents the caravan leaving the current settlement, traveling
to another market, conducting business there, and returning with its affairs
resolved. In most campaigns this takes 3 to 14 days, but remote routes may take
far longer.

Trade journeys are resolved off-screen unless the journey itself becomes an
adventure.

### Step 1: Choose the Destination

Choose the destination settlement and note its level and demand tags.

Determine the Market Level as normal.

### Step 2: Note Route Difficulty

Choose one route category.

| Route | Modifier |
| --- | ---: |
| Protected or heavily patrolled | +1 |
| Ordinary | +0 |
| Dangerous | -1 |
| War-torn, monster-haunted, or highly unstable | -2 |

### Step 3: Determine Cargo Fit

If most of the caravan's Invested Cargo matches the destination's strong demand
or the caravan's own profile, the journey gains a +1 circumstance bonus to the
trade check.

If the cargo is a poor fit for the destination or clearly oversupplied there,
the journey takes a -1 circumstance penalty to the trade check.

### Step 4: Check for Market Saturation

Small settlements cannot absorb unlimited quantities of valuable cargo.

If the caravan's Invested Cargo exceeds the destination's Comfortable Trade
Value, either split the sale across multiple journeys or apply a -2 circumstance
penalty to the trade check.

| Settlement Level | Comfortable Trade Value |
| --- | ---: |
| 0-2 | 100 gp |
| 3-4 | 250 gp |
| 5-6 | 750 gp |
| 7-8 | 2,000 gp |
| 9-10 | 5,000 gp |
| 11+ | Effectively unrestricted |

### Step 5: Attempt the Trade Check

Attempt a Mercantile Lore check against the standard Level DC of the Market
Level, applying route and cargo modifiers.

### Step 6: Resolve Profit or Loss

Return the caravan's Invested Cargo to Working Capital, then apply the result
below to determine profit or loss on that cargo.

| Result | Trade Result | Caravan XP |
| --- | --- | ---: |
| Critical Success | Gain profit equal to 25% of Invested Cargo | 150 XP |
| Success | Gain profit equal to 10% of Invested Cargo | 100 XP |
| Failure | No profit or loss | 50 XP |
| Critical Failure | Lose value equal to 10% of Invested Cargo | 25 XP |

After resolving the journey, set Invested Cargo to 0.

If the caravan had no meaningful Invested Cargo, the GM can skip the check or
resolve a token journey that grants no profit and no XP.

## Caravan Advancement

A caravan gains a level every 1,000 XP. Excess XP carries over.

When a caravan gains a level, update the following.

- Mercantile Lore
- Trade DC
- Base Working Capital
- Stock Pools

The caravan does not instantly gain its new Base Working Capital in coin. Use
the new value the next time you roll liquidity after a completed trade journey
or major financial reset.

Leveling up represents better routes, more employees, stronger contracts,
greater access to capital, and a wider reputation.

## Caravan Perks

Each time a caravan gains a level, it also gains one perk. Perks represent the
way that caravan has chosen to grow. Some caravans expand their route
discipline and transport capacity, some become harder targets, some learn to
carry dangerous or delicate cargo, and some turn themselves into social events
that attract crowds wherever they stop.

Unless a perk says otherwise, a caravan cannot take the same perk more than
once.

The GM should choose perks that match the caravan's story, staff, patrons,
route, and profile rather than selecting them at random.

### Logistics Perks

#### Efficient Quartermasters

The caravan's records, loading plans, and supply discipline are unusually good.

- Increase Provision Stock by 25%.
- Increase General Stock by 10%.
- The caravan ignores the first 10 gp of Provision Stock that would otherwise
  be depleted by ordinary rural trade during a visit.

#### Reliable Teamsters

The caravan has disciplined drivers, spare animals, and better route planning.

- Gain a +1 circumstance bonus to trade checks during Trade Journeys.
- Treat ordinary routes as protected or heavily patrolled for the purpose of
  route modifiers.

#### Warehouse Ties

The caravan has stable suppliers and off-route storage arrangements.

- Increase Base Working Capital by 10%.
- When determining current liquidity, treat a result of 1 as 2.

#### Broad Load Discipline

The caravan is unusually good at packing mixed cargo without losing efficiency.

- Increase Comfortable Trade Value by 25% when checking market saturation for
  this caravan.
- The caravan can carry one additional cargo tag without taking the normal poor
  fit penalty during a Trade Journey.

### Defense Perks

#### Hardened Guards

The caravan employs better guards, tougher outriders, or more experienced
watch captains.

- Treat dangerous routes as ordinary for the purpose of route modifiers.
- If you use Optional Trade Events, reduce cargo loss from bandits, monsters,
  or sabotage by 5% of Invested Cargo.

#### Veteran Escort

The caravan travels with a respected escort force or contracted mercenaries.

- Gain a +2 circumstance bonus to Trade DC against coercive or openly hostile
  price pressure.
- If the caravan suffers a critical failure on a Trade Journey, you can reduce
  it to a failure once per arrival cycle.

#### Secure Camp Routine

The caravan is hard to raid while encamped and keeps better night discipline.

- If you use Optional Trade Events, a result of 1 on the event table becomes a
  result of 2 instead.
- Rural settlements and roadside camps treat the caravan as one step safer and
  more respectable for first impressions.

### Special Cargo Perks

#### Warded Compartments

The caravan has invested in sealed chests, treated linings, or magical
stabilization for fragile goods.

- Increase Specialty Stock by 25%.
- The caravan can transport one category of delicate cargo without it counting
  as a poor fit solely because of fragility, contamination risk, or spoilage.

Examples include alchemical goods, preserved monster parts, ritual supplies,
rare books, unstable salvage, or other similarly delicate cargo.

#### Arcane Caravan Guards

The caravan employs battle mages, abjurers, or ritual specialists to defend
high-value loads.

- The caravan can safely carry magically protected cargo.
- Goods that are especially vulnerable to theft, magical tampering, or hostile
  environments do not take the usual penalty for obvious risk.
- If you use Optional Trade Events, magical sabotage, spoilage from ambient
  magic, or similar supernatural mishaps can be ignored once per Trade Journey.

This perk is ideal for caravans that move spellbooks, rare reagents, cursed
objects under seal, unstable relics, diplomatic treasures, or other cargo that
ordinary guards are not enough to protect.

#### Sanctuary Cages

The caravan has custom cages, reinforced shrines, holy seals, padded frames, or
other built environments suited to special transport.

- Choose one category of special cargo the caravan is built to carry, such as
  live beasts, holy relics, hazardous alchemy, funerary remains, or noble
  luxuries.
- While carrying that category, the caravan gains a +1 circumstance bonus to
  trade checks for Trade Journeys.
- Buyers seeking that category treat the caravan as one step more reputable.

### Entertainment Perks

#### Caravan Festival

The caravan brings musicians, cooks, performers, or novelty attractions that
turn its arrival into an event.

- Rural settlements, villages, and small towns usually have a favorable initial
  attitude toward the caravan unless there is a reason not to.
- Increase Provision Stock sales opportunities by 25% during visits to
  under-supplied or isolated communities.

#### Carnival Train

The caravan includes games, stage acts, curiosities, beasts, or traveling
spectacles that draw paying crowds.

- Increase Working Capital by 10% after any successful Trade Journey whose
  destination is a village, town, pilgrimage route, or festival site.
- The caravan can justify carrying one additional Luxury cargo tag without it
  feeling out of place in poor or rural regions.

#### Beloved Entertainers

The caravan has become a known social institution on part of its route.

- When this caravan returns to a settlement that has seen it before, treat the
  caravan as having a favorable reputation unless the campaign fiction says
  otherwise.
- The GM can treat one weak-demand result for Luxury or novelty goods as normal
  demand in communities that look forward to the caravan's arrival.

### Advanced Perks

The following perks are best for caravans of 6th level or higher.

#### Regional Trade Network

Prerequisite: Warehouse Ties or Reliable Teamsters

The caravan has become part of a wider and more resilient commercial web.

- Increase Base Working Capital by 15%.
- Gain a +1 circumstance bonus to Mercantile Lore checks made for Trade
  Journeys.
- Once per arrival cycle, the caravan can count the destination settlement as
  1 level higher for determining Market Level, to a maximum of the caravan's
  own level.

#### Iron Road Convoy

Prerequisite: Hardened Guards

The caravan has grown into a disciplined convoy with strong route control.

- Treat dangerous routes as protected or heavily patrolled for the purpose of
  route modifiers.
- If you use Optional Trade Events, results of 1 or 2 each become 3 instead.

#### Grand Procession

Prerequisite: Caravan Festival or Carnival Train

The caravan is no longer just a merchant line but a public attraction in its
own right.

- Increase Specialty Stock by 20%.
- Villages and towns usually count as one step more receptive to the caravan's
  arrival.
- After a successful Trade Journey to a rural, frontier, or pilgrimage
  destination, increase final profit by an additional 5% of Invested Cargo.

## Optional Trade Events

If you want journeys to feel more dynamic, roll 1d12 once per trade journey.

| d12 | Event |
| --- | --- |
| 1 | Bandits, monsters, or sabotage. Lose 10% of Invested Cargo before resolving the trade check. |
| 2 | Spoilage, breakage, or animal loss. Lose 5% of Invested Cargo before resolving the trade check. |
| 3 | Tariffs, bribes, or emergency repairs. Reduce final profit by 5% of Invested Cargo. |
| 4 | Delay. No direct effect, but the caravan arrives late and may miss a story opportunity. |
| 5-8 | Uneventful journey. |
| 9 | Favorable rumor. Gain a +1 circumstance bonus to the trade check. |
| 10 | Strong market. Increase final profit by 5% of Invested Cargo. |
| 11 | Exclusive contract or timely arrival. Increase final profit by 10% of Invested Cargo. |
| 12 | Trade boom. Increase final profit by 20% of Invested Cargo and gain 50 additional XP. |

## Recurring Caravans

A recurring caravan should retain the following between appearances.

- Current level
- Current XP
- Current Working Capital
- Current profile
- Current reputation with the PCs
- Active route notes
- Any major debts, losses, guards, rivals, or patrons

Caravans should also remember previous deals.

- A caravan that was cheated, rescued, or treated generously should behave
  accordingly.
- A caravan that repeatedly buys the same narrow kind of cargo should begin to
  saturate that route unless it expands to a new market.
- A caravan that repeatedly profits from a region should become more recognizable
  there, with better security and more reliable stock.

This is where the subsystem stops being a merchant table and starts feeling
like part of the campaign world.

## Quick Caravan Creation

When you need a caravan quickly, use this checklist.

1. Choose a level based on the route's importance.
2. Choose a profile.
3. Roll liquidity and set current Working Capital.
4. Determine the current settlement's level and the caravan's Market Level.
5. Adjust stock pools for the profile.
6. Assign one likely destination and one or two demand tags.
7. Name the caravan and note one memorable detail.

## Example Caravan

**Red Salt Company** is a 5th-level provisioner currently trading in a 4th-level
frontier town.

- Level 5
- Profile: Provisioner
- Mercantile Lore +14
- Trade DC 24
- Base Working Capital 700 gp
- Liquidity: Flush
- Current Working Capital 805 gp
- Market Level 4
- Provision Stock 150 gp
- General Stock 135 gp
- Specialty Stock 60 gp
- Invested Cargo 0 gp
- Caravan XP 300

Because Red Salt Company is a provisioner in a frontier settlement, it can
easily sell food, fodder, rope, tents, common ammunition, and similar travel
staples. It is also likely to buy preserved food, alchemical field supplies,
beast feed, or other practical goods before departing for a mining camp deeper
in the hills.
