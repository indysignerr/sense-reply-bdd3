Create an interactive PowerPoint deck (.pptx, 16:9) that I will present on a large screen to a jury. Attached, if you can read them: Part 1 (Segmentation & ICP), Part 2 (Competitor analysis), Part 3 (Business model) and the team briefing. If a number below differs from an attachment, use the number below.

# Context
We are a student team at Albert School (BDD #3, case B1) acting as business consultants for Sense Reply, the Reply group company for IoT in energy. Sense Reply has built an AI-native platform: small computers on industrial sites ("edge gateways") run AI agents that manage solar panels, batteries and machines in real time. The jury is Sense Reply managers and professors. They want one clear recommendation: who to sell to, against whom, and how to make money. The business model is the centre of the deck; segmentation and competitors are the evidence.

Core line of the deck: "Reply invents the future, but others sell it."
Our answer: "Reply stays a consulting firm, but stops starting from zero on every project and gets paid every year for what it has already built."

# Rules that must never be broken
- Everything in English. Plain words, short sentences, no jargon without a one-line explanation.
- Never call the contract a "licence". Say "managed service" and "white-label platform fee".
- Never promise guaranteed savings. The success bonus is "upside only, paid on measured savings".
- Do not present Reply as a cheap software vendor. Custom projects stay; the managed service comes on top.
- No Reply or Sense Reply logo. Footer on every slide: "Albert School BDD #3 · Team prototype · Estimates, not guarantees".
- Every slide title states a conclusion, not a topic. One message per slide.
- Every number has its source in the speaker notes.

# Interactivity (use internal slide links, no macros)
1. Slide 2 is a home screen with six large clickable tiles: Clients, Competitors, Today's model, Our model, Numbers, Roadmap. Each tile jumps to its section.
2. A slim navigation bar at the top of every slide with the same six section names plus "Home" and "Q&A". The current section is highlighted. Each name is a link.
3. Scenario switches built as linked duplicate slides, so a click looks like a toggle:
   - Plant gain slide in three versions: Cautious / Base / Optimistic, with three buttons on each.
   - Three-year slide in two versions: Today / Two-speed model, with two buttons on each.
   Use the Morph transition between these versions so bars grow and numbers change smoothly.
4. "Details" buttons that jump to an appendix slide, and a "Back" button on each appendix slide that returns to the slide it came from.
5. A Q&A slide: a grid of eight likely jury questions. Each question links to its own answer slide with a "Back to questions" button.
6. A "Live demo" button on the plant gain slide and on the last slide, linking to: https://claude.ai/artifact/QL1t3dGBcL4TFUYGn9bzKT

# Design
Light and clean, built for a large screen: titles 34 pt or more, body 20 pt or more, nothing below 16 pt, lots of white space, at most 30 words of body text per slide outside tables.
Colours: background #F5F8FA, cards #FFFFFF, text #17232E, secondary text #667482, primary #0B7F76. Data colours in this fixed order: amber #E2A336, teal #1F9E8F, blue #4C86E0, pink #D9668A. Text is never coloured with a data colour.
Fonts: Sora for titles and big numbers, Plus Jakarta Sans for text; fall back to Segoe UI or Calibri if they are not available.
Charts are native PowerPoint charts with direct labels, thin gridlines and a legend. Rounded cards, no clip art, no stock photos.

# Slides
1. Title: "Reply invents the future. Here is how it sells it." Subtitle: go-to-market and business model for the AI-native energy platform.
2. Home screen (see Interactivity).
3. Our answer on one page: start in Italy with multi-site energy-intensive manufacturers, scale through partners, with a two-speed model. Four big numbers: €52k gained per plant per year · €54k per account per year for Reply · 25 accounts in 3 years · revenue per consultant €124k → €303k.

Section: Clients
4. "Italian companies pay the most for electricity": bar chart, €/MWh, H1 2025: Italy 278, Germany 242, France 183, Spain 171, EU average 216.
5. "Only 3 of 12 segments score above 4 out of 5": ranked bars. Large multi-site energy-intensive manufacturers 4.30 · Fleet operators (ESCOs, aggregators, battery integrators) 4.20 · Utilities and energy retailers 4.10 · Cold-chain logistics 3.45 · Data centres 3.45 · EV fleet depots 3.40 · Mid-sized manufacturers 3.35 · Water utilities 3.35 · Microgrids 3.25 · Multi-site retail 3.20 · Commercial real estate 3.10 · Energy communities 2.20.
6. "Our ideal customer": three cards. Primary: Northern Italian manufacturer (food and beverage, paper, chemicals, rubber and plastics, ceramics and glass), 2 to 10 plants, 5 to 50 GWh a year, solar on the roof, flexible loads; the CFO signs, the energy manager champions, IT can block. Secondary 1: fleet operators with 50+ client sites. Secondary 2: cold-chain operators with 3 to 20 cold warehouses.
7. "About 860 named targets; 25 is a realistic three-year win": funnel. 5,253 companies on Italy's official energy-intensive list → 3,011 in five sectors → about 1,730 medium or large in Northern Italy → about 860 fit the profile → about 25 won in 3 years. In euros per year: €162M → €93M → €46M → €1.9M.
8. "Four dates make Italy urgent now": timeline. Feb 2026: sites can earn from flexibility through aggregators. Oct 2027: certified energy management system mandatory above about 23.6 GWh. Dec 2027: EU AI Act high-risk rules for critical infrastructure. Sep 2028: tax incentive window closes. Germany follows in phase 2 (grid-fee reform in 2029).

Section: Competitors
9. "Everybody sells a piece. Nobody sells the neutral brain": five families in a table. Industrial incumbents (Siemens, Schneider, ABB) own hardware · Cloud and edge platforms (AWS, Azure, Barbara) own the plumbing, about $0.16 per device per month · Utility-owned platforms (Next Kraftwerke/Shell, gridX/E.ON, Enel X) own market access · Battery makers' software owns one asset, included in the price · Status quo: fixed rules and spreadsheets.
10. "The top-right corner is empty": 2×2 map. X: openness (locked to own hardware → vendor-neutral). Y: intelligence on site (fixed rules → autonomous agents). Sense Reply alone top right; Barbara closest but built for grid operators.
11. "The neutral seat is empty": energy sellers bought the independent platforms (Centrica–REstore 2017, Shell–Limejump and sonnen 2019, Shell–Next Kraftwerke 2021, E.ON–gridX 2021–22). Counter-example: Kraken spun out of Octopus at $8.65bn in 2025. Line: "Your clients, your data, your brand. We sell no electricity."
12. "The real competitor is free": yesterday's innovations are now bundled or sold for cents (solar monitoring, peak shaving with a battery, device management, demand response). So never sell a single feature. In Italy most sites have solar but no battery: only 91 MWh of commercial storage connected in Q1 2026.

Section: Today's model
13. "How Reply sells today": three steps. Pilot of about 3 months, often free → 3-year contract for the whole business, best effort, no guaranteed result → revenue from the contract and integration, every project custom.
14. "What does not work": value leaks to copycats · growth needs more consultants · free pilots with no commitment · a big jump from one site to the whole company · only large clients can afford it · revenue after year 3 is uncertain. And what to keep: the pilot, integration, customisation for large clients, the innovation identity.

Section: Our model
15. "Two speeds, one platform": two columns. Frontier: new capabilities, co-innovation with large groups, sold by Reply, project fee. Mature: proven agents packaged as a managed service, sold plant by plant and through partners, yearly fee plus bonus. Lifecycle below: Explore → Prove → Package → Scale.
16. "A typical plant gains about €52k a year" (three linked versions). Plant: 5 GWh a year, €1.39M bill at €278/MWh, 1 MWp of solar, flexible loads, no battery. Stacked bar and four lines:
    - Cautious: solar €12k · moving consumption €7k · flexibility €3k · peaks €1k · total €24k (1.7% of the bill)
    - Base: solar €20k · moving consumption €23k · flexibility €7k · peaks €3k · total €52k (3.8%)
    - Optimistic: solar €27k · moving consumption €52k · flexibility €10k · peaks €4k · total €94k (6.8%)
    Note: a study of 83 plants measured 3 to 4% a year. "Live demo" button.
17. "The client keeps two thirds, Reply takes one third": pricing table. Conditional pilot €20k at cost, credited if the client signs · Set-up €30k first plant, €12k each further plant · Managed service €10k per plant per year · Success bonus 15% of measured savings, upside only · White-label platform fee €4k per plant per year, minimum 25 plants · Co-innovation project about €100k a year with large groups. Below: per plant in the base case, gain €52k, paid to Reply €18k, kept by the client €35k.
18. "The pilot becomes a commitment": conditional pilot on one page. One plant, 3 months · baseline and targets agreed in writing first · €20k at cost · if targets are met, the client signs and the fee is credited · if not, no obligation · Reply promises best effort and a measured result, no guaranteed saving.
19. Business Model Canvas, nine blocks, with what is kept from today in grey and what is new in teal. New items: mid-sized manufacturers through partners, fleet operators, managed service per plant, success bonus, white-label platform fees, packaged agents, partner enablement, pilot data as benchmarks.
20. "Who sells to whom": Large groups → Reply directly, co-innovation. Typical multi-site manufacturers → Reply directly, plant by plant. Mid-sized manufacturers → partners. Fleet operators → white-label platform. Aggregators provide market access.

Section: Numbers
21. "What one account brings": typical account (3 plants, one more each year) €54k a year · lighthouse account (large group, 10 plants) €247k a year · one partner (25, 50, then 75 plants) €200k a year. Message: one partner is worth almost four direct accounts, with no pilot for Reply to run.
22. "Same sales effort, more than double the revenue per consultant" (two linked versions, Today / Two-speed). Chart: revenue per year. Today €0.5M, €1.1M, €1.7M. Two-speed €0.6M, €1.6M, €3.0M, stacked by projects, yearly service and bonus, partner fees. Table: revenue over 3 years €3.3M vs €5.2M · recurring share in year 3 34% vs 65% · accounts signed 16 vs 25 · plants on the platform 57 vs 300 · people needed 13.4 vs 10.0 · revenue per person €124k vs €303k · pilot days given for free 1,760 vs 0.
23. "Partners are the engine, not a side channel": 25 direct accounts bring about €1.9M a year; partners carry 244 of the 300 plants and 32% of year-3 revenue.

Section: Roadmap
24. "Three phases in 36 months": Prove (0–6 months): conditional pilots in Northern Italy, one lighthouse account, first partner. Package and partner (6–18): package the first agents, second plants go live, two more partners. Scale (18–36): partners carry the mid-market, 25 accounts, 6 partners, about 300 plants, prepare Germany.
25. "Four numbers to steer by, and what would prove us wrong": KPIs: pilot conversion 50% · 3 plants per account after 3 years · recurring share 65% · revenue per person €300k. Kill criteria within 6 months: conversion below 30%, measured gain below 2% of the bill, no partner signed.
26. "Risks we see, and our answer": gain lower than estimated → the pilot measures before any commitment · partners build their own tool → neutrality, speed, audit trail · consultants fear fewer billable days → integration and co-innovation stay · AI controlling machines → fixed safety limits stay in control, every decision is logged.
27. Closing: the answer in one sentence, the four big numbers, next steps for the next 90 days, "Live demo" button.

Q&A section
28. Question grid with eight questions, each linked to an answer slide:
    - Why pay a bonus if you guarantee nothing? → Upside only. The client pays more only when savings are measured.
    - Does packaging kill Reply's innovation identity? → No. The mature speed funds the frontier speed.
    - Why would a partner not build its own? → Neutrality, time to market, audit trail ready for the AI Act, no team to maintain.
    - What if a battery maker gives its software away? → We do not sell battery optimisation. We run the whole site, and most Italian sites have no battery.
    - Why Italy first? → Highest prices, emptier field, home market. Germany is phase 2.
    - Is it safe to let AI control energy assets? → Agents plan; fixed controls enforce safety limits; every action is logged.
    - How is this different from today? → Paid conditional pilot, plant-by-plant growth, recurring revenue, partners.
    - Where do your numbers come from? → Team documents, public sources, and declared hypotheses. All can be changed in the live simulator.

Appendix (reached through "Details" buttons)
A1. Full scoring table of the 12 segments on 8 criteria. A2. Competitor matrix: 11 players on 9 dimensions. A3. How the plant gain is calculated, line by line. A4. Assumptions behind the three-year numbers. A5. Sources.

# Speaker notes
For every slide write 3 to 5 sentences I can say aloud, in plain English, and list the sources of the numbers. Mark every team hypothesis as "our assumption".

# Before you finish
Check that every link works in slideshow mode, that every appendix and answer slide has a working Back button, that no slide uses the word "licence" or "guaranteed", and that all numbers match this prompt.
