# The business case — who can afford this platform, and why

> Status: **working draft, 13 Nov 2026**. Numbers come from `04_business_case.xlsx` (change the blue cells, everything recalculates).
> Company analysis: `05_sense_reply_profile.md`. Segments: `01_segmentation_ICP.md`. Pricing and canvas: `03_business_model.md`.
> ✅ sourced · ⚠️ unverified or conflicting · **H** = team hypothesis. Every input and its source is listed in the Excel sheet "Inputs".

---

## 1. The argument in five findings

Most teams will describe the market. This file answers a narrower question that a CEO can act on: **at the price Sense Reply charges, which clients actually get their money back?**

| # | Finding | Evidence |
|---|---|---|
| 1 | **At €1M a year, almost no client gets a 3× return from energy value alone.** It takes a site twice the size of Rome Fiumicino airport, a 455 MW flexibility fleet, or a grid operator with 2.4 million customers. | Break-even sheet, base case |
| 2 | **At the €200k entry price, the market opens up:** a 60 GWh site, a 90 MW fleet, a grid operator with 470,000 customers. The price ladder decides the size of the market more than the choice of segment does. | Break-even sheet, base case |
| 3 | **The value is not where the demo is.** The battery agent shown at the kickoff is worth about €22k a year on a 10 MWh battery. Site-wide energy savings, maintenance and avoided grid investment are worth 50 to 100 times more. | Client value sheet |
| 4 | **The whole case rests on one unproven number:** how much better smart control performs than fixed rules. The only controlled study we found measured 2 to 3 %. Vendors claim around 20 %. Sense Reply publishes no measured result. | Research, §6 |
| 5 | **Sense Reply is a consulting firm of about 80 people.** A €500k platform contract that needs more than about 3 people earns less per person than consulting does today. That number defines how standard the product must be. | Sense Reply sheet |

**What follows for the recommendation**

- Start at the **€200k entry price with a fee that grows with use** (per gateway, per MW, per substation), and reserve €1M contracts for clients with several sources of value.
- **Sell outcomes, not "edge gateway governance".** The governance layer is built on a cloud service that costs about $0.16 per device per month.
- Make the **3-month test a paid pilot that measures the gain against the client's current control**, and use the B2 team's results as the first proof.
- **Focus on a short list of named large accounts in Italy first** (§7), because a company of 80 people cannot run many pilots at once.

---

## 2. What we re-examined in the case

| The brief says | What the research shows |
|---|---|
| The product is an "AI-native platform for the governance of edge gateways" | That layer is a commodity. Sense Reply's own accelerator (RIPA) is built on AWS IoT and AWS Greengrass. Clients pay for energy know-how and applications ✅ |
| The platform is "ready for commercial positioning" | It is already sold: customised per client, 3-month test, 3-year contracts around €1M a year, €200k minimum 💬 |
| Segment by vertical, site complexity, regulation, geography, AI readiness | These matter less than one filter: **can the client's value cover the fee?** Size decides first |
| "No equivalent platform exists" (kickoff) | Close alternatives exist: gridX (over 200,000 assets connected, E.ON as client), Barbara (edge platform for grid operators, backed by Iberdrola), and 2026 launches of "agentic" energy products by ev.energy, Sigenergy and Schneider Electric ✅ |
| Open question: product or service? | Reply already sells products through specialist companies (LEA Reply, Brick Reply, TamTamy). The real question is how many people each contract needs ✅ |
| B2 students assess the battery agent | Their result is the missing proof for finding 4. It is a sales asset, not a side project |

---

## 3. The client side: three worked examples

Method: for each type of client, add up the yearly value the platform can plausibly create, then compare it with the fee. Three cases per input: Low, Base, High. Defaults use public data on real Italian organisations so that the examples are concrete.

### A. Large infrastructure site — sized on Rome Fiumicino airport

