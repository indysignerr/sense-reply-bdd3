# Sense Reply BDD — Part 3: Business model (draft)

> Albert School BDD #3, case B1. Draft of 17 Nov 2026, for team review.
> Numbers come from `Part3_business_model.xlsx` (change the blue cells, everything recalculates).
> Built on the team briefing (13 Nov), Part 1 and Part 2. Prices are **our proposals**: Sense Reply gave us no contract value.
> **TD** = from a team document · **PS** = public source · **H** = team hypothesis, to confirm.

---

## 1. The answer on one page

**Reply stays a consulting firm, but stops starting from zero on every project and gets paid every year for what it has already built.**

| | Today | Our model |
|---|---|---|
| What Reply sells | A custom project, then a best-effort contract | The same custom projects for large groups, **plus a managed service** built from agents that have matured |
| Pilot | About 3 months, free or at cost, no commitment | About 3 months, paid at cost, KPIs agreed upfront, credited if the client signs |
| Growth | The whole business in one decision | One plant at a time |
| Incentive | No guarantee, no link to results | Still no guarantee; a bonus on measured savings, upside only |
| Reach | Reply's own consultants | Reply for large groups; partners for everyone else |

**The four numbers to remember (base case)**

| | |
|---|---|
| What a typical plant gains per year | **€52k**, about 3.8 % of its electricity bill |
| What Reply earns per plant per year | **€18k** (one third of the gain) |
| What one typical account brings Reply | **€54k per year** on average over 3 years |
| Revenue per consultant in year 3 | **€303k** in our model, against €124k with today's way of selling |

**Figures for Part 1 (market in euros per year):** typical account €54k · TAM €162M · SAM €93M · ICP €46M · SOM €1.9M (25 accounts, of which 3 lighthouse).

**The uncomfortable finding, which we keep:** selling directly to manufacturers is not enough on its own. 25 accounts bring about €1.9M a year. One partner running 50 plants is worth almost four direct accounts, with no pilot for Reply to run. **Partners are the engine, not a side channel.**

---

## 2. How Reply sells today (from the 13 Nov meeting)

1. A pilot of about 3 months on one client site, often free or at cost. Reply also uses it to collect data.
2. A 3-year contract extended to the whole business.
3. Not a licence, and no guaranteed number: Reply provides expertise on a best-effort basis.
4. Revenue = the contract + integration. Every project is heavily customised.
5. Identity: frontier innovation. What Reply invents becomes standard and is then sold more cheaply by single-feature competitors.

**What this means:** Reply is a consulting firm. It earns by selling its people's days, so revenue grows only with headcount, and each project's know-how leaves with the project. Our model keeps that identity and fixes those two points.

---

## 3. Site ROI case: what one typical plant gains (task C2)

**The typical account** (TD): a Northern Italian manufacturer with 3 plants and 15 GWh of electricity a year (Part 1: 14 GWh per company on average, 2 to 10 plants).
**The typical plant:** 5 GWh a year, a €1.39M electricity bill at €278/MWh (TD), 1 MWp of solar and flexible loads such as cold rooms, ovens and compressors (TD). No battery: Part 2 shows most Italian sites are solar-only, and battery optimisation is given away by battery makers.

| Yearly gain per plant | Low | Base | High | How |
|---|---|---|---|---|
| 1. Using more of its own solar | €12k | €20k | €27k | Agents run flexible loads when the sun shines, instead of exporting solar at a low price |
| 2. Moving consumption to cheap hours | €7k | €23k | €52k | 5 % / 10 % / 15 % of consumption moved (H), price gap of €39 / €60 / €88 per MWh (PS) |
| 3. Lower peaks | €1k | €3k | €4k | Network charge of €28 per kW per year (PS): small in Italy |
| 4. Selling flexibility through an aggregator | €3k | €7k | €10k | 100 / 200 / 300 kW (H) at €47,000 per MW per year (PS), after the aggregator's cut |
| **Total per plant** | **€24k** | **€52k** | **€94k** | |
| As a share of the bill | 1.7 % | 3.8 % | 6.8 % | |
| **Total for a 3-plant account** | **€71k** | **€157k** | **€282k** | |

