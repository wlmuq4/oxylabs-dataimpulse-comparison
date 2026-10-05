# oxylabs review: the real per-GB ladder, the fees that aren't on the hero banner, and when a $5 pay-as-you-go pool is the better buy

Most people searching "oxylabs review" aren't deciding whether Oxylabs is a serious proxy company. It obviously is. They're trying to answer one narrower question before they put a card down: at my volume, is the premium actually doing anything for me, or am I buying an enterprise pool to scrape 15 GB a month?

That question has a fairly clean answer, and it isn't the same answer for a 5 GB project and a 1 TB pipeline. So this breaks down what Oxylabs charges, what its self-serve plans actually include, where the friction sits after checkout, and where a $1/GB pay-as-you-go provider like DataImpulse covers the same job for a fraction of the spend.

## The short version, for people who scroll

Oxylabs is a Lithuanian proxy and scraping infrastructure company founded in 2015, now part of the Tesonet group alongside Decodo (formerly Smartproxy). It advertises 175M+ residential IPs across 195 countries, 2M+ datacenter IPs, compliant sourcing, SOC 2 Type II certification, and KYC verification on new accounts.

Its self-serve residential plans reward commitment. Hard. The entry plan is the worst rate on the page, the pricing page and the navigation banner disagree with each other, and the cheap per-GB numbers most comparison articles quote belong to a tier that costs $2,500 a month.

If your monthly residential traffic is under roughly 100 GB and your targets aren't on Oxylabs' blocked list, you're paying enterprise prices for a mid-size job.

## The residential price ladder, read carefully

Oxylabs' site is genuinely confusing on price, because three different headline numbers describe three different things. You'll see $4/GB quoted as the advertised floor, $6/GB on the entry plan card, and $2.50/GB in the navigation. None of those is wrong; they just belong to different tiers, and two of them require four-figure monthly commitments.

Here's what the self-serve plan cards read in late 2026, per multiple independent price checks:

| Plan | Monthly volume | Monthly price | Effective rate |
| --- | --- | --- | --- |
| Starter | 5 GB | $30 | $6.00/GB |
| Basic | 20 GB | $100 | $5.00/GB |
| Advanced | 125 GB | $500 | $4.00/GB |
| Corporate | 1 TB | $2,500 | $2.50/GB |
| Custom enterprise | Above 1 TB | Negotiated | Below $2.50/GB |

Two things jump out of that table. First, the gap between Basic and Advanced is 20 GB to 125 GB, with nothing in between. If you need 50 GB, you buy the 20 GB plan and top up the rest at the 20 GB plan's rate, which is worse than the 125 GB rate you can't quite justify. Reviewers flag this as the single most common complaint from mid-sized buyers, and it's easy to see why.

Second, VAT is added on top of every published price. Depending on where you're billing from, that's a meaningful premium on numbers that already sit above most of the field.

Worth knowing too: pay-as-you-go on residential isn't a real no-commitment balance. The genuinely free-form per-GB option is the shared datacenter pool (reported at roughly $0.44 to $0.65/GB depending on volume), while residential is monthly plans you top up from the dashboard.

## Where Oxylabs earns the money

It would be dishonest to write this as a takedown. There are real reasons the company keeps showing up at the top of enterprise shortlists.

- **Pool scale.** 175M+ residential IPs is the largest reported count in the market; DataImpulse advertises 90M+. If your job needs deep coverage in Tier-3 geographies, that difference shows up.
- **Benchmark placement.** Proxyway's annual market research has repeatedly ranked Oxylabs at or near the top of the enterprise category, and it wins proxy awards more years than not. Independent test write-ups consistently report infrastructure success rates around 99.9% and average response times in the 0.6-second range.
- **Datacenter and ISP are the cheap corner.** Dedicated datacenter starts at $2.25 per IP from three IPs ($6.75/month), and five datacenter IPs come free at signup. For a small fixed set of addresses, that's the lowest entry ticket in the category.
- **Success-based billing on the Scraper API.** Failed requests in the 5xx and 6xx range aren't charged. Web Scraper API plans start at $49/month, with pricing that reaches around $0.25 per 1,000 results on large tiers, and the output comes parsed rather than as raw HTML. Web Unblocker is listed at $5/GB, currently discounted around 40% to $3/GB.
- **Documentation and integrations.** SDKs, GitBook docs, Postman collections, cloud storage delivery, and an analytics dashboard with per-sub-user bandwidth caps. If you're running a team, that plumbing is worth real money.

## The blocked-target list almost nobody mentions

This is the detail that reframes the whole price comparison, and it sits in the FAQ on Oxylabs' own residential pricing page.

> Oxylabs restricts its residential network from a published list of targets, including all Apple domains (App Store, iTunes), banking and financial institutions, several Google domains, government sites, streaming platforms, ticketing and mailing services. The restriction applies on every plan, including the $2,500/month tier.

If your target is on that list, per-GB pricing is irrelevant. You can sign a 1 TB contract and still not be allowed to point the pool at it. Before buying, name your exact targets to support in writing and get a documented answer. Ten minutes of chat beats a month of committed spend.

