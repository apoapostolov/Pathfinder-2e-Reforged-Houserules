<!-- markdownlint-disable MD013 -->

# Caravan Trade Subsystem

This subsystem treats caravans as recurring businesses rather than static
merchants. It is written for the GM. Players will usually see only the result:
what a caravan has for sale, how much coin it can spend, what goods are in
demand, and whether a familiar caravan has prospered or fallen on hard times
since the party last saw it.

Use it for four things.

- It determines how much coin a caravan can spend when the PCs want to sell.
- It determines what kinds of supplies and items a caravan currently offers.
- It gives the GM a simple way to resolve off-screen trade journeys.
- It allows recurring caravans to grow, suffer losses, and feel like part of a
  living world.

Use [Assess Value or Negotiate](../rules/06-exploration-actions.md) whenever
the PCs haggle over prices. This subsystem does not replace that activity. It
provides the business logic behind it.

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

Caravans important enough to matter in play usually begin at 3rd level.
Smaller peddlers, isolated drovers, and one-wagon traders usually work better
as ordinary merchants without subsystem tracking.

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

These numbers are a baseline. A caravan that was raided last week, made a major
investment, or just finished a very profitable run can vary quite a bit.

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

These formulas produce a spread around the same baseline values while staying
easy to roll in Foundry or a similar VTT.

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
kind of business it does.

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

### Hub Adjacency

Some settlements function above their usual scale because they sit close to a
major trade hub, port, or magical center and are tied into its traffic.

When a settlement has unusually strong access to a nearby major market, the GM
can treat it as 1 level higher when determining Market Level for caravans,
comfortable trade, and mediated orders. This should be used for places that are
regularly supplied by larger markets, not merely for towns with occasional
travelers.

Otari near Absalom is a good example of this rule. It remains a small town, but
its access to Absalom's traffic, agents, and commissioned trade makes it behave
as a somewhat stronger market than an equally sized remote settlement.

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

### Trade Ceiling and Mediated Orders

Caravans do not usually buy or stock individual commoditized or low-quality
items whose level is 4 or more below the caravan's level.

A caravan normally trades items up to its own level. It can also mediate access
to items up to 2 levels above its own level, but those goods are not part of its
standing stock. They must be obtained as special orders through private factors,
distant suppliers, or personal courier delivery. Such orders usually require
prepayment, extra delivery fees, waiting time, or all three.

As a default, a mediated order requires at least 20% prepayment, at least 5 gp
plus 5% of the order's price in courier or brokerage fees, and a delivery time
measured in days rather than hours. The GM should also treat mediated orders as
less certain than standing stock. A supplier can fail to secure the goods,
raise the final price, arrive late, or require the buyer to wait for the next
caravan run.

Items that are always in broad demand are the main exception. A caravan can
still buy, carry, and use staple goods such as basic healing potions, common
ammunition, lamp oil, rope, rations, feed, and other routine field supplies
that remain useful regardless of the caravan's level. This exception should be
kept narrow. It covers dependable staples, not every low-level consumable or
minor magical convenience.

This creates a simple default ladder.

- Refuse individual items of caravan level - 4 or lower
- Routinely trade items up to caravan level
- Mediate special orders up to caravan level + 2

The GM can also waive the refusal threshold for bulk cargo, salvage lots,
profile-defining goods, or items in unusually strong demand on that route.

## Selling to a Caravan

When the PCs sell to a caravan, use [Assess Value or
Negotiate](../rules/06-exploration-actions.md) to determine the final price.
The subsystem adds three questions.

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

The caravan has converted liquid buying power into cargo for resale elsewhere.

## Destination Demand

Assign settlements and routes one or two strong demand tags. This affects both
what caravans bring into an area and what they prefer to buy before leaving it.

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

Resolve trade journeys off-screen unless the journey itself becomes an
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

Even the best caravan cannot erase all route friction. Weather, politics,
bridge failures, ferries, inspections, hostile attention, and magical hazards
still shape the road. Route improvements, escort perks, and convoy perks can
raise a route's category, but no route can be improved above Protected or
heavily patrolled.

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

Leveling up reflects better routes, more employees, stronger contracts, greater
access to capital, and a wider reputation.

## Caravan Perks

Each time a caravan gains a level, it also gains one perk. Perks show how that
caravan has chosen to grow. Some improve discipline and carrying capacity.
Some make the caravan harder to attack. Some specialize in dangerous or
delicate cargo. Others turn the caravan into an attraction in its own right.

Unless a perk says otherwise, a caravan cannot take the same perk more than
once.

The GM should choose perks that match the caravan's story, staff, patrons,
route, and profile rather than selecting them at random.

Some perks list a minimum caravan level. These usually require the staff,
capital, equipment, or regional influence to support them.

### Logistics Perks

#### Efficient Quartermasters

