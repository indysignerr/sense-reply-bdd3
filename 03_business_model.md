# Deliverable 3 — Business model (working draft)

> Status: **working draft, 13 Nov 2026**.
> **Client facts** = what Sense Reply told the team. **Hypotheses** = ours, to confirm.
> The numbers in §5 come from `03_revenue_scenarios.xlsx` (change the blue cells, everything recalculates).

---

## 1. What we now know about how Sense Reply sells (client facts)

| Fact | Source |
|---|---|
| The platform is **customised for each client**, with options | Team Q&A with Sense Reply |
| Clients get a **3-month test period** before signing | Team Q&A |
| Contracts then run **3 years**, around **€1M per year**, with a **€200k minimum spend** | Team Q&A |
| Reference 1: **Aeroporti di Roma** (Fiumicino and Ciampino). A cloud-native IoT platform built with AWS that collects and standardises data from airport assets, for monitoring and predictive maintenance | Reply case study and news, Oct 2026 |
| Reference 2: a platform that manages **energy consumption and generation**, and decides **when to buy and sell** | Team Q&A (client name unknown) |

**Three points to confirm with Sense Reply before we build on them**

1. **What do "€1M" and "€200k" mean exactly?** Our reading: the client commits to at least €200k per year, and a typical full contract reaches about €1M per year with options and usage. If instead €1M is the standard price, the revenue floor is 5 times higher.
2. **Is the 3-month test free or paid?** It changes the economics a lot (see §4).
3. **How many such contracts are signed today?** One, three, ten?

---

## 2. What these facts change in our analysis

**a) The "product or service?" question is already half answered.** A platform customised per client and sold on 3-year contracts is neither a pure product nor a pure service. It is a **product core with a service wrap**. The real question becomes: *how much of each contract is standard, and how much is custom?* The more custom, the less it scales.

**b) The price filters the market.** A client paying €200k to €1M per year needs to get much more than that in value.

Illustrative calculation (our assumptions: the client wants 3 times its money back, the platform saves 10 % of the energy bill, electricity at €100/MWh):

| Yearly fee | Value needed (3×) | Energy bill needed (10 % savings) | Consumption needed |
|---|---|---|---|
| €200k (minimum) | €600k | €6M | ≈ 60 GWh per year |
| €1M (full contract) | €3M | €30M | ≈ 300 GWh per year |

Consequences:
- **Energy savings alone rarely justify the price for a single site.** A factory at the EED threshold (23.6 GWh per year, about €2.4M of electricity) would save about €240k: barely the minimum fee.
- The value must come from **several sources at once**: energy cost, flexibility revenue, avoided maintenance and downtime (the Rome airport case is about asset maintenance, not energy), avoided grid investment for DSOs, compliance.
- **Direct targets are large accounts only**: DSOs, utilities and aggregators, large infrastructure (airports, ports), multi-site industrial groups. Energy communities and mid-size companies cannot be direct clients at this price. They need a partner channel or a lighter offer.

**c) Infrastructure sites move up in our segmentation.** We had scored "microgrids and closed sites" low (2.95). With Aeroporti di Roma as a live reference, Sense Reply's right to win there is high. Revised score: 3.40 (see `01_segmentation_ICP.md`).

---

## 3. Business Model Canvas

