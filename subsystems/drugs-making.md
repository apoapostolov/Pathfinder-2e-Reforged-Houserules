<!-- markdownlint-disable MD001 MD013 MD025 MD033 -->

# Drugs

## The ABC of Breaking Bad

1. Find creatures, plant life, or minerals that might contain the chemical makeup of drug components, and **Collect** samples from them. You will likely end up with samples with level lower than the creature you collect from.
2. Identify the drug components contained in the samples by **Extracting** from samples. You will likely end up with drug component formulas weaker than the samples you collected from.
3. **Refine** drug components until they reach your desired level of purity. You will probably need to make up to two Refine processes to take the drug components to a level of purity as found naturally. You may keep refining, but the risk of contaminating the samples increases.
4. **Cook** drug components (base + enhancer + solution) by combining compatible elements. This will result in a final stable drug formula and a small batch (about 20 doses, enough for seeding distribution).
5. **Congratulations**! **You have a new drug on your hands!** You can now figure out how to sell the drugs, how to mass produce the source of components as well as the drug, how to distribute, how to evade off enemy criminal organizations that will come after your newfound popularity, etc.

## Drug Component Properties

Each Drug Component has the following properties:

- **Type**: Each drug component can be one or several types: **Base, Enhancer, Solution**. You need one drug component with a different name and of each type when Cooking a drug. Each drug component may have multiple types (i.e. can be used as both Base or Solution).
- **Tags**. Each component has a number of descriptor tags, explained below.
- **Effect or Drug Level.** This is the level of the drug component. It also defines the DC for all Extract and Refine checks. When a drug is cooked, the highest Effect among all drug components used becomes the effective level of the final drug. Enhancer drug component has modifiers to Effect (i.e. an enhancer with +1 Effect is added to the base drug component effect of 4, for a total of 5). The final level of the drug defines the DC of the drug when ingested.
- **Toxicity Level**. This is the level of the negative and dangerous side-effects of a drug component, and the final drug when cooked. The typical value of Toxicity for dangerous and lethal dirty drugs is 3, and most components with toxicity of 4 or higher need to be refined before considered usable by drug makers. Base drug components usually have a static Toxicity value. Enhancer and Solution drug components have modifiers to the Toxicity (i.e. an enhancer with +2 toxicity is added to the base drug component toxicity of 5, for a total of 7). If the Toxicity level of a drug is higher than the Effect Level, the drug produces a nasty trip and the drug may be prone to overdosing and deadly withdrawal.
- The Drug hazard (as will be revealed when a drug is Cooked) will have a new final stage
  - **Max Stage +1** death (a Fortitude save to fall unconscious on success)
- The Drug Addiction (Gamemaster Guide, pg. 120) gains stages 5 and 6 as follows:
  - **Stage 5** fatigued, drained 3, sickened 3, and stupefied 3 (1 day); **Stage 6** death

## Tags

Each Drug Component can have one of the following tags that define its effect when ingested. The final drug collects the tags of all its drug components, and if multiple components have the same tag, the tag of the final drug gains a value equal to the number of same tags among all components (ex: a base with Stimulant and enhancer with Stimulant would create a drug with Stimulant 2). Drugs with a tag with a value of 3 or more may be lethal or degenerative even in limited dosage.

- **Stimulants**: These are substances that increase the activity of the central nervous system, causing increased alertness, energy, euphoria, heart rate, and blood pressure.
- **Depressants**: These are substances that decrease the activity of the central nervous system, causing relaxation, sedation, reduced anxiety, impaired memory, and coordination.
- **Hallucinogens**: These are substances that alter the perception of reality, causing distorted sensory experiences, altered mood and cognition, and sometimes psychosis.
- **Magical**: These are substances that connect the mind with specific magical sources, causing an influx of magical energy into the psyche, allowing raw magic to influence the body. Drug Components with **Magical** tag may have other tags typical to magic (i.e. **Fire, Evil, Death, Illusion,** etc.)

In addition to these tags, each Drug Component has a two-letter tag consisting of the letters A, B, X, and Y. For example [AX] or [YX]. These chemical connections represent compatibility with another type of drug components placed before or later in the order of synthesis, that is base enhancer then solution, like domino blocks. For example, an enhancer with tag [AX] is only compatible with a base that has a tag ending with A, and a solution with has a tag starting with X. Note that many drug components may take different roles (i.e. can be a base or an enhancer) and the letters can also be changed through Refining, so there are many ways to combine drug components.

