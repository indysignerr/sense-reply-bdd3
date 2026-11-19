# Sense Reply case — Every number in the business case, and where it comes from

**Albert School BDD #3 · Case B1 · 19 November 2026**

This document lists every number used in the business case (the Excel model, the simulator and the presentation) and explains how we got it, including the estimates. Use it when someone asks "where does this number come from?".

## How to read it

Each number has a status:

| Code | Meaning | How much to trust it |
|---|---|---|
| **TD** | Taken from a team document (Part 1, Part 2 or the briefing) | As reliable as that document. We did not re-check it unless stated |
| **PS** | Public source found during our research | Reliable, but several were read from search summaries, not from the full document |
| **A** | Our assumption: we chose the value because no data exists | Weakest. Defend it as an assumption, never as a fact |
| **P** | Our proposal: a price we recommend | A choice, not a measurement |
| **C** | Calculated from the numbers above | As reliable as its inputs |

Sense Reply gave us no price, no contract value, no conversion rate and no figure on how much work is reused between projects. Everything about Reply's economics is therefore **A** or **P**.

Part 10 lists the numbers we trust least.

---

## 1. The market (slide 4)

| Number | Value | How we got it | Status |
|---|---|---|---|
| Electricity price paid by Italian companies | €278 per MWh | Part 1, citing Confindustria on Eurostat and GME data, first half of 2025, all business consumers | TD |
| EU average | €216 per MWh | Same source | TD |
| Germany, France, Spain | €242, €183, €171 | Same source | TD |
| Italy above the EU average | +29% | 278 ÷ 216 − 1 = 28.7% | C |
| Companies on Italy's official energy-intensive list | 5,253 | Part 1, CSEA list, 2024 | TD |
| In the five target sectors | 3,011 | Part 1: food and beverage 953, plastics 1,187, chemicals 303, ceramics and glass 394, paper 174 | TD |
| Their electricity use | 42,213 GWh a year | Part 1, same list | TD |
| Medium or large | about 2,290 | 3,011 × 76% (list-wide average share) | TD |
| Based in Northern Italy | about 1,730 | 2,290 × 75.5% (list-wide average share) | TD |
| Fit the ideal customer | about 860 | 1,730 × 50%. The 50% is a team estimate of firms with several sites, solar and flexible loads | TD, with an **A** inside |
| Won in 3 years | about 25 | 860 × 3%. The 3% is a team target | TD, with an **A** inside |
| Segment scores | 4.30, 4.20, 4.10, 3.45 | Part 1: 12 segments scored from 1 to 5 on 8 weighted criteria | TD, team judgement |

**Caution on €278.** We could not confirm this figure ourselves. A search found other values for the same period: about €190 per MWh for the EU average and about €203 for Italian industrial consumers, on different definitions. Energy-intensive firms also receive reductions on charges. We kept €278 so that the three parts of our work stay consistent. Part 9 shows what changes at a lower price.

---

## 2. The typical plant (slide 6)

| Number | Value | How we got it | Status |
|---|---|---|---|
| Electricity per company | about 14 GWh a year | 42,213 GWh ÷ 3,011 companies = 14.0 | C |
| Plants per typical account | 3 | Part 1 says 2 to 10 plants. We took a low, round value | A |
| Electricity per plant | 5 GWh a year | About 15 GWh ÷ 3 plants | C |
| Electricity bill of the plant | €1,390,000 | 5,000 MWh × €278 | C |
| Solar on the roof | 1 MWp | Team briefing: "typical factory, 1 MWp of solar" | TD |
| Battery | None | Part 2: most Italian sites have solar but no battery | TD |
| Solar output | 1,100 MWh a year | A commercial source gives 900 to 1,250 MWh a year for a 1 MW plant in Italy. We took the middle | PS |
| Share of solar sent to the grid today | 20% | Two public cases: 19% at a manufacturing site, 45% at a small plant. We took the low end, which is cautious for our gain | A |
| Solar sent to the grid | 220 MWh | 1,100 × 20% | C |

---

## 3. What the plant gains (slide 6)

### 3.1 The inputs behind the three cases