The caravan's records, loading plans, and supply discipline are unusually good.
Its ledgers are current, its cargo marks are consistent, and its handlers know
exactly which wagon holds lamp oil, flour, spare tack, or winter blankets.

- Increase Provision Stock by 25%.
- Increase General Stock by 10%.
- The caravan ignores the first 10 gp of Provision Stock that would otherwise
  be depleted by ordinary rural trade during a visit.
- Teamsters, porters, and quartermasters quickly recognize this caravan as one
  that packs honestly and wastes little.

#### Reliable Teamsters

Minimum Level 4

The caravan has disciplined drivers, spare animals, and better route planning.
Its drivers know where wheels bog down in spring, where bridges are weak, and
which inns still honor old teamster contracts.

- Gain a +1 circumstance bonus to trade checks during Trade Journeys.
- Treat ordinary routes as protected or heavily patrolled for the purpose of
  route modifiers.
- Stables, ferrymen, and road wardens usually treat this caravan as seasoned
  traffic rather than green travelers.

#### Warehouse Ties

Minimum Level 4

The caravan has stable suppliers and off-route storage arrangements. Its
factors keep keys, seals, and standing agreements in market towns beyond the
main road.

- Increase Base Working Capital by 10%.
- When determining current liquidity, treat a result of 1 as 2.
- Merchants and warehouse clerks are more likely to know this caravan's marks
  and accept its letters, tallies, and promises as legitimate.

#### Broad Load Discipline

The caravan is unusually good at packing mixed cargo without losing efficiency.
Its wagons use nested crates, compartment frames, and careful loading order to
keep salt from tainting grain, tools from bruising fruit, and fine cloth from
traveling beside muddy salvage.

- Increase Comfortable Trade Value by 25% when checking market saturation for
  this caravan.
- The caravan can carry one additional cargo tag without taking the normal poor
  fit penalty during a Trade Journey.
- Inspectors and rival merchants can often tell at a glance that this caravan's
  loads were arranged by professionals.

### Defense Perks

#### Hardened Guards

The caravan employs better guards, tougher outriders, or more experienced
watch captains. Its sentries rotate properly, its outriders scout ahead, and
its guards know how to form a line around panicked animals before a raid
becomes a rout.

- Treat dangerous routes as ordinary for the purpose of route modifiers.
- If you use Optional Trade Events, reduce cargo loss from bandits, monsters,
  or sabotage by 5% of Invested Cargo.
- Villagers, toll keepers, and roadside traders usually think twice before
  mistaking this caravan for an easy mark.

#### Veteran Escort

Minimum Level 5

The caravan travels with a respected escort force or contracted mercenaries.
These are not merely armed drovers but known professionals with reputations,
captains, and preferred marching orders.

- Gain a +2 circumstance bonus to Trade DC against coercive or openly hostile
  price pressure.
- If the caravan suffers a critical failure on a Trade Journey, you can reduce
  it to a failure once per arrival cycle.
- Gate wardens, lesser officials, and petty extortionists usually recognize
  that this caravan is costly to pressure and dangerous to cross.

#### Secure Camp Routine

The caravan is hard to raid while encamped and keeps better night discipline.
Its wagons are circled with purpose, its lanterns are hooded, and its cooks,
guards, and drovers all know the camp signals.

- If you use Optional Trade Events, a result of 1 on the event table becomes a
  result of 2 instead.
- Rural settlements and roadside camps treat the caravan as one step safer and
  more respectable for first impressions.
- Hosts, reeves, and village elders are more willing to let this caravan camp
  near mills, shrines, or pasture land.

### Special Cargo Perks

#### Warded Compartments

The caravan has invested in sealed chests, treated linings, or magical
stabilization for fragile goods. Some wagons carry resin-lined drawers, padded
book cases, cooled alchemical lockers, or iron-bound cabinets marked with chalk
sigils and guild seals.

- Increase Specialty Stock by 25%.
- The caravan can transport one category of delicate cargo without it counting
  as a poor fit solely because of fragility, contamination risk, or spoilage.
- Scholars, apothecaries, and collectors usually regard the caravan as a safer
  handler of delicate property than ordinary drovers.

Examples include alchemical goods, preserved monster parts, ritual supplies,
rare books, unstable salvage, or other similarly delicate cargo.

#### Arcane Caravan Guards

Minimum Level 5

The caravan employs battle mages, abjurers, or ritual specialists to defend
high-value loads. Its sealed wagons are watched by spellwardens, glyph-cutters,
and practical adepts who know which threats are steel, which are curses, and
which call for ritual precautions instead.

- The caravan can safely carry magically protected cargo.
- Goods that are especially vulnerable to theft, magical tampering, or hostile
  environments do not take the usual penalty for obvious risk.
