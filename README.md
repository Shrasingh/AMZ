# amazon-engineering-observations

Five things I noticed while using Amazon that feel like real engineering problems hiding in plain sight.

I don’t work at Amazon.

I’m a backend engineer who spends a lot of time building transactional systems—APIs, retries, idempotency, database consistency—and like most people, I shop on Amazon.

This repository is my attempt to study Amazon like an engineer, not just a customer.

Every observation is:

- backed by public evidence (Reddit, Hacker News, Seller Central, FTC, App Reviews)
- framed as an engineering hypothesis, not an accusation
- followed by realistic fixes (APIs, DB design, caching, rollout, metrics)

---

## What triggered this repo

I ordered a Treo lunch box because Amazon promised 2-day delivery.

A few minutes after payment, the ETA changed to 8+ days.

That simple experience made me curious:

How does a company at Amazon’s scale make delivery promises before inventory and fulfillment are fully locked?

That question turned into this repo.

---

## The 5 observations

| # | Issue | Read time |
|---|-------|-----------|
| 01 | Checkout — duplicate orders under retry conditions | ~4 min |
| 02 | Delivery promise changes after payment | ~3 min |
| 03 | Search relevance — sponsored vs organic ranking | ~3 min |
| 04 | Cart consistency across devices | ~3 min |
| 05 | Review integrity — variation merging and trust issues | ~3 min |

---

## Why I built this

Most product complaints online stop at frustration.

I wanted to go one layer deeper:

What would the likely backend failure look like?
How would I reproduce it?
How would I fix it in production?

If an Amazon engineer reads this and disagrees, I’d rather be corrected than stay confident for the wrong reasons.