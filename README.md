# London VPS: real prices from $2.50, hourly billing, and an honest comparison with five UK hosting rivals

Type "london vps" into Google and page one is a wall of small UK-focused hosts selling fixed monthly plans between £9.99 and $14.99. That works fine if you already know exactly what you need. What most of those pages don't tell you is that Vultr sells London capacity differently: hourly billing, no contract, entry plans from **$2.50 a month**, and the same cloud compute catalog in more than 30 regions. That changes the comparison math, because you can run a real London server for a weekend for roughly 40 cents before committing to anything. This article walks through Vultr's full London price list, puts it next to the five rivals currently ranking for this search, and covers the details their sales pages tend to skip — bandwidth overage, Windows fees, renewal pricing, and what deployment actually involves.

> **If you're in a hurry:** for most readers the most flexible option is Vultr's High Performance plan at **$6/month** — 1 vCPU, 1 GB RAM, 25 GB NVMe, 1 TB traffic, billed hourly so you can destroy the server whenever you like. 👉 [Check Vultr's current London pricing](https://www.vultr.com/pricing/?ref=7268283). If you'd rather have a fixed monthly box with DDoS protection bundled in, OliveVPS ($3.99, Linux-only) and LogicWeb ($10 with 2 vCPUs and 4 GB) beat Vultr on entry-level specs; Cloudzy's $2.48 listing (50% off) is the cheapest sticker price and comes with a 14-day money-back window.

## What a London VPS is actually for

A London location makes sense in three cases: your audience is in the UK, you need an IP that geolocates to the UK, or your compliance requirements say data has to sit on UK soil.

On latency, UK visitors typically see single-digit millisecond response times, and the major western EU hubs — Paris, Amsterdam, Frankfurt — fall in the 10–20 ms range. London is also where LINX sits, one of the world's largest internet exchange points, and the UK is a landing region for transatlantic subsea cables, which is part of why finance and trading operations cluster there. If your users are in North America or Asia, London is simply the wrong region for you. Vultr's multi-region setup makes that a non-issue: the plans below can be deployed in any of its locations, so you can pick the city your visitors actually live near.

## Vultr's London plans: the full cloud compute price list

Vultr runs the same cloud compute plans across all of its regions, so what you get in London (region code LHR) is identical to New York or Singapore — same specs, same hourly billing model, billed by the hour up to a fixed monthly cap. Two shared-CPU lines are available: Regular Performance on Intel with SSD storage, and High Performance with NVMe storage and newer processors. Here's the full published lineup.

**Cloud Compute — Regular Performance (Intel, SSD):**

| Monthly price | vCPU | RAM | Storage | Traffic | Deploy |
| --- | --- | --- | --- | --- | --- |
| $2.50 | 1 | 512 MB | 10 GB SSD | 0.5 TB | [ Deploy $2.50 plan](https://www.vultr.com/products/cloud-compute/?ref=7268283) |
| $5 | 1 | 1 GB | 25 GB SSD | 1 TB | [ Deploy $5 plan](https://www.vultr.com/products/cloud-compute/?ref=7268283) |
| $10 | 1 | 2 GB | 55 GB SSD | 2 TB | [ Deploy $10 plan](https://www.vultr.com/products/cloud-compute/?ref=7268283) |
| $20 | 2 | 4 GB | 80 GB SSD | 3 TB | [ Deploy $20 plan](https://www.vultr.com/products/cloud-compute/?ref=7268283) |
| $40 | 4 | 8 GB | 160 GB SSD | 4 TB | [ Deploy $40 plan](https://www.vultr.com/products/cloud-compute/?ref=7268283) |
| $80 | 8 | 16 GB | 320 GB SSD | 5 TB | [ Deploy $80 plan](https://www.vultr.com/products/cloud-compute/?ref=7268283) |
| $160 | 16 | 32 GB | 640 GB SSD | 6 TB | [ Deploy $160 plan](https://www.vultr.com/products/cloud-compute/?ref=7268283) |
| $320 | 24 | 64 GB | 1280 GB SSD | 10 TB | [ Deploy $320 plan](https://www.vultr.com/products/cloud-compute/?ref=7268283) |

**Cloud Compute — High Performance (NVMe):**

| Monthly price | vCPU | RAM | Storage | Traffic | Deploy |
| --- | --- | --- | --- | --- | --- |
| $6 | 1 | 1 GB | 25 GB NVMe | 1 TB | [ Deploy $6 plan](https://www.vultr.com/pricing/?ref=7268283) |
| $12 | 1 | 2 GB | 60 GB NVMe | 2 TB | [ Deploy $12 plan](https://www.vultr.com/pricing/?ref=7268283) |
| $24 | 2 | 4 GB | 100 GB NVMe | 3 TB | [ Deploy $24 plan](https://www.vultr.com/pricing/?ref=7268283) |
| $48 | 4 | 8 GB | 200 GB NVMe | 4 TB | [ Deploy $48 plan](https://www.vultr.com/pricing/?ref=7268283) |
| $96 | 8 | 16 GB | 400 GB NVMe | 5 TB | [ Deploy $96 plan](https://www.vultr.com/pricing/?ref=7268283) |
| $192 | 16 | 32 GB | 800 GB NVMe | 6 TB | [ Deploy $192 plan](https://www.vultr.com/pricing/?ref=7268283) |

A few details worth knowing before you pick a row:

- Every instance includes a dedicated IPv4 address and a routed /64 IPv6 subnet.
- Traffic beyond the included quota costs $0.01 per GB.
- Need a core nobody else can touch? Optimized Cloud Compute starts at $28/month (one fully dedicated vCPU, 4 GB RAM, 25 GB NVMe), and bare metal is available if you want an entire machine to yourself.
- OS images cover Ubuntu, Debian, AlmaLinux, Rocky Linux, Fedora, FreeBSD and Windows Server; Windows adds a monthly license fee, shown before you confirm the deploy. Custom ISO uploads are supported, and it's all KVM with full root access.
- Automatic backups add 20% to the instance price. The cloud firewall and private networking (VPC) are free.
- Always-on DDoS mitigation is a paid add-on, listed at $10/month per instance — more on why that matters below.

Vultr occasionally adjusts storage sizes or adds tiers, so treat this as a snapshot and verify on the live page before ordering. 👉 [Open Vultr's cloud compute page for the current spec grid](https://www.vultr.com/products/cloud-compute/?ref=7268283).

## How Vultr compares with the five London hosts you'll actually find

On sticker price, Vultr undercuts everyone on this list. On raw hardware per dollar at the entry level, it loses to LogicWeb and FyfeWeb. Both statements are true, and which one matters depends on how you'll use the server.

| Host | Entry price | What you get at entry | Billing | Standout detail |
| --- | --- | --- | --- | --- |
| Vultr | $2.50/mo | 1 vCPU, 512 MB, 10 GB SSD, 0.5 TB | Hourly, no contract | Same plans in 30+ regions |
| Cloudzy | $2.48/mo (50% off) | 1 vCPU, 512 MB, 20 GB NVMe, 1 TB | Monthly | 14-day money-back |
| OliveVPS | $3.99/mo | 1 vCPU, 1 GB, 25 GB NVMe, 1 TB | Monthly | DDoS included; Linux-only at this tier |
| FyfeWeb | £9.99/mo | 2 cores @ 4.0 GHz, 4 GB ECC, 48 GB SSD | Monthly | Telehouse North, optional BGP, daily backups |
| LogicWeb | $10/mo | 2 vCPUs, 4 GB, 25 GB NVMe, 2 TB, 2 IPv4 | Monthly, same rate on renewal | Unlimited L3/L4 DDoS scrubbing |
| Vebloom | $14.99/mo | 1 vCPU, 1 GB, 25 GB NVMe, 1 TB | Monthly | Renewal price equals signup price |

**Billing flexibility is the biggest structural difference.** Every rival bills monthly. Vultr bills hourly — the $6 plan works out to roughly 0.8¢ per hour, capped at $6 per month, and even the $2.50 plan is around a third of a cent per hour. A 48-hour load test costs about 40 cents. For CI runners, staging environments, weekend game servers, or a bot you only want live during market hours, that's a genuinely different cost model, and none of the monthly hosts can replicate it without charging you for the weeks you didn't use.

**Bandwidth overflow is where the fine print lives.** Vultr charges $0.01 per extra GB. OliveVPS overages run at $0.005/GB — half the rate — and FyfeWeb includes a 25 TB fair-use allowance before charging £3.99 per additional TB. The included quotas (0.5–10 TB depending on plan) are generous for typical websites, but if you genuinely push multi-terabyte egress every month, run this math before committing anywhere.

**Watch the renewal side, too.** Vebloom and LogicWeb both advertise that renewal matches the signup price. Cloudzy's $2.48 is a 50% discount off a $4.95 list price, so budget for the full rate later. Vultr has no intro/renewal split at all — the rate you deploy at is the rate that persists.

**Windows and DDoS split the field.** OliveVPS bundles Windows Server into its $7.99 Pro and $15.99 Premium plans, while Vultr adds a monthly Windows license fee on top of any plan, so a low-end Windows VPS from Vultr will usually cost more than OliveVPS Pro. On DDoS, OliveVPS and LogicWeb include protection on every plan; Vultr sells always-on mitigation as a $10/month add-on. For a public-facing game server or media origin, that bundled protection can be worth more than a dollar or two of monthly price difference.

## Where a UK rival is genuinely the better choice

Vultr isn't the right answer for every London VPS shopper, and saying so upfront saves everyone time.

- You want DDoS protection included and always on → OliveVPS or LogicWeb.
- You want a cheap Windows box → OliveVPS Pro at $7.99 with Windows included.
- You want maximum hardware at entry level → LogicWeb's $10 v.box two (2 vCPUs, 4 GB, 2 IPv4) or FyfeWeb's £9.99 (2 cores at 4.0 GHz, 4 GB ECC, plus an optional BGP session if you run your own IP space).
- You want a formal refund window → Cloudzy offers 14 days. Vultr doesn't publish a money-back guarantee; its practical equivalent is hourly billing with no commitment, plus the credit promo covered below.

## Deploying your first Vultr London server: what actually happens

Deployment is self-service and takes a couple of minutes once your account is approved. Here's the realistic sequence:

1. **Create the account and add a payment method.** Cards and PayPal both work. One caveat worth knowing: brand-new accounts occasionally get a short manual review on the first payment, so a first deploy can take longer than the usual sub-minute provisioning. Don't schedule a production cutover for the same hour you sign up.
2. **Check the credit offer.** Vultr has been running new-user credit promotions — the signup page has recently shown up to $250 valid for 30 days — and the amount changes, so confirm what's live when you register. 👉 [See the current new-user offer on Vultr's site](https://bit.ly/VulTR).
3. **Deploy.** Choose Cloud Compute, a plan tier, **London** as the region, and your OS image. SSH credentials arrive in under a minute.
4. **Harden it.** Enable the free cloud firewall before exposing anything, switch on automatic backups (+20%) if the data matters, and take a snapshot before major changes.
5. **Mind the meter.** Billing is hourly and stops the instant you destroy the instance. If you're testing, set a calendar reminder so a forgotten 2 GB box doesn't quietly run for six months.

## FAQ

**Does a Vultr London VPS give me a UK IP address?**
Yes. Every instance includes a dedicated IPv4 address that geolocates to the UK, plus a /64 IPv6 subnet. That covers local SEO signals and anything that whitelists your server by IP.

**Is hourly billing really capped at the monthly price?**
Yes. A $6 plan accrues at roughly 0.8¢ per hour and never exceeds $6 in a month, no matter how long it runs.

**Can I move a Vultr server to another region later?**
There's no in-place migration. The practical path is deploying a fresh instance in another region — the same plans are available in more than 30 locations — and syncing your data across; a snapshot makes spinning up the replacement easier.

**How much does Windows Server cost on Vultr?**
Vultr adds a monthly Windows license fee on top of the plan price, and the exact amount appears on the deploy screen before you confirm, so there's no surprise on the invoice.

**Is my data stored in the UK?**
Yes — your instance and its storage physically sit in the London region. One nuance for compliance work: Vultr itself is a US-headquartered company, so UK data residency covers where the data lives, and the jurisdiction requirements that apply to your specific case are worth checking separately.

## Picking between them: a two-minute decision guide

Short-lived or bursty workloads — CI, staging, an occasional VPN endpoint, a bot with limited hours — are exactly what Vultr's hourly billing was built for. Deploy, test, destroy. 👉 [Compare Vultr's London plans and regions](https://www.vultr.com/pricing/?ref=7268283) and start with the smallest tier that fits; you can resize upward from the panel when you outgrow it.

A permanent production site with steady traffic is a different calculation. If bundled DDoS protection or Windows without a license surcharge matters to you, the monthly UK specialists make more sense — OliveVPS and LogicWeb are the standouts there, and FyfeWeb earns its premium if you want ECC memory, 4.0 GHz cores and a BGP session out of Telehouse North.

Two last checks before you pay anyone: confirm the renewal rate (intro discounts don't last forever), and start smaller than your instinct suggests. Overbuying a monthly plan elsewhere costs you a migration to fix; on Vultr, underbuying costs you one click.