## The friction that shows up after checkout

Three billing and onboarding terms matter more than most reviews admit:

1. **The refund window is three calendar days**, self-service plans only, and you must have used under 20% of your traffic. Processing takes up to 15 business days. Miss the window and the money is gone; pay-as-you-go purchases are not refundable.
2. **KYC is a time cost.** New accounts go through verification, which gates advanced residential filters and certain restricted targets. Reviewers routinely describe onboarding delays measured in days, sometimes longer, especially on free email domains. If you needed proxies working this afternoon, this is the wrong vendor for this afternoon.
3. **Review scores diverge by audience.** Platform aggregates for oxylabs.io sit in the low 4s and G2 shows roughly 4.5, but the distribution is bimodal, and one widely-read September 2026 breakdown logged 3.7 out of 5 across 713 Trustpilot reviews. The pattern inside that split is consistent: enterprise accounts with a named manager are delighted, self-serve buyers hitting billing and metering disputes are not. Trustpilot complaints include disputed bandwidth accounting and duplicate charges, both of which Oxylabs has publicly replied to.

## Who Oxylabs actually fits

Buy it if you're running sustained, high-volume residential traffic above roughly 500 GB a month, you need SOC 2 and ISO paperwork for procurement, your targets are outside the blocked list, and your downside from a failed scrape is measured in lost contracts rather than mild annoyance. The datacenter and ISP lines are a separate, genuinely cheap case worth evaluating on their own.

Skip it, or at least price the alternative properly, if any of these describe you:

- You consume under about 100 GB of residential traffic a month
- Your volume swings month to month (seasonal scraping, campaign sprints, QA gaps)
- You want to test a target list before committing budget
- You're a solo developer or small team without a compliance process to satisfy

For that second group, the subscription model is the problem, not the pool quality. You're buying a bundle and paying for whatever you don't finish.

## The pay-as-you-go alternative: DataImpulse at $1/GB

DataImpulse is the other end of this market, and it's the company the affiliate link on this page points to. It's worth being precise about what that means: a flat $1/GB residential rate with no subscription, a $5 minimum, and traffic that never expires. Unused gigabytes sit in your account until you use them, which matters if your scraping is lumpy.

The pool is 90M+ ethically sourced IPs across 195 countries, sourced first-party through DataImpulse's own opt-in participant app rather than resold from another network. Country, state, city, ZIP, and ASN targeting are bundled at the base rate with rotating and sticky sessions configurable from 1 to 120 minutes (the realistic average is around 30, because residential devices go offline). HTTP(S) and SOCKS5 are both supported, and the sticky-session behaviour is documented honestly rather than presented as a defect.

Worth knowing before you buy: advanced targeting filters (city, ZIP, ASN) consume roughly double the traffic, so treat those requests at an effective $2/GB. And DataImpulse is a young company. It doesn't carry SOC 2 or ISO 27001, its Tier-3 geographic depth is thinner than Oxylabs', and its support operation is smaller. If a procurement questionnaire is part of your purchase, that's a real blocker.

Here's the full current lineup.

**Residential proxies** — 90M+ IPs, 195 countries, non-expiring traffic

| Plan | Traffic | Price | Rate | Billing | Buy |
| --- | --- | --- | --- | --- | --- |
| Intro (new users) | 5 GB | $5.00 | $1.00/GB | One-off, no subscription | 5 GB for $5 |
| Basic | 50 GB | $50.00 | $1.00/GB | One-off, no subscription | Get the 50 GB plan |
| Advanced | 1 TB (1,000 GB) | $800.00 | $0.80/GB | One-off, no subscription | Get 1 TB at $0.80/GB |
| Custom | 5 TB+ | From $4,000 | Negotiated | One-off, no subscription | Ask about 5 TB+ pricing |

**Datacenter proxies** — speed-first pool, no subnet blocks

| Plan | Traffic | Price | Rate | Billing | Buy |
| --- | --- | --- | --- | --- | --- |
| Intro (new users) | 10 GB | $5.00 | $0.50/GB | One-off, no subscription | 10 GB of datacenter traffic for $5 |
| Basic | 100 GB | $50.00 | $0.50/GB | One-off, no subscription | Get the 100 GB datacenter plan |
| Advanced | 1 TB (1,000 GB) | $450.00 | $0.45/GB | One-off, no subscription | Get 1 TB of datacenter traffic |
| Custom | 5 TB+ | From $2,250 | Negotiated | One-off, no subscription | Request a custom datacenter quote |

**Mobile proxies** — 5G/4G/3G/LTE carriers, rotating and sticky sessions

| Plan | Traffic | Price | Rate | Billing | Buy |
| --- | --- | --- | --- | --- | --- |
| Intro (new users) | 2.5 GB | $5.00 | $2.00/GB | One-off, no subscription | Start mobile proxies at $5 |
| Basic | 25 GB | $50.00 | $2.00/GB | One-off, no subscription | Get the 25 GB mobile plan |
| Advanced | 1 TB (1,000 GB) | $1,600.00 | $1.60/GB | One-off, no subscription, dedicated account manager | Get 1 TB of mobile traffic |
| Custom | 5 TB+ | From $8,000 | Negotiated | One-off, no subscription | Request a custom mobile quote |

