# 100 System Design Bottleneck Drills

A curated set of 100 short system design problems. Each one asks a single, focused question:

> **What's the bottleneck?**

No multi-page architecture diagrams. No "design Twitter end-to-end." Just: given a system at this scale, where does it choke first, why, and what's the cheapest mitigation.

## Format

Every file (`Q01.md` … `Q100.md`) is structured the same way:

```markdown
# Q{N}. {Problem Title}

{1–2 line problem statement with realistic scale numbers.}
```

That's it. For each one, ask yourself: **what's the bottleneck?**

## How to use

1. Pick a question (random or in order).
2. Time-box yourself to 5–10 minutes.
3. Write three things:
   - **Where does this break first?** (which component saturates)
   - **Why?** (math the QPS / storage / latency / concurrency)
   - **The minimum-cost mitigation.** (the cheapest change that gets you past it)

If your instinct is "shard the database," stop and ask whether the database is actually the bottleneck. Most of the time it isn't.

## Topics covered

- URL shorteners, paste services, key-value stores
- Photo / video sharing, recommendation engines, feeds
- Ride-hailing, food delivery, last-mile tracking
- Geospatial search, geofencing, maps routing
- Ticketing, flash sales, inventory reservation
- Chat, presence, typing indicators, read receipts
- Search, autocomplete, leaderboards
- Payments, wallets, fraud detection, KYC
- Ad bidding, real-time analytics, recommendation
- Notifications, email, SMS, push, webhooks
- Multi-region replication, disaster recovery, backup
- Insurance claims, document collaboration, code hosting

## Why "bottleneck" not "architecture"

Most system design practice rewards drawing impressive diagrams. Real production work rewards correctly identifying the **one thing that's about to fall over** and the cheapest fix.

A 10-minute "where does it break" answer demonstrates more practical engineering than a 60-minute "here's the entire architecture" answer.

## License

MIT. Use for interview prep, training, blog posts, whatever — credit appreciated but not required.