| Input | Cautious | Base | Optimistic | How we got it | Status |
|---|---|---|---|---|---|
| Share of exported solar that agents bring back on site | 30% | 50% | 70% | No data found. Half is our central guess | A |
| Share of consumption that can be moved in time | 5% | 10% | 15% | No clean figure for Italian plants. A European project modelled 20% as a scenario; we stay below it | A |
| Price gap between expensive and cheap hours | €39 | €60 | €88 per MWh | Low: average daily price swing in Italy in 2025 (Electricity Maps). High: gap captured by a 4-hour battery in mid-2025 (Pexapark). Base: between the two | PS for low and high, A for base |
| Peak reduction | 5% | 10% | 15% | No data found | A |
| Flexible power offered, per GWh consumed | 20 kW | 40 kW | 60 kW | Base = 200 kW for a 5 GWh plant, one fifth of its peak | A |

### 3.2 The fixed inputs

| Input | Value | How we got it | Status |
|---|---|---|---|
| Price received for exported solar | €100 per MWh | No single figure. Anchors: a guaranteed minimum of about €47 per MWh, and a source saying a kWh used on site is worth 2 to 3 times an exported one (278 ÷ 3 ≈ 93) | A |
| Peak power of the plant | 1,000 kW (200 kW per GWh) | 5 GWh ÷ 8,760 hours = 571 kW on average. We assumed the peak is a little under twice the average | A |
| Network charge on peak power | €28.35 per kW per year | e-distribuzione medium-voltage tariff "MTA3", 2026: €28.3493 | PS |
| Revenue for flexible power | €47,000 per MW per year | Italian capacity market, auction for 2027. One source says €46,000. Used as a benchmark, not as a contract price | PS |
| Share kept after the aggregator's cut | 70% | Part 2 says aggregators take a revenue share but gives no percentage | A |

### 3.3 The calculation, base case

| Line | Formula | Result |
|---|---|---|
| Solar brought back on site | 220 MWh × 50% | 110 MWh |
| **1. Using its own solar** | 110 MWh × (€278 − €100) | **€19,580** |
| Consumption that can be moved | 5,000 MWh × 10% | 500 MWh |
| **2. Moving consumption to cheap hours** | (500 − 110) MWh × €60. We subtract the 110 MWh already counted in line 1 | **€23,400** |
| **3. Lower peaks** | 1,000 kW × 10% × €28.35 | **€2,835** |
| **4. Selling flexibility** | 0.2 MW × €47,000 × 70% | **€6,580** |
| **Total gain** | Sum of the four | **€52,395** |
| Share of the bill | 52,395 ÷ 1,390,000 | 3.8% |

### 3.4 The three cases

| | Cautious | Base | Optimistic |
|---|---|---|---|
| 1. Using its own solar | €11,748 | €19,580 | €27,412 |
| 2. Moving consumption | €7,176 | €23,400 | €52,448 |
| 3. Lower peaks | €1,418 | €2,835 | €4,253 |
| 4. Selling flexibility | €3,290 | €6,580 | €9,870 |
| **Total gain** | **€23,632** | **€52,395** | **€93,983** |
| Share of the bill | 1.7% | 3.8% | 6.8% |

All **C**. On the slides these are rounded to €24k, €52k and €94k.

### 3.5 The check against a real measurement

| Number | Value | How we got it | Status |
|---|---|---|---|
| Measured savings in plants with an energy management system | 3 to 4% a year | Study of 83 US manufacturing plants by Lawrence Berkeley National Laboratory: 4.1% in the first year, 3.4% after twelve years | PS |

Our base case (3.8%) sits in that range. The study measures energy saved; our figure is money gained, partly by using energy at better times. It is a sanity check, not a proof.

---

## 4. The prices (slide 7)