| Block | Content |
|---|---|
| **Customer segments** | **Direct (large accounts, ≥ €200k per year):** 1) flexibility aggregators and utilities operating asset fleets; 2) distribution system operators (DSOs); 3) large infrastructure sites: airports, ports, industrial parks; 4) energy-intensive multi-site industrial groups. **Indirect (through partners):** energy communities, mid-size companies, building portfolios |
| **Value propositions** | **Aggregators / utilities:** onboard new sites faster, run and secure the whole fleet from one place, optimise when to buy, sell and store energy. **DSOs:** see and steer the distribution grid in real time without new hardware, on a platform built on the grid data standard (CIM) and designed for cyber rules. **Infrastructure sites:** one view of all assets, predictive maintenance, energy optimisation, sites keep running if the connection drops. **Industry:** lower energy bill, one dashboard across sites, compliance with energy-management rules. **For all:** works with equipment from different manufacturers; business logic can be customised |
| **Channels** | Reply group account managers (cross-selling to existing Reply clients); direct enterprise sales with a CEO-level sponsor; AWS co-selling and AWS Marketplace; partners for smaller clients (energy service companies, battery and solar integrators); the 3-month test as the conversion step; reference cases (Aeroporti di Roma, demand-response platforms) |
| **Customer relationships** | Co-design during the test period; dedicated delivery team; 3-year contract with a steering committee; a customer-success role to prepare the renewal from year 2; shared savings dashboard ("where the money goes") |
| **Revenue streams** | Today: 3-year contracts, about €1M per year, €200k minimum spend. **Proposed structure:** 1) platform fee (the committed minimum); 2) optional modules; 3) usage fee per gateway or asset above an included volume; 4) integration and customisation projects; 5) optional success fee where savings can be measured |
| **Key resources** | The platform and its IoT accelerator (RIPA); energy and grid experts; library of connectors to field equipment; client references; AWS partnership; the Reply group client base |
| **Key activities** | Platform development; client integration and customisation; running trials; security and compliance (AI Act, cyber rules); customer success and renewals |
| **Key partners** | AWS (cloud, co-selling); gateway hardware makers; AI model providers (Mistral and others); battery, solar and charger manufacturers; energy service companies and integrators; other Reply companies; regulators and industry bodies for standards |
| **Cost structure** | Engineers building the platform; consultants delivering integration and customisation (largest variable cost); cost of trials that do not convert; cloud costs (to confirm: paid by Sense Reply or by the client?); sales and marketing; compliance and certification |

---

## 4. Pricing: three options and our recommendation

| Option | How it works | Strengths | Weaknesses |
|---|---|---|---|
| **A. Status quo: fully custom contract** | Free or cheap 3-month test, then a tailored 3-year contract | Fits each client; high contract value | Every deal is a project; cost of failed trials; hard to scale beyond the delivery team; price is opaque |
| **B. Modular: core + options + usage** (recommended) | Fixed platform fee (the €200k minimum) + priced modules + fee per gateway above an included volume; customisation billed as a project | Predictable recurring revenue; clear price list; grows with the client's fleet; partners can resell it | Needs discipline to keep the core standard; some clients will still ask for custom work |
| **C. Pay for results** | Fee = share of measured savings or flexibility revenue | Removes the "slow return on investment" objection raised at the kickoff | Needs an agreed baseline; revenue is uncertain; hard for regulated DSOs. Use only as an **optional add-on** for industrial energy optimisation |

**Recommendation: option B, with two changes to the current practice**

1. **Turn the 3-month test into a paid pilot**, credited against year 1 if the client signs. Reason: a customised trial costs real consultant time. With our illustrative figure of €144k per trial (3 people for 3 months, our guess) and one trial in two converting, each signed contract carries about **€288k of trial cost**. A paid pilot also filters out clients who are not serious.
2. **Standard core, custom edges.** Keep the platform core identical for all clients. Limit customisation to modules and connectors, and bill it separately. This is what turns a consulting project into a product.

How the pieces map to what Sense Reply already does:

| Price element | Role | Link to today's contract |
|---|---|---|
| Paid pilot (3 months) | Proves value on one site or one use case | Replaces the test period |
| Platform fee | Core platform, security, a set number of gateways | = the €200k minimum spend |
| Modules | Asset monitoring, energy optimisation and trading, EV charging, demand response, energy communities | = the "options" |
| Usage fee | Per gateway or asset above the included volume | Explains the path from €200k to €1M |
| Projects | Integration, connectors, custom applications | Reply's consulting business |
| Success fee (optional) | Share of measured savings | New |

---

## 5. Revenue scenarios 2027–2031

Source: `03_revenue_scenarios.xlsx`. **All inputs except the minimum spend are team hypotheses.**

