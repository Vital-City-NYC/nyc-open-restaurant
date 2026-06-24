# Methodology — How to open a restaurant in New York City

An interactive, sourced flowchart of every step, agency, fee and timeline involved in opening a sit-down restaurant in New York City. Single self-contained file: `index.html` (no build step, no dependencies).

## Scope

Models a **first-time, single-location, sit-down restaurant** in a space already zoned for eating and drinking (Use Group 6). Week 0 assumes a lease is signed and financing is in place.

## Data sources

Every figure on the page links to its source. Primary sources:

| Figure | Source |
|---|---|
| Steps, 22-day rule, permit fee ($280 + $25 frozen desserts), Food Protection Course, pre-permit inspection, Certificate of Authority and insurance requirements | NYC DOHMH, [Opening a Restaurant](https://www.nyc.gov/site/doh/business/food-operators/opening-a-restaurant.page); NYC Business, [Food Service Establishment Permit](https://nyc-business.nyc.gov/nycbusiness/description/food-service-establishment-permit) |
| Construction sequence, DOB Alteration permits, Certificate of Occupancy, FDNY hood suppression, per-step week ranges | Park Bench Architects, [Opening a Restaurant in NYC: Step-by-Step Guide](https://parkbencharchitects.com/opening-a-restaurant-in-nyc-step-by-step-guide-permits-inspections-and-common-pitfalls/) |
| Liquor license fee ($4,352 full on-premises NYC), 6–10 month timeline, 500-foot rule, 30-day community board notice, temporary permit | NYS Liquor Authority, [Restaurant License Quick Reference](https://sla.ny.gov/restaurant-license-quick-reference-0) and [retail license fee chart](https://sla.ny.gov/retail-license-fee-chart) |
| Outdoor dining license ($1,050 per café type / 4 years, up to 6-month review) | NYC DOT, [Dining Out NYC fees](https://www.diningoutnyc.info/apply/fees) |

## Assumptions & calculations

- **Timeline axis:** 0–32 weeks (~7.4 months), measured from lease signing. Month ticks placed at `month * 4.345 weeks`.
- **Gantt bar position:** `left = weekStart / 32`, `width = (weekEnd − weekStart) / 32`, minimum 4% width for legibility.
- **Parallelism:** Steps overlap in reality; bars are drawn at their independent typical windows rather than stacked sequentially.
- **Dashed bars** (liquor, outdoor dining) flag items that commonly extend past opening day.

## Confidence

- **High:** Government fees and statutory rules (22-day operating window, 500-foot rule, 30-day community board notice). Taken verbatim from official city/state pages.
- **Medium:** Week-by-week durations. These are practitioner estimates and vary widely by project — planning guides, not commitments.

## Limitations

- Processing times shift; verify with the agency before relying on them.
- Not every step applies to every restaurant (outdoor dining, liquor, Place of Assembly for 75+, Landmarks review are conditional).
- Fees are government application/permit fees only — they exclude rent, construction, professional fees and insurance.
- Current as of June 2026; rule changes after that date are not reflected.

## Last reviewed

June 2026.
