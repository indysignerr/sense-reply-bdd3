# Deliverable 1 — Segmentation map & Ideal Customer Profiles (working draft)

> Status: **working draft, 11 Nov 2026**. Figures marked ✅ were checked against a source (see §8).
> Figures marked ⚠️ are unverified or conflicting between sources: verify before they go on a slide.
> Scores in §4 are **team hypotheses**, not data. They must be challenged by the team and, where possible, by the B2 pilot data.

---

## 0. The one-line answer (draft)

**Sell first to the operators of asset *fleets* — flexibility aggregators and DSOs — not to individual sites.**
The platform's value grows with the number of gateways it governs, its data model (IEC CIM) is a grid-operator standard, and Sense Reply already has demand-response references in 20 countries. Individual factories, buildings and energy communities come later, through those fleet operators or through partners.

---

## 1. Reframe before segmenting: what are we actually selling?

| What the product really is | What it implies for segmentation |
|---|---|
| A platform that **governs fleets of edge gateways** (remote app deployment, rollback, PKI onboarding, multi-tenant) | Value grows with **number of sites/gateways per customer** → favour customers who operate many sites |
| Asset model based on **IEC 61970/61968 CIM** | CIM is the **grid operator** standard (DSO/TSO). Native fit with utilities, weak relevance for a single factory |
| **X.509/mTLS security, multi-tenant isolation** | Strong argument for entities under **NIS2 / critical-infrastructure** rules |
| **Edge AI agents that keep running offline** | Valuable where connectivity is poor or where latency/safety matter (substations, remote assets, industrial sites) |
| Multi-vendor gateways / protocol harmonisation (kickoff: "number one technical difficulty") | Every deployment includes integration work → **project + licence**, not pure self-serve SaaS |

Sense Reply's existing assets (public material): the **RIPA** IoT platform accelerator, a **Smart Grid** offer listed on AWS Marketplace, a **Multi Asset Grid Optimization** solution described as a multi-agent framework deployed at the edge, and **demand-response platforms designed in 20 countries** for a "global energy operator". ✅
→ The new platform is a productised evolution of things they already sell. Their **right to win** is highest where they already have references: utilities, DSOs, flexibility/demand response.

---

## 2. Segmentation axes used

We segment on **two levels**, because a single axis (e.g. "industry vertical") hides the real buying logic.

1. **Who buys and operates the fleet** (primary axis): grid operator, aggregator, multi-site corporate, single site, community.
2. **Qualifying filters** (from the brief): site complexity (number and mix of assets), regulatory exposure, geography, AI/digital readiness.

---

## 3. Segment map — 8 candidate segments

