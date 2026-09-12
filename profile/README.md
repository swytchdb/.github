# Swytch

**Infrastructure for distributed systems without the usual coordination bottlenecks.**

Swytch BV builds distributed databases, embedded infrastructure, and the tools around them.

## SwytchDB

[SwytchDB](https://github.com/swytchdb/swytch) is a Redis-compatible cache and database that is leaderless and infinitely scalable.

Existing Redis clients can connect directly. Underneath, Swytch is built for distribution 
from the ground up — allowing data and workloads to spread across machines and regions without introducing a central leader.

→ **[swytchdb/swytch](https://github.com/swytchdb/swytch)**

## Embedded Engine

[Swytch Engine](https://github.com/swytchdb/engine) is the distributed systems engine underneath SwytchDB.

It's available separately for applications that need to embed Swytch directly rather than run a standalone database server.

→ **[swytchdb/engine](https://github.com/swytchdb/engine)**

## Integrations

### Caddy Storage

[caddy-storage](https://github.com/swytchdb/caddy-storage) uses Swytch as Caddy's distributed certificate store.

Multiple Caddy instances can share certificate state without requiring a separate database or external coordination service.

→ **[swytchdb/caddy-storage](https://github.com/swytchdb/caddy-storage)**

### Caddy Server

[caddy-server](https://github.com/swytchdb/caddy-server) embeds Swytch directly into Caddy and exposes its Redis-compatible cache from the Caddy process itself.

Caddy becomes both the application edge and the distributed cache — without another service to deploy.

→ **[swytchdb/caddy-server](https://github.com/swytchdb/caddy-server)**

## What else are we working on?

Sometimes solving one distributed-systems problem opens a door somewhere completely unexpected.

Research originally developed for Swytch's leaderless distributed indexing led us into a very 
different problem: whether an AI model could learn while performing its forward pass.

That became **Kestrel**, our ongoing research into forward-pass learning, persistent model memory, and distributed learning.

It's early R&D, not another database product — but it came from the same work.

→ **[What does distributed systems have to do with AI?](https://withinboredom.info/posts/dist/)**

## Open source

Most of what we build starts in the open. Browse the repositories here, or learn more at **[getswytch.com](https://getswytch.com)**.

---

**Swytch BV** · Netherlands
