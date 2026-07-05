ChatGPT























Here's how I would structure it as a single subsystem chapter. I would deliberately keep Assess Value/Negotiate as its own exploration action and have the caravan rules reference it rather than duplicate it. That way, if you later tweak negotiation percentages, every merchant—not just caravans—updates automatically.

Caravan Trading System
Overview
Caravans are mobile businesses that travel between settlements purchasing goods, transporting cargo, and reselling it elsewhere. Unlike ordinary merchants, caravans possess their own wealth, experience, trade expertise, and business growth. Over time, successful caravans become wealthier, establish wider trade networks, and gain access to larger markets.

The caravan system serves two purposes:

It determines how much wealth a caravan has available to purchase goods from the PCs.

It simulates the caravan's continued business after leaving, allowing recurring caravans to grow naturally through successful trade.

Caravan Statistics
Every caravan has the following statistics.

Statistic	Description
Level	Overall business size, reputation and logistical capability.
Mercantile Lore	Skill modifier used for trade negotiations and commercial decisions.
Trade DC	10 + Mercantile Lore modifier. Used whenever the caravan resists haggling.
Liquid Gold	Coins immediately available for purchasing goods.
Caravan XP	Experience gained from successful trade expeditions.
Caravan Level Progression
Level	Mercantile Lore	Trade DC	Liquid Gold
3	+10	20	/r 280+(10d10-55)
4	+12	22	/r 420+(12d10-66)
5	+14	24	/r 700+(16d10-88)
6	+16	26	/r 900+(18d10-99)
7	+18	28	/r 1120+(20d10-110)
8	+20	30	/r 1600+(24d10-132)
9	+22	32	/r 2400+(30d10-165)
10	+24	34	/r 3600+(36d10-198)
Roll Liquid Gold whenever the caravan first appears or after it has completed a trade expedition.

Liquid Gold represents immediately available coinage. It does not represent the caravan's total assets, wagons, merchandise, credit, or property.

Purchasing Goods
Caravans purchase items using the Assess Value / Negotiate exploration activity.

Friendly caravans generally negotiate using the item's Level DC.

Professional caravans, merchant houses, guild factors, and organized businesses usually haggle using their Trade DC instead.

If the caravan cannot afford the negotiated price, it simply cannot purchase the item.

Caravan Cargo
After purchasing goods, record only the amount of gold invested.

Do not track individual crates or inventories unless they are story-important.

Example:

Cargo	Purchase Cost
Player goods	520 gp
Trade goods	340 gp
Total cargo investment: 860 gp

Trade Expedition
A trade expedition represents travel between settlements and usually lasts between 3 and 14 days, depending on the route.

Upon reaching its destination, resolve the expedition.

Step 1 — Determine Trade Level
The Trade Level equals the lower of:

Caravan Level

Settlement Level

This represents the largest market the caravan can effectively exploit.

Step 2 — Trade Check
Attempt a Mercantile Lore check against the standard Level DC for the Trade Level.

Mercantile Lore
vs
Level DC
Step 3 — Determine Profit
Result	Profit
Critical Success	+25% of invested cargo
Success	+10% of invested cargo
Failure	No profit
Critical Failure	Lose 10% of invested cargo
Add the resulting profit directly to the caravan's Liquid Gold.

Caravan Experience
Successful trade expands business connections, reputation and logistics.

Result	XP Earned
Critical Success	150 XP
Success	100 XP
Failure	50 XP
Critical Failure	25 XP
A caravan levels up after accumulating 1,000 XP.

Any excess XP carries over.

Caravan Improvements
Whenever a caravan gains a level:

Increase Mercantile Lore according to the progression table.

Increase Trade DC.

Roll new Liquid Gold using the new level.

Expand the caravan's business network and number of employees as appropriate.

Higher-level caravans naturally represent larger organizations with additional guards, wagons, contracts, warehouses, and established trade routes.

Market Conditions
The GM may adjust selling prices before negotiation.

Market Condition	Modifier
Weak demand	–10%
High demand	+10%
Local demand for uncommon goods	+15%
Collector purchasing rare or unique items	+25% or more
These modifiers are applied before any negotiated adjustments.

Market Saturation
Small settlements cannot absorb unlimited quantities of expensive merchandise.

The GM may reduce trade profits if the caravan attempts to sell significantly more valuable goods than the destination settlement could realistically purchase.

As a guideline:

Settlement	Maximum Comfortable Trade
Village	Small quantities of common goods
Town	Moderate cargo
City	Large cargo
Metropolis	Effectively unrestricted
Trade Events (Optional)
Roll once during each expedition.