Public data: solar farm of 22 MWp that produced over 30,000 MWh in its first year, about 20 % of the airport's electricity need, so about **150 GWh a year** ✅ (derived). Battery of 10 MWh ✅. Italian industrial electricity price about €203 per MWh in 2025 ✅.

| Yearly value | Low | Base | High | Main assumption |
|---|---|---|---|---|
| Energy saved by monitoring and optimising loads | €0.60M | €1.50M | €2.40M | 2 % / 5 % / 8 % of consumption saved **H** |
| Extra battery value from smart control | €0.01M | €0.02M | €0.04M | 3 % / 10 % / 20 % better than fixed rules **H** |
| Flexibility revenue | €0.09M | €0.24M | €0.47M | 2 / 5 / 10 MW at €47,000 per MW ✅ benchmark |
| **Energy value** | **€0.70M** | **€1.76M** | **€2.91M** | |
| Maintenance savings | €0.50M | €1.00M | €1.80M | ⚠️ placeholder spend of €10M, not a real figure |
| **Total** | **€1.20M** | **€2.76M** | **€4.71M** | |
| Energy value ÷ €1M fee | 0.7× | 1.8× | 2.9× | |
| Total ÷ €1M fee | 1.2× | 2.8× | 4.7× | |

Reading:
- Even for Italy's largest airport, energy value alone returns less than 2× the full fee in the base case. **The contract is justified only when maintenance value is added**, which is exactly what the Aeroporti di Roma platform does (asset monitoring and predictive maintenance) ✅.
- The battery contributes almost nothing. The whole 10 MWh battery earns about €224k a year whatever controls it. Smart control adds a fraction of that. To cover even the €200k entry fee from battery optimisation alone, a client would need about **90 MWh** of batteries.

### B. Flexibility fleet operator — 200 MW under management

Market revenue benchmark: about €110,000 per MW per year for a 4-hour battery in North Italy, first half of 2026 ✅.

| Yearly value | Low | Base | High | Main assumption |
|---|---|---|---|---|
| Extra revenue from better optimisation | €0.44M | €1.10M | €2.20M | 2 % / 5 % / 10 % of market revenue **H** |
| Revenue protected by higher availability | €0.11M | €0.22M | €0.44M | 0.5 % / 1 % / 2 % **H** |
| Integration cost saved on new sites | €0.10M | €0.25M | €0.50M | 50 sites a year, €2k / €5k / €10k each **H** |
| **Total** | **€0.65M** | **€1.57M** | **€3.14M** | |
| Total ÷ €1M fee | 0.7× | 1.6× | 3.1× | |

Reading: a 200 MW fleet does not justify €1M a year unless the gain is at the top of the range. Fleet operators think in euros per MW, so **the fee should be per MW managed**. At the base case, each MW gains about €7,900 a year, which sets the ceiling for a per-MW price.

### C. Distribution grid operator — sized on Areti (Rome)

Areti serves over 1.6 million customers ✅. Benchmark: UK Power Networks reports that buying flexibility saved its customers about £94M in 2025-26, for 8.5 million customers ✅ (company figure), so about €12.70 per customer per year (exchange rate **H**).

| Yearly value | Low | Base | High | Main assumption |
|---|---|---|---|---|
| Benchmark applied to 1.6M customers | €20.3M | €20.3M | €20.3M | Mature-market level |
| **Value the platform helps capture** | **€0.61M** | **€2.03M** | **€4.07M** | 3 % / 10 % / 20 % of the benchmark **H** |
| Value ÷ €1M fee | 0.6× | 2.0× | 4.1× | |

Reading: the prize is large (the EU-wide study by DNV for smartEn estimates €11 to 29bn a year of avoided distribution-grid investment by 2030 ✅), but Italy's local flexibility markets are still pilots. The value arrives later and is shared with other tools. **Grid operators are the largest long-term prize and the slowest to convert.**

---

## 4. How big must a client be?

