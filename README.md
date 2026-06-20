# 100 System Design Architecture Drills

A curated set of 100 short system design problems. Each one is a prompt to design the **end-to-end architecture** for a real system at scale.

Given a system and its scale numbers: sketch the components, the data stores, the queues, the read and write paths, and the trade-offs. Then go a level deeper — where does it break first, and how would you evolve it as load grows?

## Format

Every file (`Q01.md` … `Q100.md`) is structured the same way:

```markdown
# Q{N}. {Problem Title}

{1–2 line problem statement with realistic scale numbers.}
```

That's it. The scale numbers are the constraint — let them drive the design.

## How to use

1. Pick a problem (random or in order).
2. Time-box yourself to 15–30 minutes.
3. Work through the architecture:
   - **High-level design** — components, data stores, queues, the critical read/write/dispatch path.
   - **Scale the numbers** — math out the QPS, storage, latency, concurrency. Let the math force the design decisions.
   - **Bottlenecks** — name the component that saturates first, the failure mode, and the fix.
   - **Evolve it** — what breaks at 10× the load, and what you'd change.

Don't reach for Redis / sharding / a CDN by reflex. Start simple, and let the scale numbers justify each upgrade.

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

## How to get the most out of these

Design the whole architecture, but don't stop at the happy-path diagram. The signal is in the depth: which component saturates first, why that failure mode happens, and the cheapest change that gets you past it. A design that names its own bottlenecks and shows how it evolves under 10× load demonstrates far more than a static box-and-arrow diagram.

## License

MIT. Use for interview prep, training, blog posts, whatever — credit appreciated but not required.