**Is this credible?** A study of 83 plants that put an energy management system in place measured 3 to 4 % a year (Lawrence Berkeley National Laboratory). Our base case sits in that range.

**What it tells us**
- The value comes from **solar plus flexible loads** (lines 1 and 2: over 80 % of the gain). This is Part 2's "virtual battery".
- **Peak shaving is not the argument in Italy.** It becomes one in Germany, where grid fees are the issue (phase 2).
- These are estimates. Reply promises none of them.

---

## 4. Pricing (task C5)

**Principle:** the client keeps about two thirds of the gain, Reply takes about one third.

| Revenue line | Who pays | Price | Logic |
|---|---|---|---|
| **Conditional pilot** | Client | €20k for about 3 months on one plant | At cost. KPIs and baseline agreed before the start. Credited against set-up if the client signs |
| **Set-up / integration** | Client | €30k for the first plant, €12k for each further plant | Reply's DNA, kept. Cheaper after the first plant because agents and connectors are reused |
| **Managed service** | Client | **€10k per plant per year** | Reply runs the plant's energy orchestration on its platform. About €830 a month: well above the market signals in Part 2 ($200–300 per site per month), well below an incumbent's project |
| **Success bonus** | Client | **15 % of measured savings** (about €8k per plant in the base case) | Upside only, no penalty. Measured by the digital twin against the agreed baseline. Includes flexibility revenue, so no separate line for market access |
| **White-label platform fee** | Partner (ESCO, integrator, aggregator) | €4k per plant per year, minimum 25 plants | 40 % of the direct fee: the partner sells and installs. Minimum of €100k a year per partner |
| **Frontier co-innovation** | Lighthouse client | Project fee, about €100k a year (H) | Today's business, kept. Reply keeps the right to package what it builds |

Optional add-ons, not in the numbers: a compliance pack (audit-trail reports for the EU energy audit and the AI Act) and extra agents as they mature.

**Does the client win?**

| Per plant, per year | Low | Base | High |
|---|---|---|---|
| Gain | €24k | €52k | €94k |
| Paid to Reply (service + bonus) | €14k | €18k | €24k |
| Reply's share of the gain | 57 % | 34 % | 26 % |
| Kept by the client | €10k | €35k | €70k |
| Result in year 1 of the first plant, after set-up | −€20k | +€5k | +€40k |

In the base case the first plant pays for itself in the first year. In the low case it takes until year 3: this is why the pilot must measure the gain **before** the client commits.

**What one account brings Reply**

| Account type | Year 1 | Year 2 | Year 3 | Average per year |
|---|---|---|---|---|
| Typical account, 3 plants, one more each year | €48k | €48k | €66k | **€54k** |
| Lighthouse account, large group, 10 plants + co-innovation | €178k | €225k | €339k | **€247k** |
| Partner, 25 then 50 then 75 plants | €100k | €200k | €300k | **€200k** |

One partner is worth about 3.7 typical accounts.

**Why this is not "cheap SaaS":** the recurring line is a service run by Reply's experts, priced at 3 to 4 times the market signal for energy software, and it comes on top of integration and co-innovation, which stay.

---

## 5. Business Model Canvas, to-be (task C4)

| Block | Kept from today | New |
|---|---|---|
| **Customer segments** | Large groups, as lighthouse clients | Mid-sized energy-intensive manufacturers in Northern Italy (through partners); fleet operators (ESCOs, integrators, aggregators); cold-chain logistics |
| **Value propositions** | Frontier innovation, tailored | Lower energy bill from solar and flexible loads working together; one system that keeps gaining agents; works with any vendor's equipment; every AI decision logged. For partners: "your clients, your data, your brand" |
| **Channels** | Reply's direct sales and existing clients | Partners for mid-sized firms; cloud marketplaces for packaged agents |
| **Customer relationships** | Co-innovation with large clients | Conditional pilot; growth one plant at a time; managed service with a yearly review of measured savings |
| **Revenue streams** | Integration and project fees | Managed service per plant; success bonus; white-label platform fees |
| **Key resources** | Reply's people and innovation capability | The platform and its catalogue of agents; pilot data used as benchmarks ("plants like yours save X") |
| **Key activities** | Frontier R&D; integration | Packaging mature agents; running the managed service; enabling partners |
| **Key partners** | Cloud providers | ESCOs, battery and solar integrators, aggregators with market access, gateway hardware makers |
| **Cost structure** | People (integration, R&D) | Cloud and AI running costs (small per plant); partner support; a small product team to package agents |

