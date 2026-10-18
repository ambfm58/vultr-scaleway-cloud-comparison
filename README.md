# vultr vs scaleway: Where Each Cloud Wins on Price, Performance, and EU Data Residency (Plus Which Plans Are Actually Worth It)

Vultr and Scaleway show up on the same "affordable AWS alternative" lists, but they're built for different jobs. Vultr, launched in 2014 out of New Jersey, is a global operator with 32+ regions across six continents, selling hourly-billed compute to developers anywhere. Scaleway is a French cloud provider with all of its zones inside Europe, no US presence, and a sovereignty pitch backed by French SecNumCloud qualification and a recent European Commission contract to deliver sovereign cloud and AI services to EU institutions.

Because of that, a vultr vs scaleway search usually resolves on one question before price even comes up: where are your users? A founder in Berlin with a mostly German audience has a genuinely different best answer than a SaaS team with customers in Sydney, São Paulo, and Toronto. This piece covers both sides — the real monthly cost including fees that don't show in headline pricing, what independent benchmarks actually graded, how the two startup programs filter applicants, and Vultr's full Cloud Compute lineup with current prices.

> **The 60-second version**
> - Users spread across the world → Vultr. Cloud Compute starts at $3.50/mo (512 MB) or $5/mo for 1 vCPU/1 GB with 1 TB transfer, IPv4 included, deployable in 32+ regions. 👉 [Check Vultr's current Cloud Compute prices](https://www.vultr.com/pricing/?ref=7268283)
> - Users in Europe with GDPR or sovereignty requirements → Scaleway. Paris, Amsterdam, Warsaw (Milan on the most recent check), plus GDPR, ISO 27001, SecNumCloud in select regions, and HDS health-data hosting.
> - Startup credits: a funded (Series A+) company migrating workloads qualifies for Vultr's program — up to $100,000 in credits plus up to 35% off long-term. An EU-incorporated team at idea stage qualifies for Scaleway's staged vouchers (€1,000 to €36,000).

## Vultr vs Scaleway at a glance

Neither provider sweeps this comparison, and the split is consistent: Vultr wins wherever geography and per-plan pricing clarity matter, Scaleway wins wherever EU compliance and bandwidth costs matter.

|  | Vultr | Scaleway |
| --- | --- | --- |
| Regions | 32+ across six continents | A few European zones: Paris, Amsterdam, Warsaw (Milan on the latest check) |
| Cheapest listed compute | $3.50/mo (512 MB; $2.50 IPv6-only) | DEV1-S instance ~€6.55/mo, roughly €11.15 all-in with IPv4 and storage |
| 2 vCPU / 4 GB class | from $20/mo (3 TB transfer) | €16.79/mo (BASIC2-A2C-4G, unlimited transfer) |
| Transfer overage | billed per GB, rate varies by data center (around $0.01/GB) | no egress fees on instances (unmetered per-instance speed) |
| Disk performance | A grade on the VX1 GP line | F grade on the tested POP2 plan (block storage) |
| Compliance | SOC 2, GDPR | GDPR, ISO 27001, SecNumCloud (select regions), HDS |
| Uptime SLA | 100% network uptime | 99.9–99.99% depending on product tier |
| Free tier / credit | limited early-access free plan | no free tier; €100 credit for new Professional accounts |

## Data center coverage: the category that settles most decisions

Vultr wins coverage by a wide margin, and for a lot of projects that alone answers the question. Latency is physics — a server in Warsaw will always feel faster to a Warsaw user than one in Mumbai, and no pricing trick changes that.

Vultr runs 32–33 regions: eleven cities in North America (Atlanta, Chicago, Dallas, Los Angeles, Miami, New Jersey, Seattle, Silicon Valley, Honolulu, Toronto, Mexico City), plus São Paulo and Santiago in South America, nine in Europe (Amsterdam, Frankfurt, London, Madrid, Manchester, Milan, Paris, Stockholm, Warsaw), three in India, six in Asia-Pacific (Tokyo, Osaka, Seoul, Singapore, Sydney, Melbourne), plus Tel Aviv and Johannesburg. Vultr's own marketing claims this footprint puts roughly 90% of the world's population within 2–40 ms of a server.

Scaleway's map is deliberately smaller: zones in Paris, Amsterdam, and Warsaw, with Milan appearing in the most recent September 2026 check. Nothing in the Americas, Asia, Africa, or the Middle East.

A Berlin developer running a side project loses nothing here — Paris or Amsterdam means sub-15 ms pings, GDPR-aligned hosting, and no transatlantic data hops. A product with users on three continents is a different story; Scaleway simply can't serve it. If your audience is global, the decision makes itself. If it's European, keep reading, because Scaleway gets more interesting from here.

## What you actually pay each month

Sticker prices favor Vultr at the low end; the real bill depends on add-ons Scaleway doesn't put on the front page and one thing Vultr doesn't put there either.

Scaleway prices instances à la carte. The DEV1-S instance lists around €6.55, but a flexible IPv4 adds €3.65/mo (IPv6 is free) and block storage runs about €0.095/GB/mo. Realistic all-in cost: **≈€11.15/mo** for the DEV1-S (2 shared vCPU, 2 GB), ≈€25.65 for a PLAY2-NANO (2 shared vCPU, 4 GB), and ≈€45.75 for a PLAY2-MICRO (4 shared vCPU, 8 GB), all ex-VAT. Vultr bundles IPv4 into its plan prices — $5/mo gets you 1 vCPU, 1 GB RAM, 25 GB SSD, and 1 TB transfer; $20/mo gets 2 vCPU, 4 GB, 80 GB SSD, and 3 TB.

The trade: Scaleway charges no egress fees on instances. Bandwidth is an unmetered per-instance speed. Vultr's included transfer (1–6 TB on the plans tested) is generous, but overage is billed per GB at a rate that varies by data center — around $0.01/GB in the models most comparisons use. A project pushing 3 TB/month on Vultr's 1 TB-transfer plan adds roughly $20/mo in overage; on Scaleway, nothing extra.

Fine print worth knowing before you commit to either:

- Scaleway's dedicated Kubernetes control plane is a paid add-on at roughly €80/mo, above the free shared control plane.
- Windows on Scaleway runs about 2.5x the price of the equivalent Linux instance variant. On Vultr, Windows licensing is also billed outside the base price.
- Scaleway's "no egress" applies to instance bandwidth — Object Storage traffic gets 75 GB free per month, then €0.01/GB, and restoring from its cold storage tier costs €0.009/GB. Snapshots are billed separately per GB-hour.
- Commitment discounts differ: Scaleway's Savings Plans take up to 25% off compute for 12- or 36-month commitments. Vultr's comparable long-term discount (up to 35%) exists mainly through its startup program.

On a light-traffic project, Vultr usually comes out ahead on total cost. Past a couple of terabytes of monthly transfer inside Europe, Scaleway's zero-egress model starts winning. 👉 [See Vultr's plan list and included transfer](https://www.vultr.com/pricing/?ref=7268283)

## Vultr plans and pricing: the full Cloud Compute lineup

Vultr's core Cloud Compute line starts at $3.50/mo and scales up through Regular, High Frequency, High Performance, CPU Optimized, and the newer VX1 lines. Here are the plans people actually compare, with prices as independently verified:

| Plan | Config | Transfer | Price/mo | Purchase |
| --- | --- | --- | --- | --- |
| Cloud Compute Regular 512 MB | 512 MB RAM | – | $3.50 ($2.50 IPv6-only) | [ Get this plan](https://www.vultr.com/pricing/?ref=7268283) |
| Cloud Compute 1 GB | 1 vCPU · 1 GB · 25 GB SSD | 1 TB | $5 | [ Get this plan](https://www.vultr.com/pricing/?ref=7268283) |
| High Frequency 1 GB | 1 vCPU · 1 GB · 32 GB | 1 TB | $6 | [ Get this plan](https://www.vultr.com/pricing/?ref=7268283) |
| Regular 2 GB | 1 vCPU · 2 GB · 55 GB | 2 TB | $10 | [ Get this plan](https://www.vultr.com/pricing/?ref=7268283) |
| High Performance 2 GB | 1 vCPU · 2 GB · 50 GB | 3 TB | $12 | [ Get this plan](https://www.vultr.com/pricing/?ref=7268283) |
| High Performance 4 GB | 2 vCPU · 4 GB · 100 GB | 5 TB | $24 | [ Get this plan](https://www.vultr.com/pricing/?ref=7268283) |
| CPU Optimized 2-4-50 | 2 vCPU · 4 GB · 50 GB | 5 TB | $40 | [ Get this plan](https://www.vultr.com/pricing/?ref=7268283) |
| Regular 8 GB | 4 vCPU · 8 GB · 160 GB | 4 TB | $40 | [ Get this plan](https://www.vultr.com/pricing/?ref=7268283) |
| High Performance 8 GB | 4 vCPU · 8 GB · 180 GB | 6 TB | $48 | [ Get this plan](https://www.vultr.com/pricing/?ref=7268283) |
| VX1 GP 2C 8G 50S | 2 vCPU · 8 GB · 50 GB | 5 TB | $48.80 | [ Get this plan](https://www.vultr.com/pricing/?ref=7268283) |
| VX1 GP 2C 8G 120S | 2 vCPU · 8 GB · 120 GB | – | $55.48 | [ Get this plan](https://www.vultr.com/pricing/?ref=7268283) |
| VX1 GP 4C 16G 240S | 4 vCPU · 16 GB · 240 GB | 6 TB | $110.16 | [ Get this plan](https://www.vultr.com/pricing/?ref=7268283) |

A few notes on reading this table:

- Billing is hourly against these monthly caps.
- Every line above continues to larger sizes, and Vultr also runs separate Bare Metal, Managed Database, Object Storage, and GPU catalogs, plus managed Kubernetes.
- The early-access free plan (1 vCPU, 512 MB RAM, 10 GB disk) is hosted in Seattle, Frankfurt, or Miami. Confirm it's actually enabled in your account before building anything on it.
- Bandwidth overage varies by data center, and IPv4 comes included on Cloud Compute plans.

One judgment call: Vultr's $6–12 entry plans graded mostly D in benchmark testing (the $10 Regular plan even picked up an E in web performance). That's typical for shared-CPU budget boxes, but it means the cheap tiers are a bad sample of what Vultr's faster lines do. Judge the lineup by the High Performance and VX1 rows instead. 👉 [Compare Vultr's High Performance and VX1 plans](https://www.vultr.com/pricing/?ref=7268283)

## Performance: what independent benchmarks actually show

In VPSBenchmarks' testing, Vultr's VX1 GP line posts the strongest results of either provider, Scaleway's BASIC2 is the budget standout, and Scaleway's block storage is the one category to avoid depending on.

The headline result: the Vultr VX1 GP 2C 8G 120S ($55.48/mo) earned a B in web performance, an A in stability (17.1/20), and an A in disk IO (17.7/20) — the strongest single result across the plans tested from both providers. Scaleway's POP2-HC-2C-4G (€45.20/mo) managed a B in web performance (11.6/20) but a D in stability and an F in disk IO. The benchmark write-up notes block storage has historically been Scaleway's weak point, so that F isn't a surprise.

The budget side is where Scaleway fights back. Its BASIC2-A2C-4G at €16.79 (2 vCPU, 4 GB, unlimited transfer) graded C in web performance and B in stability, and costs roughly half of a comparable Vultr plan. Vultr's counterargument lives higher up the lineup, in the High Performance and VX1 tiers.

Two secondary metrics are worth a glance. Plan consistency — how much two identical servers of the same plan can differ — came in at 65 for Scaleway and 61 for Vultr, effectively a tie. Provisioning averaged 30 seconds for Scaleway versus 85 for Vultr, though Scaleway's figure comes from a two-instance sample against Vultr's twelve, so treat it as directional rather than definitive.

Aggregated user reviews lean slightly toward Scaleway: one 2026 aggregation of G2, Capterra, and Software Advice scores puts Vultr at 4.2 across roughly 850 reviews and Scaleway at 4.5 across about 397. Reviewer comments on Vultr circle around fast provisioning, an easy console, and price-to-performance; on Scaleway, around EU data residency and cheap entry-level instances.

Practical read: match the plan line to the workload. Vultr's VX1 GP is the pick when disk IO and stability matter — databases, busy web apps. Scaleway's BASIC2 is the efficiency pick for EU-hosted workloads that aren't disk-bound. Neither provider's cheapest tier represents what it can actually do.

## Startup programs: geography gates one, funding gates the other

The two startup programs filter for entirely different things. Scaleway asks where your company is incorporated; Vultr asks how much you've raised.

| Your situation | Series A or later | Pre-Series A |
| --- | --- | --- |
| EU-incorporated | Both programs open | Scaleway only |
| Incorporated elsewhere | Vultr only | Neither — start on standard plans |

Scaleway's program runs in tiers tied to consumption: a one-time €1,000 Founders voucher valid 12 months, then either the Early Stage track (€1,500/mo for 6 months, €9,000 total, expecting around €500/mo of real spend) or the Growth track (€3,000/mo for 12 months, €36,000 total, expecting around €1,500/mo). Credits cover H100 and L40S GPUs, managed AI services, object storage, and Kubernetes, and training data stays in the EU by default. No equity changes hands.

Vultr's program is a single, bigger, negotiated deal: up to $100,000 in credits calculated against the invoices you bring, plus up to 35% in ongoing discounts that persist after the credits run out. GPU credits include H100, A100, GH200, and L40S. The gate is strict, though — a recent Series A through E round, six months of cloud invoices, and an executive contact, because the program is built around migrating existing workloads rather than starting new ones.

The headline gap, $100,000 versus about $40,000, flatters Vultr for early teams. An idea-stage EU startup can't enter Vultr's program at all, so its realistic comparison is Scaleway's €9,000 Early tier versus nothing. Only funded European startups face a genuine either/or, and for them Vultr's standing 35% discount is usually worth more over three years than Scaleway's capped monthly vouchers.

## Frequently asked questions

**Does Vultr have a free tier?**
Yes, as a limited early-access plan: 1 vCPU, 512 MB RAM, and 10 GB disk, hosted in Seattle, Frankfurt, or Miami. Availability has to be confirmed inside your account — don't build launch plans around it until you see it there.

**Which one is cheaper for a small website?**
For low-traffic sites, Vultr: $5/mo buys 1 vCPU, 1 GB RAM, 25 GB SSD, 1 TB transfer, and an IPv4 address with nothing billed separately. Scaleway's closest equivalent, the DEV1-S, comes to roughly €11.15 all-in. The math flips for bandwidth-heavy European projects, where Scaleway's zero egress fees beat Vultr's per-GB overage.

**Do powered-off servers stop billing?**
On Vultr, no — hourly billing continues until you destroy the instance, so an idle but powered-off server still costs its full plan price. Scaleway handles this better: a fully powered-off (archived) instance stops compute billing, though attached IPs and volumes keep charging.

**Is managed Kubernetes available on both?**
Yes. The cost difference to know: Scaleway's free option uses a shared control plane, and upgrading to a dedicated control plane with a higher SLA runs about €80/month.

## So, Vultr or Scaleway?

Run your situation through these rules and the answer usually falls out in one line:

- Users outside Europe, or split across continents → Vultr. Scaleway has no region that can serve them, and no roadmap fixes latency.
- EU-only users with regulated data — health data, public sector, strict sovereignty → Scaleway. SecNumCloud and HDS certifications are things Vultr doesn't offer.
- Small site, light traffic, simplest possible bill → Vultr's $3.50–$5 tier, with IPv4 and transfer included and a free early-access tier to test with.
- Bandwidth-heavy project with a European audience → Scaleway. Unmetered per-instance speed beats paying around $0.01/GB in overage.
- Best tested performance for the money → Vultr's VX1 GP line for disk and stability; Scaleway's BASIC2-A2C-4G at €16.79 for a cheap 2 vCPU/4 GB box.
- Funded startup migrating workloads → Vultr's program. EU idea-stage team → Scaleway's vouchers.

Three details to confirm before you click buy on either side: whether the Vultr free tier is actually enabled in your account, what the bandwidth overage rate is for your specific Vultr region, and how Scaleway's ex-VAT pricing fits your accounting. None of these are dealbreakers. They're just the things that show up on invoice two rather than invoice one.

If the global-footprint side of the argument is what sold you, 👉 [pick your Vultr region and plan here](https://www.vultr.com/pricing/?ref=7268283) — VPSBenchmarks' average says the server will be up in about 85 seconds.