## Exploration Actions

### Collect

[Exploration]

You spend 10 minutes extracting parts from a creature or an object that might be useful to extract drug components. Make a Medicine, Nature or Surgery Lore check at a DC based on the level of the creature or the object. You can collect from a source only once, as any other remains will be unusable (the DM may rule otherwise for large inorganic sources, but even so they would allow only one attempt per character from such sources).

**Critical Success** You gain a sample of level equal to the CL of the creature. You gain a +1 item bonus to attempt to Extract from that sample (plus an additional +1 for each proficiency tier of used skill to Collect above Trained, up to +4).

**Success** You gain a sample of level equal to the CL of the creature minus 1.

**Failure** You gain a sample of level equal to the CL of the creature minus 4.

> There is a reason you may want to have multiple samples as Extract and Refine may cause contamination and loss of a sample. Each sample has its own level based on the degree of success when it was collected.

### Extract

[Exploration]

**Requirements** Alchemical Crafting; Access to an alchemical lab or alchemist’s tools (time is doubled when using only an alchemist’s tools)

**Prerequisite** a collected extract

You spend one hour conducting various alchemical experiments trying to identify contained substances that may be useful to the concoction of drugs. In a full day of downtime, you can work with up to 8 different batches of samples, and you make a separate roll for each. Make a Crafting check against a DC based on the sample.

**Critical Success** Like success, but the drug component’s Effect rating is equal to the sample. You gain a +1 item bonus for all attempts to Refine that Component. The bonus increases to +2 if you are a Master in Crafting or better.

**Success** If the sample contained any drug component, you learn its properties and the formula for that component with an Effect rating equal to the sample level minus 1. You also gain enough samples of the component for the purpose of experimental drug synthesis in individual batches (you do not need to count any batches while you experiment, only when you start to mass produce). You may still collect more samples in the future when you start producing the drug in larger quantities.

**Critical Failure** You contaminate the samples and make them unusable for future attempts to Extract from them. The sample is lost.

**Special** Each attempt to Extract the same extract increases the DC of all follow-up attempts by 1.

### Refine

[Downtime]

**Requirements** Alchemical Crafting; Access to alchemical lab or alchemist’s tools (time is doubled when using only an alchemist’s tools)

**Prerequisite** an extracted drug component

You spend one day to make numerous experiments aimed to improving the quality of a single drug component. Pick one desired effect and attempt a hard (DC + 2) Crafting check at a DC based on the Effect rating of the drug component. Add cumulative +1 to the DC for each refining process after the second one.

- Increase the Effect of a drug component by 1.
- Lower the Toxicity of a drug component by 1.
- Change one letter of its compatibility tag to any other letter among A, B, X, and Y.

**Critical Success** You may pick an additional effect different from the one you initially picked. Make the two changes to the drug formula and its extracts.

**Success** You make a change to the drug formula and its extract and its extracts.

**Critical Failure** You contaminate the samples and make them unusable for future attempts to Extract from them. The sample is lost.

**Special** Each successful attempt to Refine the same drug component increases the DC of all follow-up attempts by 1. After the fifth successful attempt the cumulative increase becomes 2 for each follow-up attempt.

### Cook

[Downtime]

**Requirements** Alchemical Crafting; Access to an alchemical lab or alchemist’s tools (time is doubled when using only an alchemist’s tools)

**Prerequisite** three extracted drug components with different names; each should be a different type between base, enhancer, and solution; each drug component must have a compatible two-letter tag with the next or previous component in the drug chain (base > enhancer > solution)

You spend four days cooking a stable drug solution. Make a hard (DC + 2) Crafting check at a DC based on the highest Effect among all drug components.

**Critical Success** Like success, but the drug substance level is one higher than the highest Effect value among all drug components. You also gain a +1 item bonus to all standard Crafting and Mass Produce checks as you discover a highly optimized process to do so.

**Success** You successfully isolate a stable drug substance with a level equal to the higher Effect value among all drug components. You learn the formula to make these drugs using the standard Crafting process (alchemical crafting is still needed for the process) in small batches, as well to Mass Produce large distribution batches.