**Premium residential proxies** — highest-quality pool, personal account manager

| Plan | Traffic | Price | Rate | Billing | Buy |
| --- | --- | --- | --- | --- | --- |
| Intro (new users) | 1 GB | $5.00 | $5.00/GB | One-off, no subscription | Test premium residential for $5 |
| Basic | 10 GB | $50.00 | $5.00/GB | One-off, no subscription | Get the 10 GB premium plan |
| Advanced / Custom | 1 TB+ | From $4,000 | From $4.00/GB | One-off, no subscription | Request premium residential pricing |

A few terms worth flagging. Intro plans carry a 7-day money-back guarantee on card payments, provided you've consumed less than 80% of the traffic; crypto purchases on Intro plans are not refundable. There's no free tier, so $5 is the real entry cost. Payment methods include cards via Stripe, PayPal, wire transfer, Alipay, Apple Pay, Google Pay, and four cryptocurrencies via Cryptomus. Live chat is staffed by humans rather than a bot queue, and G2 reviews for DataImpulse sit around 4.7 to 4.8 across a modest review base of 28.

## Oxylabs vs DataImpulse, without the spin

|  | Oxylabs | DataImpulse |
| --- | --- | --- |
| Residential entry cost | $30 for 5 GB | $5 for 5 GB |
| Residential rate at 100 GB/month | $500 (125 GB plan) | $100 (flat $1/GB) |
| Traffic expiry | Not published; ask support | Documented: never expires |
| Commitment | Monthly subscription minimum | None, top up anytime |
| Residential pool | 175M+ claimed | 90M+ claimed |
| Certifications | SOC 2 Type II, ISO/IEC 27001 | None yet |
| Managed unblocker | Yes, Web Unblocker | No |
| Per-result scraper API | Yes, failures not charged | No |
| Advanced targeting | Country, city, state, ASN, ZIP | Country, city, ZIP, ASN — billed at ~2x traffic |
| Tier-3 geo depth | Strong | Thinner |
| Support model | Live chat, email, named account manager | Live chat with human agents |

Read that table honestly: they're not competing for the same buyer. Oxylabs wins on pool size, certifications, managed anti-bot tooling, and the ability to survive a compliance review. DataImpulse wins on cost per gigabyte below enterprise volumes, on not charging you for bandwidth you didn't burn, and on a $5 test that tells you within an afternoon whether the IPs get blocked on your targets.

## Practical call

**Run Oxylabs if** your targets are hard, your volume is high, and you have procurement requirements to satisfy. Start with the datacenter lines (five free IPs, $6.75 for three dedicated) to test the network before committing to a residential tier, and get your target domains confirmed against the blocked list in writing first.

**Run DataImpulse if** you're under roughly 100 GB a month, your workload is uneven, or you want proof before a contract. Buy 5 GB for $5, point it at the sites you actually scrape, and measure the failure rate yourself. A $1/GB pool that fails 40% of requests costs more per usable page than a $3/GB pool that fails 5%, so the test is the point, not the sticker price.

**Consider both if** you're at mid-volume with a mix of easy and hard targets: route the long tail of ordinary domains through the cheap pool and reserve the expensive one for the handful of hosts that actually block you. That split is where most budgets get saved, and it's the approach neither vendor's marketing page is going to suggest.

## FAQ

**Does Oxylabs have a free trial?**
A 7-day trial is advertised on several products, with limited bandwidth, and enterprise prospects can request an extended proof of concept. Several reviews note the trial is more of a smoke test than a real evaluation, and access still runs through KYC, so confirm current terms with support before you plan around it.

**What's the minimum spend at Oxylabs?**
On residential self-serve, $30 for 5 GB. Dedicated datacenter starts at $6.75/month for three IPs, and five datacenter IPs are free at signup.

**Does Oxylabs offer true pay-as-you-go on residential?**
Only on the shared datacenter pool, billed per GB. Residential is monthly plans topped up from the dashboard with unused traffic treated differently from a no-expiry balance.

**Can I get a refund?**
Self-service plans, within three calendar days of your first transaction, under 20% of traffic used, up to 15 business days to process. Pay-as-you-go purchases aren't refundable.

**Is $1/GB realistic for residential proxies?**
Yes, within limits. DataImpulse holds that flat rate from 5 GB to 50 GB with a $5 minimum, which is why it tops most cheap-residential comparisons. The catch is scale and depth: 90M+ IPs and thinner Tier-3 coverage versus 175M+ at Oxylabs, and advanced geo filters that double the effective rate.

**Which is better for someone scraping a few hundred pages a day?**
Almost certainly the pay-as-you-go option. You'd be paying a $30 monthly minimum for a plan sized for a workload several times larger, before VAT. Paying for exactly what you use is the cheaper structure until your volume becomes predictable and heavy.

The honest summary: Oxylabs is priced for teams whose scraping failures show up on a P&L, and it delivers at that level. If that isn't you yet, 👉 test DataImpulse for $5 and let your own success rates make the argument.