---

## 6. Channels: who sells to whom

| Segment | Speed | Who sells | What is sold |
|---|---|---|---|
| Large multi-site groups | Frontier | Reply directly | Co-innovation project + managed service across plants |
| Typical multi-site manufacturers (primary ICP) | Mature, with light tailoring | Reply directly at first, to build references | Conditional pilot, then managed service plant by plant |
| Mid-sized manufacturers (2,221 firms Reply cannot serve one by one) | Mature | Partners | Packaged agents under the partner's brand |
| Fleet operators | Mature | Reply directly, to the partner's management | White-label platform |
| Cold-chain logistics | Mature | Reply or partners | Packaged "virtual battery" agent for cold rooms |

Aggregators provide market access for line 4 of the site case. Reply has no trading licence (Part 2) and does not need one.

---

## 7. Go-to-market roadmap (task C7)

| Phase | When | What happens | Target at the end (base case) |
|---|---|---|---|
| **1. Prove** | 0–6 months | Conditional pilots with typical accounts in Northern Italy; 1 lighthouse account; write the standard pilot contract; sign a first partner | 5 pilots started, measured gains on at least 3 plants |
| **2. Package and partner** | 6–18 months | Turn what worked into packaged agents (virtual battery first); expand signed accounts to their second plant; sign 2 more partners; first cold-chain package | 13 accounts signed, 3 partners, about 100 partner plants |
| **3. Scale** | 18–36 months | Partners carry the mid-market; third plants go live; prepare Germany for the 2029 grid-fee reform (Part 1) | 25 accounts, 6 partners, about 300 plants on the platform |

---

## 8. Three-year numbers: today's model against ours (task C6)

Same sales effort in both: the same number of pilots started (10, 16, 18) and one lighthouse account a year. What changes is how they are sold.