Smallest client for which yearly value reaches **3× the fee** (base case; 3× is our hypothesis for what a buyer wants before signing for three years).

| Client type | Measure | At €1M a year | At €200k a year | Real-world comparison |
|---|---|---|---|---|
| Infrastructure site (energy saving only) | Electricity use | 300 GWh | 60 GWh | Fiumicino ≈ 150 GWh |
| Fleet operator | Capacity managed | 455 MW | 91 MW | — |
| Grid operator | Customers | 2.36 million | 0.47 million | Areti ≈ 1.6 million |

Just to cover the €1M fee once (1×): 100 GWh, 152 MW, 0.79 million customers.

**What this table says**

1. At the full price, the direct market in Italy is a handful of accounts.
2. At the entry price, it widens to large industrial sites, mid-size aggregators and second-tier grid operators.
3. So the commercial question is less "which segment?" and more "**which price for which size?**" A fee that starts at the minimum and grows with gateways, MW or substations lets one product serve both ends.

---

## 5. The Sense Reply side

⚠️ Company figures come from business-register aggregators and are not checked against filed accounts.

| Measure | Value |
|---|---|
| Revenue per employee today (€11.9M, 80 people) | about €149k |
| One €1M contract as a share of yearly revenue | about 8 % |
| Revenue per person on a €500k contract needing 5 / 3 / 2 people | €100k / €167k / €250k |
| People per €500k contract at which the platform only matches consulting | 3.4 |
| People needed for 19 active contracts in 2031 (base scenario) at 5 / 3 / 2 per contract | 95 / 57 / 38 |
| Revenue from those 19 contracts | €9.5M, about 80 % of today's revenue |

Reading:
- **A platform contract beats consulting only if it needs about 3 people or fewer.** With heavy customisation (5 people), it earns less per person than the business Sense Reply already has.
- The base scenario would need 57 of today's 80 people on platform contracts. Growth therefore depends on **partners doing part of the integration** (other Reply companies, system integrators) or on a more standard product.
- This turns "product or service?" into a measurable target: **people per contract**.

---

## 6. The proof gap

| What we looked for | What we found |
|---|---|
| Measured gain of AI control over fixed rules, on a real site | One controlled university study (greenhouse, solar and battery): electricity cost down 2.2 % and 2.7 % in two months ✅ |
| Vendor claims | About 21 % (an estimate, not measured), other figures of 15 to 40 % without data ⚠️ |
| Predictive maintenance | 18 to 25 % lower maintenance cost for mature programmes (McKinsey, via secondary sources ⚠️); reviews note that early pilots fall short |
| Sense Reply's own results | None published in any case study |
| Pilots in general | About 70 % of industrial IoT pilots do not scale (McKinsey surveys) ✅ |

Consequences:
1. A client's finance director will ask for this number first. Today Sense Reply cannot answer with its own data.
2. **The B2 team's comparison (cost agent vs. cost and sustainability agents, against a baseline) is the first measured answer.** Its percentage goes straight into the yellow cells of the Excel file.
3. The 3-month test should be designed as a measurement: a baseline agreed at the start, the gain measured at the end, and the contract price linked to it.

---

## 7. Where to send the sales team

A company of 80 people needs a short list. Proposal, by order of effort:

| Priority | Who | Why them | Status of facts |
|---|---|---|---|
| 1. Expand existing accounts | Aeroporti di Roma and its parent Mundys (which also controls the Nice, Cannes and Saint-Tropez airports and holds a stake in Bologna airport); the demand-response client | A live reference, a proven budget, no new sales cycle | ✅ Mundys holdings; client name for demand response unknown |
| 2. Replicate the airport case | Largest Italian airports by passengers in 2025: Milan Malpensa (31.4M), Bergamo (16.9M), Naples (13.2M), Bologna (11.1M); Catania and Venice (about 12M each in 2024) | Same assets, same needs. Only the largest reach the entry-price threshold on energy alone, so lead with maintenance | ✅ passenger numbers; electricity use unknown |
| 3. Grid operators through flexibility pilots | Areti (Rome, RomeFlex), Unareti (Milan and Brescia, MiNDFlex), e-distribuzione (about 85 % of the market, 450,000 secondary substations) | Regulator-approved pilots already exist; about €3.6bn of recovery-plan money went to smart-grid projects | ✅ |
| 4. Fleet operators above about 90 MW | Utilities' flexibility arms and large aggregators | Fast decisions, but only above the size threshold, and with a per-MW fee | ⚠️ list to build from the grid operator's register |