| Input | Conservative | Base | Ambitious |
|---|---|---|---|
| Average contract value per year | €300k | €500k | €800k |
| Trials started per year (2027 → 2031) | 2 → 5 | 4 → 12 | 6 → 18 |
| Trials that become contracts | 40 % | 50 % | 60 % |
| Renewal after 3 years | 70 % | 80 % | 90 % |

| Result | Conservative | Base | Ambitious |
|---|---|---|---|
| Contracts signed over 5 years | 7 | 20 | 36 |
| Expected revenue in 2027 | €0.1M | €0.5M | €1.4M |
| Expected revenue in 2029 | €0.8M | €3.5M | €10.1M |
| **Expected revenue in 2031** | **€1.7M** | **€8.2M** | **€24.0M** |
| Committed floor in 2031 (minimum spend only) | €1.2M | €3.3M | €6.0M |
| 5-year expected revenue | €4.4M | €19.6M | €57.0M |
| 5-year cost of trials (if free, at €144k each) | €2.6M | €5.8M | €8.6M |
| Trial cost as a share of revenue | 59 % | 29 % | 15 % |

**What the scenarios show**

- **Revenue builds slowly.** Even in the base case, year 1 brings €0.5M. Long sales cycles and mid-year starts delay everything. The plan needs patience from Reply's management.
- **Only part of the revenue is guaranteed.** In the base case, €3.3M of the €8.2M expected in 2031 is contractually committed. The rest depends on clients buying options and adding gateways.
- **Free trials are expensive when conversion is low.** In the conservative case, trials cost 59 % of revenue. This is the strongest argument for a paid pilot.
- **Few contracts, high concentration.** 20 contracts in 5 years means that losing two renewals removes about 10 % of the client base.

**What the model does not include:** delivery, R&D, cloud and sales costs. We have no data on them, so this is a revenue model, not a profit plan.

---

## 6. Main risks to the business model

| Risk | Why it matters | Mitigation |
|---|---|---|
| Too much customisation | Each client becomes a separate product; growth is capped by the number of consultants | Standard core; custom work only in modules and connectors, billed separately |
| Free trials | High cost per signed contract when conversion is low | Paid pilot credited against year 1 |
| Low committed share | Only the minimum spend is guaranteed | Raise the minimum for large clients; include more gateways in the base fee |
| Client concentration | A few large contracts carry the business | Add a partner channel for smaller clients in a second phase |
| Dependence on AWS | AWS is both partner and potential competitor | Keep the platform portable; use AWS as a sales channel |
| AI rules for grid operators | Agents acting on the grid may be classed high-risk under the AI Act | Human validation by default for DSO use cases |
| Internal conflict at Reply | Product revenue vs. consultant-day revenue | Show that each contract still carries integration projects |

---

## 7. Questions to ask Sense Reply to firm this up

1. What do the €1M and the €200k cover exactly? Is the €200k a yearly commitment?
2. Is the 3-month test paid? How many tests turn into contracts?
3. How many 3-year contracts are active today, and in which segments?
4. In a typical contract, how is the yearly amount split between licence, options, usage and consultant days?
5. Who pays the cloud bill: Sense Reply or the client?
6. How many trials can the team run at the same time?
7. Has any client renewed after 3 years yet?

---

## 8. Sources

- Team Q&A with Sense Reply (contract length, price, minimum spend, test period, references).
- Reply case study, Aeroporti di Roma: https://www.reply.com/en/iot/adr-ottimizza-la-gestione-intelligente-degli-asset-aeroportuali-con-ai-e-iot
- Reply news, 1 Oct 2026 (Fiumicino and Ciampino): https://www.reply.com/it/newsroom/news/sense-reply-potenzia-gestione-predittiva-infrastrutture-aeroportuali-roma-fiumicino-ciampino-iot-ai
- EED threshold (85 TJ ≈ 23.6 GWh): see `01_segmentation_ICP.md`, §8.