| | Today's model | Our model |
|---|---|---|
| Pilots that become contracts (H) | 30 % | 50 % |
| Accounts signed in 3 years | 16 | **25** (Part 1's target) |
| Plants on the platform in year 3 | 57 | **300** (244 through partners) |
| Revenue over 3 years | €3.3M | **€5.2M** |
| Revenue in year 3 | €1.7M | **€3.0M** |
| Recurring share in year 3 | 34 % | **65 %** |
| People needed in year 3 | 13.4 | **10.0** |
| **Revenue per person in year 3** | €124k | **€303k** |
| Pilot days given for free over 3 years | 1,760 | 0 |

Year by year, our model: €0.6M, €1.6M, €3.0M. Partners bring 32 % of revenue in year 3.

**Reading**
- Our model does not shrink the consulting business. Integration and co-innovation are still there. It adds recurring revenue on top.
- The gain a consulting firm cares about is **revenue per person**: more than double, because agents are reused and partners do the field work.
- Every driver is a declared hypothesis (conversion rates, days per site, partner growth). The Excel file shows the effect of changing any of them.

---

## 9. KPIs and risks (task C7 / R)

**Four KPIs**

| KPI | Target | Why |
|---|---|---|
| Pilot conversion | 50 % | Shows the conditional pilot works |
| Plants per account after 3 years | 3 | Shows land and expand works |
| Recurring share of revenue | 65 % in year 3 | Shows Reply earns after the project ends |
| Revenue per person | €300k in year 3 | The measure a consulting firm manages by |

**Top risks**

| Risk | Mitigation |
|---|---|
| The gain is lower than estimated (low case: Reply would take 57 % of it) | The pilot measures the gain before any commitment; the bonus falls with the gain |
| Partners build their own tool instead | Neutrality, time to market and the AI Act-ready audit trail (Part 2); minimum commitment keeps the deal simple |
| Reply's consultants see the managed service as a threat to billable days | Integration and co-innovation stay; track revenue per person, not days sold |
| Clients do not have an hourly-priced supply contract, so line 2 of the site case is not available | Check in the pilot; the solar line alone still covers the fixed fee in the base case |
| Disagreement on the baseline for the bonus | Baseline agreed in writing before the pilot, measured by the digital twin, reviewed once a year |
| The electricity price used (€278/MWh, all business consumers) may be higher than what energy-intensive firms pay | Kept for consistency with Part 1; the Excel file recalculates everything if the team changes it |

---

## 10. Going beyond the brief

Five things most teams will not bring:

1. **A tool, not only slides.** The Excel calculator answers "what would my plant gain?" in front of a client. Reply's sales team can reuse it the day after the presentation.
2. **A pilot contract on one page** (annex below). It turns "conditional pilot" from an idea into something a client could sign.
3. **Reply's own measure of success.** We show revenue per consultant, not software metrics. It answers the objection "we are a consulting firm" before it is raised.
4. **Kill criteria.** We say what would prove us wrong within 6 months: pilot conversion below 30 %, measured gain below 2 % of the bill, or no partner signed.
5. **Named targets and real voices.** Twenty real companies from the official list, checked for plants and solar (Part 1's open task), and two quotes from an energy manager and an ESCO.

### Annex: the conditional pilot on one page

| Term | Proposal |
|---|---|
| Scope | One plant, about 3 months, the agents for solar self-consumption and load shifting |
| Before the start | Baseline measured by the digital twin; 2 or 3 KPIs agreed in writing (for example: share of solar used on site, cost per MWh consumed) |
| Price | €20k, at cost |
| If the KPIs are met | The client signs the managed service for that plant; the €20k is credited against set-up |
| If the KPIs are not met | No obligation for the client; Reply keeps the data for its benchmarks, with consent |
| What Reply promises | Best effort and a measured result. No guaranteed saving |
| After the pilot | One more plant each year; bonus of 15 % on measured savings, upside only |

---

## 11. To confirm before Thursday

| Open point | Who can answer |
|---|---|
| Size of a typical project today, and how many pilots convert | Sense Reply (questions 2 and 3 of the follow-up email) |
| Would Reply accept a variable bonus? | Sense Reply (question 8) |
| Share of consumption a plant can really move in time | Energy manager interview |
| Would an ESCO pay €4k per plant for a white-label platform? | ESCO or aggregator interview |
| Share of the 860 targets with solar and flexible loads | Part 1's 20-name check |
| Wording: Part 1 and Part 2 say "white-label licence"; the brief asks us not to call the contract a licence | Team decision: we use "white-label platform fee" |

## 12. Sources

- Team briefing (13 Nov 2026), Part 1 (Segmentation & ICP), Part 2 (Competitor analysis), Part 3 kick-off brief, Sense Reply case brief.
- Solar output, export prices: https://www.solareindustriale.it/incentivi/ritiro-dedicato ; https://www.solareindustriale.it/progetti/impianto-fotovoltaico-1-mw
- Self-consumption case of a manufacturing site: https://www.me.camcom.it/sites/default/files/contenuto_redazione/notizie/file/usecase_manifattura_ur_sicilia.pdf
- Daily price gap in Italy: https://www.electricitymaps.com/grid-in-review-2025/italy ; https://pexapark.com/blog/with-macse-the-italian-bess-market-looks-to-stability-instead-of-merchant-upside/
- Network charge on peak power (medium voltage, 2026): https://www.e-distribuzione.it/content/dam/e-distribuzione/a-chi-ci-rivolgiamo/venditori/2026/MTA3.pdf
- Capacity market price for 2027: https://www.ess-news.com/2025/02/28/terna-energy-storage-capacity-auction-2027-delivery-results/
- Measured savings in 83 plants: https://eta-publications.lbl.gov/publications/deeper-and-persistent-energy-savings