| # | Segment | Who buys | Typical assets | Main regulatory driver | Size anchors |
|---|---|---|---|---|---|
| S1 | **Distribution System Operators (DSOs)** | CTO / Head of Grid Digitalisation, Head of Network Operations | Secondary substations, transformers, MV/LV sensors, DER connections | EU Grids Action Plan; flexibility needs assessments; IT: ARERA observability of distributed generation | ✅ ~2,570 DSOs in the EU, 250 M customers. Very concentrated: one DSO in 5 member states, 883 in Germany (2021). Italy: e‑distribuzione ≈ 85 % of the market. ✅ €584 bn grid investment needed by 2030, of which ~€375–425 bn in distribution |
| S2 | **Flexibility aggregators / VPP / Balancing Service Providers** (incl. utilities' flexibility arms) | Head of Flexibility / Trading, CTO | Hundreds to thousands of distributed sites: BESS, PV, flexible industrial loads, EV chargers | Electricity Market Design reform (Reg. 2024/1747) — non‑fossil flexibility objectives & support schemes; upcoming Network Code on Demand Response | ⚠️ No reliable count found yet. Sense Reply already built DR platforms in **20 countries** ✅ |
| S3 | **Energy‑intensive, multi‑site industry** (chemicals, food, metals, paper, plastics…) | CFO / COO + Energy Manager; IT/OT for gateways | Production lines, compressors, chillers, PV + BESS on site, CHP | ✅ EED recast Art. 11: certified energy management system mandatory above **85 TJ/yr (≈ 23.6 GWh)** by **Oct 2027**; audit above 10 TJ (≈ 2.8 GWh) by Oct 2026 | ✅ EU ETS covers > 16,000 stationary installations (proxy for heavy sites; Germany alone: 1,794 in 2025). ⚠️ No count found of companies above 85 TJ |
| S4 | **Commercial real estate portfolios** (offices, retail, logistics, hotels) | Asset / property manager, ESG lead | HVAC, lighting, PV, BESS, EV chargers | ✅ EPBD recast: building automation (BACS) mandatory in non‑residential buildings > **290 kW** HVAC (end 2024) and > **70 kW** (end 2029), "where feasible" | ⚠️ To size via national building stock data |
| S5 | **Renewable energy communities (CER)** and their facilitators (municipalities, ESCOs, utilities) | Community manager / ESCO / municipality | Small PV, small BESS, smart meters | RED II/III energy-community rules; IT: DM 414/2023 incentives (until end 2027) + PNRR grants | ✅ Italy: GSE counts vary strongly by date/definition — 212 active (Mar 2025), 904 (Dec 2025), 3,630 configurations / 303 MW (Jun 2026), > 4,800 / ~400 MW (Aug 2026) ⚠️. PNRR grants: €1,014.5 M granted for 2.3 GW. **Average community ≈ 80 kW** → very small assets |
| S6 | **Microgrids & closed sites** (ports, airports, industrial parks, campuses, islands) | Infrastructure / technical director | PV, BESS, gensets, shore power, EV, HVAC | Port electrification (shore power), resilience, grid-connection delays | ⚠️ To size |
| S7 | **EV charge point operators & e‑fleet depots** | CTO / Head of Operations | Chargers, site BESS, PV | AFIR, smart-charging requirements | ⚠️ To size |
| S8 | **BESS / PV owners, IPPs and equipment OEMs** (as customer *or* as channel) | Asset manager / OEM product lead | Utility-scale and C&I batteries, PV plants | Storage support schemes; flexibility markets | ✅ Europe installed **36 GWh** of batteries in 2025, fleet > 100 GWh, forecast 138 GWh/yr by 2030. C&I batteries: **4.7 GWh in 2025 (+77 %)** — mostly used for simple self-consumption / peak shaving |

---

## 4. Scoring grid (team hypotheses — to challenge)

**Criteria and weights**

| Criterion | Weight | Question asked |
|---|---|---|
| Product fit | 25 % | Does the platform's architecture (fleet governance, CIM, edge, security) solve a real problem here? |
| Regulatory pull | 20 % | Does a regulation force or fund the purchase in the next 1–3 years? |
| Ability to pay | 15 % | Budget size and willingness to pay for software |
| Sales-cycle speed | 15 % | 5 = < 6 months, 1 = > 24 months / public tender |
| Sense Reply right to win | 15 % | Existing references, relationships, credibility |
| Scale per deal | 10 % | Number of gateways/sites per customer |

**Scores (1 = poor, 5 = excellent)**

| Segment | Fit | Reg. | Pay | Speed | Right to win | Scale | **Weighted score** |
|---|---|---|---|---|---|---|---|
| S1 DSOs | 5 | 5 | 4 | 1 | 5 | 5 | **4.25** |
| S2 Aggregators / VPP | 4 | 4 | 4 | 4 | 4 | 5 | **4.10** |
| S8 BESS/PV owners & OEMs | 4 | 3 | 3 | 4 | 2 | 5 | **3.45** |
| S3 Energy‑intensive industry | 3 | 4 | 4 | 3 | 3 | 3 | **3.35** |
| S7 CPOs / e‑fleets | 3 | 3 | 3 | 3 | 3 | 4 | **3.10** |
| S6 Microgrids / ports | 4 | 2 | 3 | 3 | 3 | 2 | **2.95** |
| S4 Commercial real estate | 2 | 3 | 3 | 3 | 2 | 4 | **2.70** |
| S5 Energy communities (direct) | 3 | 4 | 1 | 2 | 3 | 2 | **2.65** |

Formula: `score = 0.25·Fit + 0.20·Reg + 0.15·Pay + 0.15·Speed + 0.15·RightToWin + 0.10·Scale`

**Reading the map (for the slide: X = ability to win/speed, Y = attractiveness)**

- **Priority now — S2 aggregators/VPP**: high score *and* fast cycle; Sense Reply already has DR references → shortest path to first revenue.
- **Strategic anchor — S1 DSOs**: best fit and biggest deals, but 18–36-month cycles and tenders. Start now, expect revenue later. Use existing Reply DSO relationships (Italy first).
- **Second wave — S3 industry & S8 OEM channel**: EED 2027 deadline creates urgency for industry; OEMs can embed the platform and multiply gateways without a direct sales force.
- **Deprioritise as direct targets — S4 real estate, S5 energy communities**: real estate is a crowded building-management market (Siemens, Schneider, Johnson Controls…); energy communities have tiny assets (~80 kW on average in Italy) and almost no software budget. **Serve energy communities as a *use case sold to* DSOs, utilities and ESCOs**, not as direct customers.

> ⚠️ Where we disagree with the client's framing: the kickoff put DSOs **and** energy communities on the same level. The data does not support selling directly to energy communities; it supports reaching them through B2B2C partners.

---

## 5. Ideal Customer Profiles

### ICP 1 — Flexibility aggregator / VPP operator (entry segment)

| Field | Profile |
|---|---|
| Firmographics | European aggregator, BSP, or the flexibility arm of a utility/energy major; operates **≥ 200 distributed sites** in ≥ 2 countries |
| Assets | Mixed fleet: C&I batteries, PV, flexible industrial loads, EV chargers — **multiple vendors and protocols** |
| Trigger events | Entering a new national flexibility market; launch of a non-fossil flexibility support scheme; scaling pains with the current rule-based dispatch; gateway fleet becoming hard to update/secure |
| Pain | Each new site = custom integration; fleet updates are manual; dispatch is single-objective; cyber obligations rising |
| Value proposition | "Onboard a new site in days, not weeks; update and secure the whole fleet from one console; optimise each site on several objectives at once (revenue, cost, battery health, CO₂)" |
| Economic buyer | CEO / Head of Flexibility |
| Champion | Head of Operations / CTO |
| Blockers | Internal IT team that built its own stack ("build vs buy") |
| Disqualifiers | < 50 sites; single-vendor fleet already locked into an OEM cloud |
| Why Sense Reply wins | Existing DR platforms in 20 countries; AWS-native; can customise business logic |

### ICP 2 — Distribution System Operator (strategic anchor)

| Field | Profile |
|---|---|
| Firmographics | Medium to large DSO (≥ 500,000 connection points), **Italy first**, then markets with similar regulation; ideally an existing Reply client |
| Assets | Secondary substations and transformers, MV/LV sensors, connected DER |
| Trigger events | Regulator observability / real-time monitoring requirements (IT: ARERA framework on distributed generation data); flexibility needs assessments; regulated investment plans; NIS2 audits; grid-connection backlogs |
| Pain | Low visibility on LV/MV grid; heterogeneous field devices; need to manage congestion without new copper; strict cyber requirements |
| Value proposition | "Monitor and steer your distribution grid in real time **without building new hardware**, on a CIM-native and NIS2-ready platform" |
| Economic buyer | CEO / CFO (capex vs opex treatment under regulation) |
| Champion | Head of Grid Digitalisation / Network Operations |
| Blockers | Procurement (public tenders), OT security team, incumbent SCADA/ADMS vendor |
| Disqualifiers | Very small municipal DSOs (< 50,000 customers) without IT capacity — reach them through national associations or shared-service providers |
| Why Sense Reply wins | Existing smart-grid references, CIM model, security by design, Reply's long-term utility relationships |

### ICP 3 — Energy-intensive multi-site manufacturer (second wave)

| Field | Profile |
|---|---|
| Firmographics | Manufacturing group with **≥ 3 sites in Europe**, at least one site **> 85 TJ/yr (≈ 23.6 GWh)**, energy = significant share of costs |
| Assets | On-site PV and/or BESS (installed or planned), flexible loads (compressors, furnaces, chillers, cold storage) |
| Trigger events | EED energy-management-system deadline (Oct 2027); new BESS investment; energy price spike; ESG reporting |
| Pain | Energy bills; IT/OT split; no single view across sites; batteries used only for peak shaving |
| Value proposition | **Savings first** (kickoff: "companies want to save money, not the planet"): one dashboard showing where the money goes + agents that shift load and battery use to cheaper hours, with optional flexibility revenue |
| Economic buyer | CFO / COO (CEO push needed — kickoff) |
| Champion | Group Energy Manager |
| Blockers | OT/plant engineering (safety), IT security |
| Disqualifiers | Single small site; no on-site flexible assets |
| Channel | Better reached through ESCOs, BESS integrators or the customer's aggregator than by a direct sales force |

### ICP 4 (optional) — BESS / PV OEM or integrator as channel partner

| Field | Profile |
|---|---|
| Firmographics | European BESS/PV integrator or OEM shipping C&I systems (C&I batteries grew +77 % in 2025 in Europe) |
| Need | Offer a fleet-management and optimisation layer without building it |
| Model | White-label / OEM licence per gateway shipped |
| Why it matters | Multiplies gateways without Sense Reply sales effort |

---

## 6. Regulatory drivers (summary for the deck)

| Driver | What it does | Segments | Status |
|---|---|---|---|
| EU Action Plan for Grids (Nov 2023) | €584 bn grid investment need by 2030; push for digitalisation and smart grids | S1 | ✅ |
| Electricity Market Design reform (Reg. 2024/1747) | National flexibility needs assessments → non-fossil flexibility objectives and possible support schemes | S1, S2, S8 | ✅ methodology approved; national reports in progress (2026) |
| Network Code on Demand Response | Harmonises access of demand response, storage and distributed generation to markets and to DSO local services | S1, S2 | ⚠️ ACER recommendation March 2025; **not yet adopted as of June 2026** |
| Energy Efficiency Directive recast (2023/1791), Art. 11 | Certified energy management system > 85 TJ (Oct 2027); audit > 10 TJ (Oct 2026) | S3 | ✅ thresholds; national transposition ongoing |
| EPBD recast (2024/1275) | BACS mandatory > 290 kW (end 2024) and > 70 kW (end 2029) in non-residential buildings | S4 | ✅ (some secondary sources quote other dates) |
| Energy communities (RED II/III; IT: DM 414/2023 + PNRR) | Incentives on shared energy until end 2027; PNRR grants for municipalities < 50,000 inhabitants | S5 | ✅ |
| Italy — ARERA observability of distributed generation | Real-time data from distributed generation for grid operation; new architecture for remote curtailment (2026) | S1 | ⚠️ details of the 2026 decision to verify |
| NIS2 + Network Code on Cybersecurity for electricity | Cyber obligations on energy entities | S1, S2, S7 | ⚠️ scope per entity type to verify |
| **AI Act — Annex III point 2 (headwind)** | AI used as a *safety component* in electricity supply by entities designated "critical" is **high-risk** → conformity obligations. Pure forecasting/optimisation may be out of scope | S1 mainly | ⚠️ application date disputed (Aug 2026 vs postponed to Dec 2027) |

**Implication:** the AI Act is a **risk for the DSO segment** if agents act directly on the grid. The "human validates the decision" pattern shown in the kickoff demo must be presented as a design feature.

---

## 7. Market sizing — method (numbers still to fill)

We did **not** find a reliable published market size for "edge-AI orchestration platforms for energy". Do not invent one. Use a bottom-up estimate:

```
Serviceable market (€/yr) = Σ over priority segments of
    (number of target customers) × (gateways per customer) × (annual price per gateway)
  + one-off integration fees
```

| Input | Where to find it | Status |
|---|---|---|
| Number of DSOs by size, Italy + priority countries | ACER DSO report annex (early 2025), EU DSO Entity map | to collect |
| Number of aggregators / BSPs per country | National TSO lists of qualified balancing service providers | to collect |
| Number of sites > 85 TJ | National EED transposition / energy agencies (e.g. ENEA for Italy) | to collect |
| Price per gateway / per asset | Competitor benchmark (Deliverable 2, week 2) | to collect |
| Gateways per customer | Sense Reply / B2 pilot data | ask the client |

---

## 8. Sources

- EU DSO Entity — facts on DSOs (≈ 2,570 EU DSOs, citing Eurelectric 2025): https://eudsoentity.eu/knowledge-sharing/
- EU DSO map 2024: https://eudsoentity.eu/wp-content/uploads/2025/01/2024_EU-DSO-map_web.pdf
- ACER 2026 DSO revenue-setting report annex: https://www.acer.europa.eu/sites/default/files/documents/Publications_annex/ACER-2026-DSO-revenue-setting-report-Annex.pdf
- European Commission — EU Action Plan for Grids: https://energy.ec.europa.eu/publications/eu-action-plan-grids_en
- Commission factsheet (grids): https://ec.europa.eu/commission/presscorner/api/files/attachment/876888/Factsheet_EU%20Action%20Plan%20for%20Grids.pdf
- EED Art. 11 (85 TJ / 10 TJ): https://www.dnv.com/assurance/Management-Systems/eu-directive-2023-1791-energy-efficiency-iso-50001/ ; https://www.iea.org/policies/32009 ; https://www.mhc.ie/latest/insights/changes-to-energy-audit-and-management-obligations
- EPBD BACS thresholds: https://build-up.ec.europa.eu/en/resources-and-tools/articles/what-makes-building-smart-technologies-driving-energy-efficiency ; https://www.rehva.eu/rehva-journal/chapter/the-epbd-recast-boosts-smart-ready-buildings
- Italy energy communities (GSE data, incentives): https://greencam.unioncamere.it/wp-content/uploads/2026/02/CACER-Bilancio-e-prospettive-alla-luce-della-revisione-del-PNRR_GSE.pdf ; https://lentepubblica.it/cittadini-e-imprese/comunita-energetiche-rinnovabili-italia-e-ancora-lontana-dagli-obiettivi-del-2027/ ; https://www.infobuildenergia.it/incentivi-cer-associazioni-chiedono-proroga-2030/ ; https://ediltecnico.it/nuovo-decreto-cer/
- Battery storage Europe (SolarPower Europe data): https://reglobal.org/europe-installed-36-gwh-bess-capacity-in-2025-report/ ; https://taiyangnews.info/storage/europe-battery-storage-capacity-exceeds-100-gwh ; https://battery-tech.net/battery-markets-news/eu-battery-storage-capacity-soars-45-to-27-1-gwh-in-2025/
- Network Code on Demand Response: https://www.acer.europa.eu/news/new-network-code-demand-response-will-further-advance-energy-transition ; https://electra.cigre.org/346-june-2026/one-grid/from-fragmentation-to-coordination-how-the-network-code-on-demand-response-reshapes-demand-side-flexibility-in-europe
- Flexibility needs assessment (EMD reform): https://www.entsoe.eu/news/2025/04/16/dso-entity-and-entso-e-submit-joint-methodology-on-flexibility-needs-assessment/ ; https://www.acer.europa.eu/news/acer-approves-eu-wide-methodology-assess-national-electricity-flexibility-needs
- AI Act and electricity: https://fsr.eui.eu/the-ai-act-in-the-electricity-sector/ ; https://www.mccannfitzgerald.com/knowledge/data-privacy-and-cyber-risk/critical-infrastructure-spotlight-eu-ai-act-draft-guidelines-on-high-risk-ai-classification
- Italy distribution market: https://www.websim.it/azioni/blue-chip/utilities-sector-confermata-nella-legge-di-bilancio-2025-la-proroga-delle-concessioni-di-distribuzione-elettrica-20250103071528/ ; https://reports.acea.it/2023/en/sustainability-report/relations-stakeholders/customers-and-community/acea-group-customers-electricity-and-water-services
- ARERA observability of distributed generation: https://arera.it/allegati/docs/22/287-22.pdf ; https://www.arera.it/allegati/docs/21/540-21.pdf
- EU ETS installations: https://www.eea.europa.eu/en/analysis/maps-and-charts/emissions-trading-viewer-1-dashboards ; https://www.umweltbundesamt.de/en/press/pressinformation/european-emissions-trading-german-emissions-to-fall
- Sense Reply offers (RIPA, smart grid, multi-asset optimisation, energy flexibility): https://www.reply.com/sense-reply/en/our-services/iot-platforms ; https://www.reply.com/sense-reply/en/our-services/multi-asset-grid-optimization ; https://reply.com/sense-reply/en/our-services/energy-flexibility ; https://www.reply.com/en/energy-and-utilities/a-demand-response-platform-for-electric-grids

---

## 9. Questions to ask Sense Reply (to close the gaps)

1. How many gateways does a typical customer deploy today (DSO vs aggregator vs industrial site)?
2. Which existing clients (Italy, Netherlands, TotalEnergies, Iceland) could become pilot customers for the new platform, and in which segment?
3. Is the "global energy operator" demand-response client an aggregator? Can it be named as a reference?
4. Are agents expected to **act** on assets autonomously or only **propose** (AI Act implications)?
5. Which hardware gateways are supported, and can OEMs embed the platform (channel model)?