**Critical Failure** You contaminate the samples and make them unusable for future attempts to Extract from them. One of the drug components (1d6: 1,2 the base, 3,4 the enhancer, 5,6 the solution) is lost.

### Craft Drugs

[Downtime]

To be revealed when the party Cooks at least one drug.

### Mass Produce

[Downtime]

To be revealed when the party Cooks at least one drug.

## Pricing and Distribution

The following list of published drugs lets you put your own creations in perspective.

[bookmark](https://app.notion.com/p/d078784364994affb74ebb05ce30c2da#cdab14b0f7264279aad6df7f7bdb9931)

In the world of Golarion, most drugs available among poor people and dregs of society range between levels 1 and 2. These drugs often have a Toxicity of 3 and higher and are lethal for prolonged use and their withdrawal often risks death as well.

Folk who can afford comfortable lifestyles in the urban regions and who can pay extra for quality drugs have access to drugs of effect levels 3 and 4, and their toxicity rarely goes over 3, thus being borderline dangerous only after years of consumption, and withdrawal does not pose death risks.

Drugs of level 5 and onward are available to nobility and merchants, or used for specific purposes (such as combat drugs given at gladiatorial matches to ensure performance at a cost). Any drug of level 6 and above is considered to be a “novelty drug” and is subject of great interest by all criminal organizations.

> **But how do I mass produce when the creatures I collected samples are long dead?** You cannot, but you have the formula and in the future, you may seek other locations where such creatures exist and capture them for mass production. Or you may sell the formula to criminal organizations or shady consortiums who may take on mass production themselves while you pocket a hefty sum. These are often stories left beyond the scope of a single adventure path.

## Known Components

| Name | Type | Traits | Lv | Chain | Toxicity | Effect | Toxicity and Effect |
| --- | --- | --- | --- | --- | --- | --- | --- |
| pesh | Base | Stimulant | 2 | AA | 3 |  | item bonus vs fear, temp hp |
| qat | Base, Enhancer | Stimulant | 2 | AX | +2 |  | item bonus for Reflex saves |
| shiver oil | Enhancer, Solution | Hallucinogen | 3 | AY | +1 | +1 | improve result by 1 stage vs fear |
| blood dew | Solution | — | 2 | YA | -2 | -1 | — |
| darkwood bark | Enhancer | Depressant | 2 | BX | — | +1 | **+1 to Refine**, pain endurance (bludgeoning resistance half level, rounded down) |
| calmleaf extract | Base, Solution | Depressant | 1 | XX | -1 | — | **+1 to Refine**, Dillutant (lowers the Base level by 1) |
| black pudding ooze | Base | Depressant | 6 | BX | 9 | — | **+1 to Refine**, Acidic dissolution of internal organs while skin numbing (slashing, piercing resistance half level, rounded down) |
| malevolent fey flesh | ??? | ??? | 8 | ??? | ??? | ??? | ??? |
| basilisk blood | ??? | ??? | 5 | ??? | ??? | ??? | **+2 to Extract** |
| wyrmwood essence | Base | Hallucinogen | 5 | AX | 4 | — | **+1 to Refine.** See through thin items (paper, cloth, skin). See the particle consistence of small and tiny objects. Become stupefied 2 and fatigued after overdose. |
| shroom crystalshine | Base, Solution | Hallucinogen | 6 | AY | 5 or -2 | +1 | **+1 to Refine.** Feel the air as a semi-solid consistency, experience lower gravity. You take 10 feet less for each 50 feet of falling. You gain resistance 3 against all falling damage. Become drained 1 and featigued after overdose. |
| crystal veil | Base, Enhancer | Hallucinogen | 4 | BA | 3 | -1 | **+1 to Refine.** Experience a floating sensation and powerful pain numbing sensations. May cause a panic attack of infinite falling followed by a spike of manic happiness, which is exhilarating and addictive. Become blind for 1 minute and fatigued after overdose. |
| umbral elixir | Enhancer | Depressant | 4 | BY | 5 | -1 | **+1 to Refine.** Experience powerful desires to feel soil or earthlike substances and have experiences of sinking and becoming one with the earth. Has a chance to develop temporary quasi-telekinetisis with lower forms of life (insects, plants, and proto forms of life). Become drained 1 and fatigued after overdose. |