- If you use Optional Trade Events, magical sabotage, spoilage from ambient
  magic, or similar supernatural mishaps can be ignored once per Trade Journey.
- Temples, arcane colleges, and noble agents are more likely to entrust sealed
  commissions to a caravan known to travel with proper wards.

This perk is ideal for caravans that move spellbooks, rare reagents, cursed
objects under seal, unstable relics, diplomatic treasures, or other cargo that
ordinary guards are not enough to protect.

#### Sanctuary Cages

Minimum Level 4

The caravan has custom cages, reinforced shrines, holy seals, padded frames, or
other built environments suited to special transport. It may contain relic
shrines on suspension frames, beast wagons with feeding hatches, or traveling
alchemical labs built to survive rutted roads.

- Choose one category of special cargo the caravan is built to carry, such as
  live beasts, holy relics, hazardous alchemy, funerary remains, or noble
  luxuries.
- While carrying that category, the caravan gains a +1 circumstance bonus to
  trade checks for Trade Journeys.
- Buyers seeking that category treat the caravan as one step more reputable.
- People familiar with that trade usually know this caravan by sight, nickname,
  or the distinctive shape of its special wagons.

### Entertainment Perks

#### Caravan Festival

The caravan brings musicians, cooks, performers, or novelty attractions that
turn its arrival into an event. Children run ahead of it, villagers prepare
extra tables, and its cookfires and lantern strings are recognized from the
road.

- Rural settlements, villages, and small towns usually have a favorable initial
  attitude toward the caravan unless there is a reason not to.
- Increase Provision Stock sales opportunities by 25% during visits to
  under-supplied or isolated communities.
- The caravan usually picks up local gossip, songs, petitions, and invitations
  more quickly than a purely mercantile outfit.

#### Carnival Train

Minimum Level 5

The caravan includes games, stage acts, curiosities, beasts, or traveling
spectacles that draw paying crowds. Painted wagons, drummers, illusionists,
trained animals, and barkers turn a stopover into a fairground.

- Increase Working Capital by 10% after any successful Trade Journey whose
  destination is a village, town, pilgrimage route, or festival site.
- The caravan can justify carrying one additional Luxury cargo tag without it
  feeling out of place in poor or rural regions.
- Local officials, innkeepers, and shrine custodians may welcome the caravan
  for the coin and excitement it reliably brings.

#### Beloved Entertainers

Minimum Level 4

The caravan has become a fixture on part of its route. Its performers are
remembered by name, its old banners are recognized from afar, and its return
marks the season as surely as a local market day.

- When this caravan returns to a settlement that has seen it before, treat the
  caravan as having a favorable reputation unless the campaign fiction says
  otherwise.
- The GM can treat one weak-demand result for Luxury or novelty goods as normal
  demand in communities that look forward to the caravan's arrival.
- Communities along its route may keep stories, rivalries, romances, and
  standing invitations connected to the caravan from one visit to the next.

### Advanced Perks

The following perks are best for caravans of 6th level or higher.

#### Regional Trade Network

Prerequisites: 6th level, Warehouse Ties or Reliable Teamsters

The caravan has become part of a wider commercial web. Its masters exchange
couriers, debt tallies, and sealed memoranda with distant factors who may never
ride the same road themselves.

- Increase Base Working Capital by 15%.
- Gain a +1 circumstance bonus to Mercantile Lore checks made for Trade
  Journeys.
- Once per arrival cycle, the caravan can count the destination settlement as
  1 level higher for determining Market Level, to a maximum of the caravan's
  own level.
- Harbor clerks, guild agents, and tax collectors are more likely to treat this
  caravan as part of a recognized regional enterprise.

#### Iron Road Convoy

Prerequisites: 6th level, Hardened Guards

The caravan has grown into a disciplined convoy with strong route control.
Scouts ride ahead, standards mark the lead wagons, and hostile bands know this
company has crossed dangerous country before and intends to do so again.

- Treat dangerous routes as protected or heavily patrolled for the purpose of
  route modifiers.
- If you use Optional Trade Events, results of 1 or 2 each become 3 instead.
- Smaller merchants may try to attach themselves to this caravan's wake when
  crossing troubled country.

#### Grand Procession

Prerequisites: 6th level, Caravan Festival or Carnival Train

The caravan is no longer just a merchant line but a public attraction in its
own right. Its arrival is announced in advance, its banners are copied by
children, and some settlements rearrange market days to match its route.

- Increase Specialty Stock by 20%.
- Villages and towns usually count as one step more receptive to the caravan's
  arrival.
- After a successful Trade Journey to a rural, frontier, or pilgrimage
  destination, increase final profit by an additional 5% of Invested Cargo.
- Nobles, priests, and magistrates may seek the procession's presence for holy
  days, civic celebrations, and politically useful displays of prosperity.

## Optional Trade Events

If you want journeys to feel more dynamic, roll 1d12 once per trade journey.