d20	Event
1–2	Bandits or monster attack. Lose 10% cargo.
3–4	Tariffs, tolls or bribes. Lose 5% cargo value.
5–6	Delays. No profit modifier.
7–14	Uneventful journey.
15–17	Strong demand. Increase profit by 5%.
18–19	Exceptional market. Increase profit by 10%.
20	Trade boom. Increase profit by 20% and gain +50 XP.
Recurring Caravans
A caravan that repeatedly visits the same settlements should retain:

Current level

Current XP

Current Liquid Gold

Reputation with the PCs

Previous negotiations

A caravan remembers previous deals. Once a specific item has been negotiated, the same caravan will not renegotiate its purchase price for that item again.

I think one design change would improve the entire subsystem
I would remove "Trade Bonus DC" from the table and simply call it Trade DC everywhere. "Trade Bonus DC" mixes two different concepts (a bonus and a DC). The cleaner presentation is:

Level	Mercantile Lore	Trade DC
Then throughout the rules, consistently refer to Trade DC. It reads much more like an official PF2e subsystem and avoids unnecessary terminology.


Yes good idea

I also have one additional suggestion that I think will make the subsystem feel much more like an official PF2e subsystem.

Rename "Liquid Gold" → Working Capital
"Liquid Gold" is understandable, but Working Capital better describes what the number actually represents: money currently allocated for commerce.

For example:

Working Capital represents the coins, letters of credit, and readily available assets the caravan has available to purchase goods. It doesn't represent the caravan's total wealth, wagons, buildings, or merchandise.

Then your table becomes:

Level	Mercantile Lore	Trade DC	Working Capital
3	+10	20	/r 280+(10d10-55)
4	+12	22	/r 420+(12d10-66)
5	+14	24	/r 700+(16d10-88)
6	+16	26	/r 900+(18d10-99)
7	+18	28	/r 1120+(20d10-110)
8	+20	30	/r 1600+(24d10-132)
9	+22	32	/r 2400+(30d10-165)
10	+24	34	/r 3600+(36d10-198)
I also recommend a couple of terminology changes for consistency:

Trade Expedition → Trade Journey (reads more naturally and can cover anything from a short route to a long caravan run).

Trade Level → Market Level. Since you're taking the lower of the caravan level and the destination settlement level, you're really determining the size of the market, not the quality of the trade.

That gives you:

Determine Market Level.

Attempt a Mercantile Lore check against the Level DC of the Market Level.

Apply profit.

Gain XP.

I would also simplify the growth section. Instead of saying "roll new Working Capital using the new level," I'd say:

Whenever a caravan completes a successful trade journey or first appears in the campaign, roll its Working Capital. A caravan that has recently suffered losses or made major investments may have less Working Capital at the GM's discretion.

That better explains why the amount changes. It's not magically becoming richer because it leveled; it's because it has completed more business and reinvested its profits. It also lets you reroll its available funds each time the PCs encounter it without implying the caravan literally has exactly that amount at all times.

Overall, I think this has evolved into a cohesive subsystem. It no longer feels like a collection of house rules—it feels like something that could plausibly appear in a Pathfinder subsystem chapter.


Good idea apply it

I would revise the subsystem as follows. These changes improve terminology, make the economy feel more natural, and better explain why caravan wealth changes over time.

Caravan Trading System
Overview
Caravans are mobile businesses that travel between settlements purchasing goods, transporting cargo, and reselling it elsewhere. Unlike ordinary merchants, caravans possess their own working capital, trade expertise, business reputation, and experience. Over time, successful caravans expand their networks, increase their purchasing power, and establish themselves as prominent trading enterprises.

This subsystem serves two purposes:

It determines how much wealth a caravan has available to purchase goods from the PCs.

It simulates the caravan's commercial growth between encounters, allowing recurring caravans to develop naturally over the course of a campaign.

Caravan Statistics
Every caravan has the following statistics.

Statistic	Description
Level	Overall size, reputation, logistics, and commercial capability.
Mercantile Lore	Skill modifier used for negotiations, market analysis, and trade operations.
Trade DC	Equal to 10 + Mercantile Lore modifier. Used whenever the caravan haggles over prices.
Working Capital	Coinage, letters of credit, and readily available assets available to purchase goods. This doesn't represent the caravan's total wealth, wagons, merchandise, or property.
Caravan XP	Experience earned through successful trade journeys.
Caravan Level Progression
Level	Mercantile Lore	Trade DC	Working Capital
3	+10	20	/r 280+(10d10-55)
4	+12	22	/r 420+(12d10-66)
5	+14	24	/r 700+(16d10-88)
6	+16	26	/r 900+(18d10-99)
7	+18	28	/r 1120+(20d10-110)
8	+20	30	/r 1600+(24d10-132)
9	+22	32	/r 2400+(30d10-165)
10	+24	34	/r 3600+(36d10-198)
Roll a caravan's Working Capital whenever it first appears in the campaign or after it has completed a trade journey.

