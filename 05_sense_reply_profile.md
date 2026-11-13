# Sense Reply — company profile and what it means for our recommendation

> Status: **working draft, 13 Nov 2026**. Built from public sources and from what Sense Reply told the team.
> ✅ = found in a public source. ⚠️ = unverified, conflicting or from a weak source. 💬 = said by Sense Reply to the team.
> We could not open reply.com or aws.amazon.com from our tool (network block). Facts from those sites come from search-result extracts, not from reading the full pages.

---

## 1. Identity card

| Item | Fact | Status |
|---|---|---|
| Legal entity | Sense Reply S.r.l., Corso Francia 110, Turin (Reply's headquarters address) | ✅ |
| Founded | 2017 | ✅ |
| Parent | Reply S.p.A., listed in Milan. 2025: revenue €2,483.6M (+8.0 %), EBITDA €467.6M, net profit €250.9M | ✅ |
| Revenue | About €12M: €12.4M in 2023, €11.9M in 2024. One source lists €14.9M for 2025 | ⚠️ business-register aggregators, they disagree |
| Profit | About €2.3M (year unclear: 2023 or 2025 depending on the source) | ⚠️ |
| Employees | 76 to 80 in 2025 (42 listed for 2023 by one source) | ⚠️ |
| Weight in the group | Roughly 0.5 % of Reply's revenue | derived |
| Markets | Energy & Utilities first; also Telecommunications and Smart Cities | ✅ |
| Geography | Italy, the Netherlands, TotalEnergies in France, Iceland | 💬 kickoff; not confirmed publicly |

**Reading.** Sense Reply is a specialist boutique of about 80 people inside a €2.5bn group. Revenue per employee is about €150k, which is the profile of a consulting firm: revenue grows only when headcount grows. Revenue looks flat between 2023 and 2024.

---

## 2. What it sells today

| Offer | What it is | Status |
|---|---|---|
| **RIPA** (Reply IoT Platform Accelerator) | A ready-to-deploy, serverless IoT platform built on AWS services, including AWS IoT and AWS Greengrass. Covers gateway and edge, device management, data, security | ✅ |
| Smart grid | Monitoring of low-voltage networks, transformers and secondary substations for electricity, gas and water network operators | ✅ |
| Smart metering | Meter data acquisition and management; listed on AWS Marketplace | ✅ |
| Energy flexibility | Demand-response programme platforms, designed and implemented "in 20 countries" | ✅ |
| Multi Asset Grid Optimization | Coordination of distributed energy assets through a multi-agent framework deployed at the edge and controlled centrally | ✅ |
| Renewables | Harmonising data from generation plants into one data lake | ✅ |
| E-mobility | Charging-point management, roaming, billing, smart charging; works with ThunderSoft for edge intelligence | ✅ |
| Energy communities | Shared local production and consumption | ✅ |
| Asset monitoring with drones, IoT advisory, business applications | Supporting services | ✅ |

**Reading.** The "new" AI-native platform is the next step of RIPA plus the multi-agent optimisation offer. It is not a blank-sheet product: Sense Reply has been selling its building blocks for years as accelerators inside consulting projects.

---

## 3. Known references

| Client | What was built | Status |
|---|---|---|
| **Aeroporti di Roma** (Fiumicino, Ciampino) | Cloud-native IoT platform, with AWS, that collects and standardises operating data from airport assets; AI for anomaly detection and a move towards predictive maintenance. Announced 1 Oct 2026 | ✅ |
| "A global energy operator" | Demand-response platform that monitors and aggregates consumption of commercial and industrial sites, data centres and EV charging stations, connected to national grid operators | ✅ client not named |
| Low-voltage network operators | Monitoring of transformers and secondary substations | ✅ clients not named |
| "A leading e-mobility company" | Platform managing chargers of several brands for operators and service providers | ✅ client not named |
| Renewable generation operator | IoT platform to harmonise plant data | ✅ client not named |
| A platform deciding when to buy and sell energy | 💬 team Q&A; client unknown | 💬 |

None of the public case studies gives a measured result (euros saved, downtime avoided, time to deploy). **This is the biggest gap in their sales material.**

Aeroporti di Roma is also a client of another Reply company: Storm Reply built its AI virtual assistant with AWS (Oct 2025). The account belongs to the group, not only to Sense Reply.

---

## 4. Partnerships and recognition

| Item | Status |
|---|---|
| AWS Premier Consulting Partner | ✅ |
| AWS Energy Competency, obtained with Data Reply and Storm Reply (2021) | ✅ |
| Contribution to two AWS Partner Awards won by Reply in 2023 | ✅ |
| **AWS Industry Partner of the Year, Energy & Utilities, EMEA (2025)** | ✅ |
| AWS Business Value Realization Competency (2026) | ✅ |
| Several packaged offers on AWS Marketplace (smart grid, smart metering, renewables) | ✅ prices not visible to us |
| Second year of collaboration with Albert School on this Business Deep Dive | ✅ |

**Reading.** AWS is their strongest commercial asset and their main dependency. The platform is built on AWS Greengrass, which AWS sells for about $0.16 per device per month. So the layer the brief describes as the product ("governance of edge gateways") is the cheapest part of the stack. Clients do not pay €1M a year for it. They pay for the energy know-how and the applications on top.

---

## 5. Position inside the Reply group

| Reply company | Role | Relation to Sense Reply |
|---|---|---|
| Power Reply | Consulting and processes for Energy & Utilities (Italy, UK, Germany, France) | Natural door-opener to utilities abroad ✅ |
| Storm Reply | AWS cloud specialist | Joint AWS competency; shares the Aeroporti di Roma account ✅ |
| Data Reply | Big data and AI | Joint AWS competency ✅ |
| Concept Reply | IoT | ⚠️ not confirmed in our sources; possible overlap |

**The group already knows how to sell products.** Reply runs several proprietary platforms through dedicated companies: LEA Reply and Click Reply (logistics; Gartner listed Reply as a Visionary for warehouse management systems in 2021), Brick Reply (manufacturing, described as "digital-as-a-service"), TamTamy (enterprise social network, since 2007), Ticuro (remote care). ✅

**Reading.** "Product or service?" is not a new question for Reply. The group's own pattern is a product owned by a specialist company and sold together with integration services. Our recommendation can point to that precedent.

---

## 6. Strengths, weaknesses, opportunities, threats

| | |
|---|---|
| **Strengths** | Deep energy domain knowledge (grid data standard, device protocols). Live references in three areas: airport assets, demand response, grid monitoring. Top-tier AWS status and awards. Access to the client base of a €2.5bn group. Security built in from the start |
| **Weaknesses** | Small: about 80 people, so only a few trials and deployments can run at once. Revenue tied to headcount. No public measured results. Every deployment needs integration work. Price is high and not transparent. Product not yet packaged |
| **Opportunities** | Italy has the highest wholesale power price among large EU markets (€116 per MWh in 2025, EU average €85), so savings are worth more there. Italian grid operators are opening local flexibility markets (RomeFlex in Rome, MiNDFlex in Milan). About €3.6bn of recovery-plan money went to smart-grid projects. New rules open balancing markets to aggregators from 2026. Cyber rules push operators towards secure platforms |
| **Threats** | AWS and other cloud providers sell the edge layer for cents. Energy specialists already run large fleets: gridX (over 200,000 assets, clients such as E.ON) and Barbara (edge platform for grid operators, backed by Iberdrola). New "agentic AI" energy products appeared in 2026 (ev.energy, Sigenergy, Schneider Electric). AI rules for critical infrastructure. Long sales cycles |

---

## 7. What this means for our recommendation

1. **Focus is forced by size.** With about 80 people, Sense Reply cannot chase five segments. One full contract is about 8 % of its yearly revenue. Each trial ties up scarce experts.
2. **The platform must need fewer people per euro than consulting does.** Today the company earns about €150k per employee. A €500k contract that needs more than about 3 people to deliver and run earns less per person than consulting. This gives a concrete target for how standard the product must be. (See `04_business_case.xlsx`, sheet "Sense Reply".)
3. **Sell outcomes, not gateway governance.** The governance layer is a commodity. The price is justified by what the client saves or earns.
4. **Use the group.** Aeroporti di Roma, Power Reply's utility clients and AWS co-selling are the realistic channels. A direct sales force built from zero is not.
5. **Measure and publish results.** Competitors publish numbers (assets connected, named clients). Sense Reply's case studies do not. The B2 pilot and the first paid pilots should produce the proof.

---

## 8. Questions this profile raises for Sense Reply

1. What are the real revenue and headcount, and how much of the revenue is recurring today?
2. How many people work on one client platform during the build, and afterwards?
3. Who is the "global energy operator", and can it be named as a reference?
4. Are the Netherlands, TotalEnergies and Iceland projects on the new platform or on earlier versions?
5. What does AWS co-selling bring today: leads, funding, Marketplace sales?
6. Does any client contract already include a measured result?

---

## 9. Sources

- Sense Reply, company pages (via search extracts): https://www.reply.com/sense-reply/en/about-us ; https://www.reply.com/sense-reply/en ; https://www.reply.com/sense-reply/en/ripa-solutions/reply-iot-platform-accelerator ; https://www.reply.com/sense-reply/en/our-services/smart-grid ; https://www.reply.com/sense-reply/en/our-services/energy-flexibility ; https://www.reply.com/sense-reply/en/our-services/multi-asset-grid-optimization ; https://www.reply.com/sense-reply/en/our-services/e-mobility
- Albert School collaboration: https://www.reply.com/sense-reply/en/education-autonomous-ai-agents-and-the-energy-transition
- Aeroporti di Roma case: https://www.reply.com/en/iot/adr-ottimizza-la-gestione-intelligente-degli-asset-aeroportuali-con-ai-e-iot ; https://www.reply.com/it/newsroom/news/sense-reply-potenzia-gestione-predittiva-infrastrutture-aeroportuali-roma-fiumicino-ciampino-iot-ai
- Storm Reply and Aeroporti di Roma: https://secure.businesswire.com/news/home/20251022666853/en/Aeroporti-di-Roma-Transforms-Passenger-Experience-with-AI-Virtual-Assistant-Powered-by-Amazon-Web-Services-and-Storm-Reply
- Demand-response case: https://www.reply.com/en/energy-and-utilities/a-demand-response-platform-for-electric-grids
- Renewables case: https://www.reply.com/en/iot/iot-platform-for-renewables
- AWS: https://aws.amazon.com/marketplace/seller-profile?id=seller-be5c4tjqfyhra ; https://aws.amazon.com/blogs/apn/how-sense-reply-enables-large-energy-and-utilities-organizations-to-manage-iot-platforms/ ; https://www.reply.com/en/newsroom/news/data-reply-sense-reply-and-storm-reply-achieve-aws-energy-competency-status ; https://www.reply.com/sense-reply/en/experience-for-energy-transition-on-aws
- AWS IoT Greengrass pricing: https://aws.amazon.com/greengrass/pricing/
- Company figures (aggregators): https://www.reportaziende.it/sense_reply_srl_to_11755160014 ; https://aziende.money.it/aziende/sense-reply-srl-11755160014 ; https://www.ufficiocamerale.it/8256/sense-reply-srl
- Reply 2025 results: https://www.reply.com/en/newsroom/financial-news/the-board-of-directors-approved-the-draft-financial-statements-for-the-year-2025
- Power Reply: https://www.reply.com/power-reply/en
- Reply products: https://www.reply.com/tamtamy-reply/en/about-us ; https://www.reply.com/en/investors/financial-reports/2024/reply.html
- Competitors: https://www.gridx.ai/press-releases/gridx-connects-200-000th-energy-asset-to-xenon-platform ; https://iberdrola.com/press-room/news/detail/iberdrola-and-caixa-capital-risc-invest-2-5-million-in-barbara-iot ; https://reimagine.edgeir.com/iberdrola-taps-barbara-for-edge-computing-overhaul-in-smart-grid-substations-20241022 ; https://platform.ev.energy/resources/ev.energy-launches-eve-the-ai-native-platform-built-to-coordinate-the-grid-edge ; https://www.pv-tech.org/industry-updates/sigenergy-unveils-first-all-domain-ai-agent-for-renewable-energy-industry/ ; https://www.esgtoday.com/schneider-electric-launches-new-ai-powered-platform-to-unify-energy-and-sustainability-solutions/
- Italian market context: see `04_business_case.md`, sources.