| d12 | Event |
| --- | --- |
| 1 | Bandits, monsters, or sabotage. Lose 10% of Invested Cargo before resolving the trade check. |
| 2 | Spoilage, breakage, or animal loss. Lose 5% of Invested Cargo before resolving the trade check. |
| 3 | Tariffs, bribes, inspections, or emergency repairs. Reduce final profit by 5% of Invested Cargo. |
| 4 | Delay from weather, road damage, ferries, or official interference. No direct profit effect, but the caravan arrives late and may miss a story opportunity. |
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

Handled this way, a caravan becomes part of the campaign world rather than just
another merchant table.

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

## Example Caravans for Otari

The following caravans are written for campaigns centered on Otari, including
an *Abomination Vaults* campaign. Otari is a small fishing and timber town near
Absalom. Caravans that visit it usually come looking for fish, timber, rope,
tar, common provisions, and adventuring salvage, while bringing in finished
goods, better tools, weapons, luxuries, and commissioned items from larger
markets.

These entries preserve older roll formulas for arrival cadence, length of stay,
delivery time, and budget. Those formulas predate this subsystem, but the
listed caravan levels are the correct levels to use in play.

### Narin Alveri's Absalom Circuit

Narin Alveri runs a well-established circuit between Absalom, Otari, and
Meravon before returning home to Absalom. In Otari, this caravan is the most
reliable source of expensive imports, commissioned gear, and mediated orders
that the local market cannot normally support.

- Home Market: Absalom
- Route: Absalom -> Otari -> Meravon -> Absalom
- Profile: Outfitter
- Owner: Narin Alveri
- Terms: 20% prepaid; 5 gp + 5% courier delivery in `[[/gmroll 1d4+1]]` days
- Applicable Perks at 6th Level: `Reliable Teamsters`, `Warehouse Ties`,
  `Veteran Escort`
- Applicable Perks at 7th Level: `Reliable Teamsters`, `Warehouse Ties`,
  `Veteran Escort`, `Regional Trade Network`

When this caravan arrives in Otari on its regular circuit, use the following
6th-level state.

- Level 6
- Trade DC 26
- Arrives Each: `[[/gmroll 2d6+8]]` days
- Stays: `[[/gmroll 1d3]]` days
- Budget: `[[/gmroll 1120+(20d10-110)]]` gp

When the same caravan leaves Absalom on a heavier and better-supplied outbound
run, use the following 7th-level state.

- Level 7
- Trade DC 28
- Arrives Each: `[[/gmroll 1d6+8]]` days
- Stays: `[[/gmroll 1d3]]` days
- Budget: `[[/gmroll 1120+(20d10-110)]]` gp

This is the natural caravan to handle expensive commissions, high-end imports,
and mediated orders beyond what Otari can normally support on its own.

### Tawen Keefrow's Meravon Caravan

Tawen Keefrow, a 5th-level halfling merchant, runs a smaller but steady
Meravon line. In Otari, Tawen's caravan works best as a practical mixed
merchant: useful finished goods, modest imports, and enough flexibility to buy
interesting cargo without operating on Narin's scale.

- Home Market: Meravon
- Route: Meravon -> Otari -> Meravon
- Profile: General Trader
- Owner: Tawen Keefrow (male halfling 5)
- Terms: unknown
- Applicable Perks: `Reliable Teamsters`, `Broad Load Discipline`
- Level 5
- Trade DC 24
- Arrives Each: `[[/gmroll 1d4+6]]` days
- Stays: `[[/gmroll 1d2]]` days
- Budget: `[[/gmroll 700+(16d10-88)]]` gp

This caravan suits mixed lots, ordinary imports, and the kind of worthwhile
trade that exceeds what Otari's resident merchants can easily absorb but does
not justify waiting for the Absalom circuit.

### Garrik Vane's Diobel Buyers

Garrik Vane is a rowdy human buyer out of Diobel who runs a blunt, fast-moving
line between the river trade and the coast. His caravan is less refined than
the Absalom and Meravon lines, but it is quick to buy salable goods, harder to
bother with niceties, and willing to move on short margins if the cargo will
turn over quickly in Diobel.

- Home Market: Diobel
- Route: Diobel -> Otari -> Diobel
- Profile: General Trader
- Owner: Garrik Vane (male human)
- Terms: rough bargaining, fast payment, short stay
- Applicable Perk: `Warehouse Ties`
- Level 4
- Trade DC 22
- Buys up to 5th-level items
- Arrives Each: `[[/gmroll 1d10+12]]` days
- Stays: 1 day
- Budget: `[[/gmroll 420+(12d10-66)]]` gp

This line works well as a short-stay buyer that appears, makes a few loud deals,
loads up quickly, and heads back toward Diobel before the town fully knows what
it has sold.