The result represents the funds currently available for purchasing goods and paying expenses. Previous investments, successful sales, unexpected losses, taxes, wages, or other business costs are already reflected in this amount.

Purchasing Goods
Caravans purchase goods using the Assess Value / Negotiate exploration activity.

Friendly merchants generally negotiate against the item's Level DC.

Professional caravans, merchant houses, guild factors, and organized businesses usually negotiate using their Trade DC.

A caravan cannot purchase goods whose negotiated value exceeds its current Working Capital.

Cargo
Track only the caravan's investment, not every individual crate or wagon unless doing so is important to the story.

Example:

Cargo	Purchase Cost
Goods purchased from PCs	520 gp
Other trade goods	340 gp
Total Cargo Investment: 860 gp

Trade Journey
A trade journey represents transporting goods between settlements and usually requires 3–14 days, depending on distance, terrain, and weather.

After arriving, resolve the journey.

Step 1 — Determine Market Level
The Market Level equals the lower of:

the caravan's Level

the destination settlement's Level

This represents the largest market the caravan can effectively exploit.

Step 2 — Trade Check
Attempt a Mercantile Lore check against the standard Level DC for the Market Level.

Mercantile Lore
vs
Market Level DC
Step 3 — Determine Profit
Result	Profit
Critical Success	+25% of Cargo Investment
Success	+10% of Cargo Investment
Failure	No profit
Critical Failure	Lose 10% of Cargo Investment
Add the resulting profit to the caravan's available wealth.

Caravan Experience
Trade success also expands the caravan's commercial reputation and network.

Result	XP Earned
Critical Success	150 XP
Success	100 XP
Failure	50 XP
Critical Failure	25 XP
A caravan gains a level after accumulating 1,000 XP. Any excess XP carries over.

Caravan Growth
Whenever a caravan gains a level:

Increase its Mercantile Lore according to the progression table.

Increase its Trade DC.

Expand its trade network, employees, wagons, contracts, and reputation as appropriate.

Leveling reflects the gradual growth of a successful business rather than a sudden increase in wealth.

Refreshing Working Capital
Whenever a caravan first appears after completing one or more trade journeys, roll its Working Capital using its current level.

The GM may adjust the result if circumstances warrant. For example:

A caravan that recently suffered bandit attacks or poor markets may have reduced Working Capital.

A caravan that completed several exceptionally profitable journeys may have additional Working Capital.

Major investments, taxes, wages, or purchasing new wagons may temporarily reduce available funds.

This roll represents only the caravan's immediately available purchasing power at the time it is encountered.

Market Conditions
Before negotiation, determine whether local market conditions affect demand.

Market Condition	Modifier
Weak demand	–10%
Strong demand	+10%
Local demand for uncommon goods	+15%
Collector seeking rare or unique goods	+25% or more
Apply these modifiers before any negotiated adjustments.

Market Saturation
Settlements can absorb only a limited quantity of valuable merchandise.

If the caravan attempts to sell significantly more valuable goods than the destination market can reasonably purchase, the GM should reduce profits appropriately.

As a guideline:

Settlement	Typical Market Capacity
Village	Small quantities of common goods
Town	Moderate cargo
City	Large cargo
Metropolis	Effectively unlimited
Trade Events (Optional)
Roll once during each trade journey.

d20	Event
1–2	Bandits or monsters. Lose 10% of Cargo Investment.
3–4	Tariffs, tolls, or bribes. Lose 5% of Cargo Investment.
5–6	Delays. No modifier.
7–14	Uneventful journey.
15–17	Strong market. Profit +5%.
18–19	Exceptional demand. Profit +10%.
20	Trade boom. Profit +20% and gain +50 XP.
Recurring Caravans
Recurring caravans should retain:

Level

Caravan XP

Current Working Capital (until refreshed)

Trade reputation

Relationships with the PCs

Caravans remember previous business dealings.

Unless market conditions have substantially changed, a caravan won't renegotiate the purchase price of the same item more than once. This prevents repeated attempts to improve the same transaction while encouraging players to seek different buyers or wait for changing markets.

I think this version reads much closer to an official PF2e subsystem. It uses consistent terminology ("Trade DC," "Working Capital," "Market Level," "Trade Journey"), separates narrative concepts from mechanics, and clearly explains why caravans' available funds fluctuate without implying that their total wealth magically changes. It should also integrate cleanly with your Assess Value / Negotiate exploration activity.