| Number | Value | How we got it | Status |
|---|---|---|---|
| Managed service fee | €10,000 per plant per year | Set so that Reply's total take is about one third of the base gain. Equal to €833 a month, which is 3 to 4 times the market signal in Part 2 ($200 to $300 per site per month for energy software with services) | P |
| Fee as a share of the bill | 0.7% | 10,000 ÷ 1,390,000 | C |
| Success bonus | 15% of measured savings | Chosen with the fee to reach one third of the gain, with most of Reply's revenue fixed | P |
| Set-up, first plant | €30,000 | Our estimate of integration work for a first site | P, weakly grounded |
| Set-up, each further plant | €12,000 | 40% of the first, because agents and connectors are reused | P |
| Conditional pilot | €20,000 | About 25 days of work at about €800 a day. Both figures are ours | P, built on an **A** |
| White-label platform fee | €4,000 per plant per year | 40% of the direct fee, because the partner sells and installs | P, the least grounded price |
| Minimum per partner | 25 plants | Gives a minimum of €100,000 a year per partner | P |
| Co-innovation project with a large group | €100,000 a year | Stands for Reply's project business today. No real figure available | A |

### What follows from these prices

| Number | Cautious | Base | Optimistic | Formula |
|---|---|---|---|---|
| Bonus | €3,545 | €7,859 | €14,097 | 15% × gain |
| **Paid to Reply per plant per year** | **€13,545** | **€17,859** | **€24,097** | €10,000 + bonus |
| Reply's share of the gain | 57% | 34% | 26% | Paid ÷ gain |
| **Kept by the client** | **€10,087** | **€34,536** | **€69,885** | Gain − paid |
| Gain for each euro paid | 1.7 | 2.9 | 3.9 | Gain ÷ paid |
| First year of the first plant, set-up included | −€19,913 | +€4,536 | +€39,885 | Gain − €30,000 − paid |

On the slides: "€18k", "€35k", "one third", "about €3 for every €1".

---

## 5. What one account brings Reply (slide 7, and the figure for Part 1)

### Typical account: 3 plants, one more each year

| | Year 1 | Year 2 | Year 3 |
|---|---|---|---|
| Plants running | 1 | 2 | 3 |
| Set-up | €30,000 | €12,000 | €12,000 |
| Fee and bonus | €17,859 | €35,719 | €53,578 |
| **Revenue** | **€47,859** | **€47,719** | **€65,578** |

Average over 3 years: **€53,719**, shown as "€54k". The roll-out of one plant a year is an **A**.

### Lighthouse account: a large group with 10 plants