**An idea to test with Sense Reply:** a showcase in Rome linking two of these accounts. A large site (the airport, with its solar farm and battery) offering flexibility to the local grid operator through the platform would demonstrate the site use case and the grid use case in one reference. ⚠️ We have not checked whether the airport sits in an area covered by a local flexibility market.

**Why Italy first**
- Highest wholesale electricity price among large EU markets: €116 per MWh in 2025 against €61 in France, €65 in Spain and an EU average of €85 ✅. Every MWh saved is worth more.
- Balancing markets open to independent aggregators from February 2026 ✅.
- Grid regulation now looks at total spending, not only investment, for operators above 25,000 connection points ✅, which makes a subscription easier to accept (to confirm with a regulation specialist).
- A tax incentive for 2026–2028 covers site energy-management software ✅, but only if the software is booked as an asset; the treatment of subscriptions is still open ⚠️. A licence option could help industrial clients (to confirm with a tax adviser).

---

## 8. How to use this in the final presentation

A possible storyline in six slides:

1. **The question:** at €1M a year, who gets their money back?
2. **The answer in one table:** minimum client size at €1M and at €200k (§4).
3. **Where the value is:** the three worked examples, with the battery line shown next to the site-wide lines (§3).
4. **The missing proof:** 2–3 % measured vs. 20 % claimed, and how the B2 result and paid pilots close the gap (§6).
5. **What it means for Sense Reply:** people per contract, and the price ladder (§5, `03_business_model.md`).
6. **Next 90 days:** the named accounts and one paid pilot with a measured baseline (§7).

**The live moment:** open the Excel file, type the B2 team's measured percentage into the yellow cell, and show the break-even table change. It answers the kickoff complaint that "the payback is not visible" and it is a tool Sense Reply's sales team can reuse with a client's CEO.

---

## 9. What is still weak — to fix before the final

| Gap | How to close it |
|---|---|
| Savings percentages are hypotheses | B2 results; ask Sense Reply for one measured client result |
| Maintenance spend is a placeholder | Ask Sense Reply for an order of magnitude from the airport project |
| Sense Reply revenue and headcount are from aggregators | Ask them, or check the filed accounts |
| The 3× return target is our assumption | Ask what return their clients expect |
| Grid-operator value uses a UK benchmark | Look for an Italian figure in the pilot project reports |
| Fleet operator list is missing | Build it from the Italian grid operator's list of qualified providers |
| Meaning of "€1M" and "€200k" | Confirm with Sense Reply |
| No competitor prices found (gridX, Barbara publish none) | Ask Sense Reply what they see in tenders |

---

## 10. Sources