Plants running: 2, then 5, then 10 (an **A**; 10 plants is the top of Part 1's range). Revenue = set-up + fee and bonus on running plants + €100,000 of co-innovation.

| | Year 1 | Year 2 | Year 3 |
|---|---|---|---|
| Revenue | €177,719 | €225,296 | €338,593 |

Average: **€247,202**, shown as "€247k".

### Partner

Plants in the partner's fleet: 25, then 50, then 75 (an **A**). Revenue = plants × €4,000: €100,000, €200,000, €300,000. Average: **€200,000**.

"One partner is worth almost four direct accounts": 200,000 ÷ 53,719 = 3.7.

### The market in euros per year

| Step | Companies | × revenue per account | Result |
|---|---|---|---|
| Five sectors | 3,011 | × €53,719 | €162M |
| Medium or large, Northern Italy | 1,730 | × €53,719 | €93M |
| Ideal customers | 860 | × €53,719 | €46M |
| Won in 3 years | 25 | × €76,937 | €1.9M |

€76,937 is the average for the 25 accounts if 3 of them are lighthouse accounts: (3 × 247,202 + 22 × 53,719) ÷ 25. The "3 of 25" is an **A**.

---

## 6. The three-year comparison (slide 8)

### 6.1 The assumptions

| Input | Today's model | Two-speed model | Status |
|---|---|---|---|
| Pilots started in years 1, 2, 3 | 10, 16, 18 | 10, 16, 18 | A. Chosen so that our model reaches Part 1's 25 accounts |
| Pilots that become contracts | 30% | 50% | A. Reply gave no figure |
| Large groups signed per year | 1 | 1 | A |
| Plants per typical account | 3, all in the year of signing | 1, then 2, then 3 | A |
| Partners signed per year | None | 1, 2, 3 | A |
| Plants lost each year | None | 5% of last year's plants | A |
| Yearly revenue per plant | €10,000, no bonus | €17,859 | P and C |
| Set-up per plant | €30,000 for every plant | €30,000 first, €12,000 after | P |
| Days per pilot | 40, free | 25, paid | A |
| Days to set up a plant | 40 | 15 after the pilot | A |
| Days per plant per year to run the service | 8 | 5 | A |
| Days to onboard a partner | — | 30 | A |
| Days per partner plant per year | — | 1 | A |
| Days of co-innovation per large group per year | 150 | 150 | A |
| Working days per person per year | 200 | 200 | A |

"Today's model" is our reconstruction from one meeting. The same prices are used in both models so that only the way of selling differs.

### 6.2 Two-speed model, year by year

| Volumes | Year 1 | Year 2 | Year 3 | Formula |
|---|---|---|---|---|
| Typical accounts signed | 5 | 8 | 9 | Pilots × 50% |
| Their plants running | 5 | 18 | 40 | One more plant per account each year |
| Their plants paying, after losses | 5.0 | 17.8 | 38.9 | Minus 5% of last year's plants |
| Large-group plants running | 2 | 7 | 17 | 2, 5, 10 per group |
| Partners signed | 1 | 2 | 3 | Input |
| Partner plants paying, after losses | 25 | 98.8 | 243.8 | 25, 50, 75 per partner, minus 5% |

| Revenue (€ thousand) | Year 1 | Year 2 | Year 3 | Formula |
|---|---|---|---|---|
| Pilot fees from clients that do not sign | 100 | 160 | 180 | Pilots × 50% × €20,000 |
| Set-up, typical accounts | 150 | 300 | 426 | First plants × €30,000 + further plants × €12,000 |
| Fee and bonus, typical accounts | 89 | 317 | 694 | Plants paying × €17,859 |
| Set-up, large groups | 42 | 78 | 138 | Same rule |
| Fee and bonus, large groups | 36 | 125 | 304 | Plants running × €17,859 |
| Co-innovation | 100 | 200 | 300 | Groups active × €100,000 |
| Partner fees | 100 | 395 | 975 | Partner plants paying × €4,000 |
| **Total** | **617** | **1,575** | **3,017** | |

| People | Year 1 | Year 2 | Year 3 |
|---|---|---|---|
| Days of work | 595 | 1,253 | 1,993 |
| People needed (days ÷ 200) | 3.0 | 6.3 | 10.0 |
| **Revenue per person** | €207k | €251k | **€303k** |

Year 3 days in detail: pilots 18 × 25 = 450 · first plants 10 × 15 = 150 · further plants 22 × 15 = 330 · running 55.9 plants × 5 = 279 · onboarding 3 partners × 30 = 90 · partner plants 243.8 × 1 = 244 · co-innovation 3 × 150 = 450. Total 1,993.

### 6.3 Today's model, year by year

| | Year 1 | Year 2 | Year 3 | Formula |
|---|---|---|---|---|
| Typical accounts signed | 3 | 4.8 | 5.4 | Pilots × 30% |
| Their plants running | 9 | 23.4 | 39.6 | 3 plants per account, all at once |
| Integration, typical accounts (€k) | 270 | 432 | 486 | New plants × €30,000 |
| Yearly service, typical accounts (€k) | 90 | 234 | 396 | Plants running × €10,000 |
| Integration, large groups (€k) | 60 | 150 | 300 | New plants × €30,000 |
| Yearly service, large groups (€k) | 20 | 70 | 170 | Plants running × €10,000 |
| Co-innovation (€k) | 100 | 200 | 300 | Same as our model |
| **Total revenue (€k)** | **540** | **1,086** | **1,652** | |
| Days of work | 1,078 | 1,959 | 2,671 | Pilots × 40 + new plants × 40 + plants running × 8 + co-innovation |
| People needed | 5.4 | 9.8 | 13.4 | Days ÷ 200 |
| **Revenue per person** | €100k | €111k | **€124k** | |

Fractions of accounts (4.8, 5.4) are averages, not real deals.

### 6.4 The headline numbers

| Number on the slide | Today | Two-speed | How |
|---|---|---|---|
| Revenue per year | €0.5M, €1.1M, €1.7M | €0.6M, €1.6M, €3.0M | Totals above, rounded |
| 3-year revenue | €3.3M | €5.2M | 540 + 1,086 + 1,652 = 3,278 · 617 + 1,575 + 3,017 = 5,209 |
| Recurring share, year 3 | 34% | 65% | (396 + 170) ÷ 1,652 · (694 + 304 + 975) ÷ 3,017 |
| Revenue per person, year 3 | €124k | €303k | Tables above |
| Accounts signed in 3 years | 16 | 25 | 13.2 + 3 · 22 + 3 |
| Plants on the platform, year 3 | 57 | 300 | 39.6 + 17 · 38.9 + 17 + 243.8 |
| Plants through partners | — | 244 of 300 | 243.8 |
| Partner share of year-3 revenue | — | 32% | 975 ÷ 3,017 |
| Pilot days given for free | 1,760 | 0 | (10 + 16 + 18) × 40 |

All **C**, built on the **A** and **P** inputs of 6.1.

---

## 7. The stress test (slide 8 buttons and backup slide)

Each scenario changes one input and keeps the others at the base case. We recalculated every line with the team model.

| Scenario | What we changed | 3-year revenue | Revenue per person, year 3 |
|---|---|---|---|
| Base case | Nothing | €5.2M | €303k |
| Only 30% of pilots convert | Conversion 50% → 30% | €4.6M | €296k |
| No partner at all | Partners signed 1, 2, 3 → 0, 0, 0 | €3.7M | €246k |
| Both | The two changes together | €3.1M | €230k |
| Cautious plant gain | Gain €52k → €24k, so fee and bonus €17,859 → €13,545 | €4.8M | €279k |
| No time saved by reusing agents | Days set to today's values: pilot 40, every plant 40, running 8 | €5.2M | €187k |
| Today's model | — | €3.3M | €124k |

What it shows: the result depends most on the days saved by reuse. It depends least on the conversion rate.

---

## 8. The slider on slide 6

The slider changes the plant's electricity use from 2 to 20 GWh. Solar stays at 1 MWp, so line 1 does not move. Lines 2, 3 and 4 use the formulas of part 3 with the new size.

| Plant | Cautious | Base | Optimistic | Base: share of the bill | Base: paid to Reply | Base: kept by the client |
|---|---|---|---|---|---|---|
| 2 GWh | €15k | €29k | €46k | 5.2% | €14k | €14k |
| 5 GWh | €24k | €52k | €94k | 3.8% | €18k | €35k |
| 10 GWh | €38k | €92k | €174k | 3.3% | €24k | €68k |
| 20 GWh | €67k | €171k | €334k | 3.1% | €36k | €135k |

Example, base case at 10 GWh: solar €19,580 · moving consumption (1,000 − 110) × €60 = €53,400 · peaks 2,000 kW × 10% × €28.35 = €5,670 · flexibility 0.4 MW × €47,000 × 70% = €13,160 · total €91,810.

---

## 9. What happens if the electricity price is lower

Only line 1 depends on the price paid. If the plant pays €200 per MWh instead of €278:

| | At €278 | At €200 |
|---|---|---|
| 1. Using its own solar | €19,580 | 110 × (200 − 100) = €11,000 |
| Lines 2, 3 and 4 | €32,815 | €32,815 |
| **Total gain, base case** | **€52,395** | **€43,815** |
| Share of the bill | 3.8% | 4.4% of €1.0M |
| Paid to Reply | €17,859 | €16,572 |
| Kept by the client | €34,536 | €27,243 |

The model still holds: the gain falls by about 16%.

---

## 10. The numbers we trust least

| Rank | Number | Why it is weak | What would fix it |
|---|---|---|---|
| 1 | Days saved by reusing agents (40 → 15 days per plant) | Reply said it has no figure on reuse. It drives the revenue per person most | A real figure from Sense Reply |
| 2 | Share of consumption that can be moved (10%) | No data for Italian plants. It drives 45% of the gain | One energy manager interview, or the pilot |
| 3 | Today's conversion rate (30%) and ours (50%) | Pure assumptions | Sense Reply's real rate |
| 4 | €278 per MWh | Not confirmed by our own search; an average for all businesses | The original Confindustria table |
| 5 | White-label fee (€4,000) and partner growth (25 plants a year) | No market reference found | One ESCO or aggregator interview |
| 6 | Set-up prices (€30,000 and €12,000) and pilot (€20,000) | Built on our guess of days and day rates | Sense Reply's real project sizes |
| 7 | Price for exported solar (€100) | Varies by hour and by contract | A real invoice |
| 8 | The 50% and 3% in the funnel | Team estimates | A check on 20 names from the list |

---

## 11. Numbers on the competitor slide (slide 5)

All come from Part 2. We did not re-check them.

| Number | Value | Status |
|---|---|---|
| Price of cloud device management | About $0.16 per device per month | TD (Part 2, from the provider's price page). Also seen in our own search |
| Kraken valuation at its spin-out | $8.65bn, 2025 | TD |
| Centrica bought REstore | 2017 | TD |
| Shell bought Next Kraftwerke | 2021 | TD |
| E.ON took full control of gridX | 2022 | TD |
| Commercial storage connected in Italy | 91 MWh in the first quarter of 2026 | TD |
| EU AI Act, high-risk rules for critical infrastructure | From 2 December 2027 | TD. Our own search found sources disagreeing on this date |
| Competitor matrix | 11 players, 9 dimensions | TD, team judgement |

---

## 12. The roadmap numbers (slide 9)

| Number | Value | How we got it | Status |
|---|---|---|---|
| Pilots in the first 6 months | 5 | Half of year 1's 10 pilots | C |
| Accounts, partners and plants at month 36 | 25, 6, about 300 | From the three-year model: 22 + 3 accounts, 1 + 2 + 3 partners, 300 plants | C |
| Target: pilot conversion | 50% | Our model's input | A |
| Target: plants per account | 3 | Our model's input | A |
| Target: recurring share | 65% | Result of the model in year 3 | C |
| Target: revenue per person | €300k | Result of the model in year 3, rounded | C |
| Stop if conversion stays under | 30% | Today's assumed rate: below it, the conditional pilot adds nothing | A |
| Stop if the measured gain is under | 2% of the bill | Just above the cautious case (1.7%), where Reply would take more than half the gain | A |

---

## 13. Sources

**Team documents:** team briefing (13 November 2026) · Part 1, Client Segmentation & ICP · Part 2, Competitor & Alternative Solutions Analysis · Part 3 kick-off brief.

**Public sources found during our research**

- Solar output and export prices: https://www.solareindustriale.it/incentivi/ritiro-dedicato and https://www.solareindustriale.it/progetti/impianto-fotovoltaico-1-mw
- Self-consumption at a manufacturing site: https://www.me.camcom.it/sites/default/files/contenuto_redazione/notizie/file/usecase_manifattura_ur_sicilia.pdf
- Daily price swing in Italy, 2025: https://www.electricitymaps.com/grid-in-review-2025/italy
- Gap captured by a 4-hour battery: https://pexapark.com/blog/with-macse-the-italian-bess-market-looks-to-stability-instead-of-merchant-upside/
- Network charge on peak power, 2026: https://www.e-distribuzione.it/content/dam/e-distribuzione/a-chi-ci-rivolgiamo/venditori/2026/MTA3.pdf
- Capacity market, auction for 2027: https://www.ess-news.com/2025/02/28/terna-energy-storage-capacity-auction-2027-delivery-results/
- Measured savings in 83 plants: https://eta-publications.lbl.gov/publications/deeper-and-persistent-energy-savings
- Share of industrial demand modelled as flexible: https://europeanenergyinnovation.eu/Latest-Research/Winter-2017/IndustRE-Can-the-industrial-sector-enable-the-grid-integration-of-renewables
- Other price figures seen for the same period: https://www.eunews.it/en/2026/05/18/fossil-fuels-and-poor-interconnectivity-italy-had-the-most-expensive-electricity-among-eu-countries-in-2025/

**The model itself:** `Part3_business_model.xlsx` (sheets Inputs, Site ROI, Pricing, 3-year numbers). Every number in this document can be recalculated there.