**Prices and markets**
- Italian wholesale price 2025 and comparison: https://www.mercatoelettrico.org/Portals/0/Documents/en-US/Gme_RelazioneAnnualeWeb_2025_en.pdf ; https://en.ilsole24ore.com/art/italia-pays-almost-double-the-price-of-electricity-compared-to-france-and-spain-its-dependence-on-gas-is-a-burden-AIoRBuxD ; https://en.ilsole24ore.com/art/electricity-prices-italy-cinderella-of-europe-116-euro-megawatt-hour-against-eu-average-85-euro-AIAePm8C
- Italian industrial electricity price: https://www.eunews.it/en/2026/05/18/fossil-fuels-and-poor-interconnectivity-italy-had-the-most-expensive-electricity-among-eu-countries-in-2025/
- Battery spreads in Italy: https://pexapark.com/blog/with-macse-the-italian-bess-market-looks-to-stability-instead-of-merchant-upside/ ; https://modoenergy.com/research/jp/italy-bess-benchmark-h1-2026-battery
- Storage auction and capacity market: https://www.pv-magazine.com/2025/10/01/italys-first-macse-battery-auction-smashes-expectations-with-10-gwh-awarded-at-record-low-prices/ ; https://www.ess-news.com/2025/02/28/terna-energy-storage-capacity-auction-2027-delivery-results/
- Balancing market reform: https://arera.it/area-operatori/produzione-tide

**Value benchmarks**
- Controlled study on battery control: https://www.kau.se/en/news/adaptive-battery-reduces-energy-costs-and-peak-power-demand-greenhouses
- Vendor estimate: https://verdigris.co/case-studies/battery-control-for-s-p-global-factory-in-korea
- Predictive maintenance review: https://reliamag.com/topics/guides/predictive-maintenance-roi-benchmarks-what-the-studies-show
- Pilots that do not scale: https://www.mckinsey.com/capabilities/operations/our-insights/operations-blog/its-the-last-it-ot-mile-that-matters-in-avoiding-industry-40s-pilot-purgatory
- UK Power Networks flexibility savings and customers: https://d1lf1oz5vvdb9r.cloudfront.net/app/uploads/2026/04/UKPN-DSO-Panel-Report-2025-26-FINAL.pdf ; https://annualreview2024.ukpowernetworks.co.uk/our-business/who-we-are
- EU flexibility benefits: https://www.dnv.com/publications/demand-side-flexibility-quantification-of-benefits-in-the-eu-232342

**Named organisations**
- Fiumicino solar farm and battery: https://www.fiumicino-online.it/articoli/attualita/aeroporti-di-roma-aderisce-a-millumino-di-meno-scali-romani-protagonisti-della-transizione-energetica ; https://corporate.enelx.com/en/media/press-releases/2023/06/enel-x-aeroporti-di-roma-europes-largest-self-consumption-photovoltaic-system-at-romes-leonardo-da-vinci-airport
- Italian airports, passengers 2025: https://www.9colonne.it/612728/italian-airports-record-strong-growth-with-nearly-230-million-passengers-in-2025 ; https://www.theflightclub.it/en/2026/01/nel-2025-gli-aeroporti-italiani-tornano-a-volare-alto-superati-i-229-milioni-di-passeggeri/
- Mundys holdings: https://www.mundys.com/en/about-us
- Local flexibility pilots: https://www.gruppo.acea.it/en/media/press-releases-and-news/press-releases/2023/10/smart-city-acea-with-romeflex-the-flexibility-of-the-electrical-grids-starts-from-rome ; https://www.arera.it/fileadmin/allegati/docs/24/117-2024-R-eel.pdf
- e-distribuzione network and smart-grid funding: https://www.e-distribuzione.it/content/dam/e-distribuzione/documenti/piano-di-sviluppo/Webinar_Piano_di_Sviluppo_2023_conQA.pdf ; https://www.ecoseven.net/flash-news/pnrr-mase-via-libera-a-36-mld-per-22-progetti-su-smart-grid/
- Grid regulation (total-spending approach): https://arera.it/atti-e-provvedimenti/dettaglio/23/497-23
- Tax incentive 2026–2028: https://www.reteagevolazioni.it/allegati-iv-e-v-legge-bilancio-2026-beni-strumentali-ammessi-alliperammortamento/ ; https://www.mysolution.it/fisco/informazioni/news/2026/07/10/iperammortamentosoftware-agevolabili-se-iscritti-tra-le-immobilizzazioni/

**Sense Reply, Reply and competitors:** see `05_sense_reply_profile.md`, §9.
