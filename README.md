# 🏗️ Architecture Field Notes

> **"Architecture is the art of deciding which trade-offs you can live with."**

Welcome! This repository is a **comprehensive glossary** of architectural patterns. It serves as the foundational reference for [**my Substack**](https://qianarthurwang.substack.com/), where I discuss high-level strategy and real-world implementation. This repository is where you go if you need a quick, simple explanation of a specific pattern or term.

---

## 🏗️ The 30-50-20 Philosophy

I categorize architectural knowledge into three distinct layers based on their role in a system's lifecycle and the intuition required to master them:

* 🧱 **The Foundations (30%):** The invariants. Essential building blocks required for architectural closure and baseline reliability.
* ⚔️ **The Battlegrounds (50%):** Where real engineering happens. This layer focuses on scale, state management, and the messy trade-offs of high-availability systems.
* 🛰️ **The Expert's Edge (20%):** Specialized domains. Niche algorithms and advanced coordination models designed for extreme constraints and performance frontiers.

---

## 🛠️ Patterns Wiki (Index)

### 0. The Architect's Ruler (The "Sense" of Scale)
- [ ] [Hardware Latency Numbers](./patterns/latency-numbers.md) 🧱
- [x] [Availability Math](./patterns/availability-math.md) 🧱

### 1. Ingress & Traffic Orchestration (How users reach us)
- [ ] [Load Balancing (L4/L7)](./patterns/load-balancing.md) 🧱
- [ ] [Consistent Hashing](./patterns/consistent-hashing.md) 🧱
- [ ] [Service Discovery](./patterns/service-discovery.md) 🧱
- [ ] [Health Checks & Probing](./patterns/health-checks.md) 🧱
- [ ] [API Gateway](./patterns/api-gateway.md) 🧱
- [ ] [Backend for Frontend (BFF)](./patterns/bff.md) ⚔️
- [ ] [Sidecar Pattern](./patterns/sidecar.md) ⚔️
- [ ] [Service Mesh](./patterns/service-mesh.md) ⚔️
- [ ] [Global Traffic Management (GTM)](./patterns/gtm.md) 🛰️
- [ ] [Edge Computing](./patterns/edge-computing.md) 🛰️

### 2. Data Strategy & State (How we handle information)
- [ ] [Database Sharding](./patterns/db-sharding.md) 🧱
- [ ] [Partitioning (Horizontal/Vertical)](./patterns/partitioning.md) 🧱
- [ ] [Replication Models](./patterns/replication-models.md) 🧱
- [ ] [Write-Ahead Log (WAL)](./patterns/wal.md) 🧱
- [ ] [LSM-Tree vs B-Tree Engines](./patterns/storage-engines.md) ⚔️
- [ ] [CQRS](./patterns/cqrs.md) ⚔️
- [ ] [Event Sourcing](./patterns/event-sourcing.md) ⚔️
- [ ] [Change Data Capture (CDC)](./patterns/cdc.md) ⚔️
- [ ] [Anti-Entropy Mechanisms](./patterns/anti-entropy.md) ⚔️
- [ ] [Geo-Replication](./patterns/geo-replication.md) 🛰️
- [ ] [Conflict Resolution (LWW, etc.)](./patterns/conflict-resolution.md) 🛰️

### 3. Coordination & Consistency (How servers agree)
- [x] [CAP & PACELC](./patterns/cap-pacelc.md) 🧱
- [x] [Consistency Models](./patterns/consistency-models.md) 🧱
- [ ] [Saga Pattern](./patterns/saga.md) 🧱
- [ ] [TCC (Try-Confirm-Cancel)](./patterns/tcc.md) ⚔️
- [ ] [Distributed Locking](./patterns/distributed-locking.md) ⚔️
- [ ] [Leader Election](./patterns/leader-election.md) ⚔️
- [ ] [Consensus (Raft/Paxos)](./patterns/consensus.md) 🛰️
- [ ] [Logical Clocks](./patterns/logical-clocks.md) 🛰️
- [ ] [CRDTs](./patterns/crdts.md) 🛰️

### 4. Communication & Messaging (How services talk)
- [ ] [Protocols (gRPC/REST/GraphQL)](./patterns/protocols.md) 🧱
- [ ] [Message Queues & Pub/Sub](./patterns/messaging-basics.md) 🧱
- [ ] [Idempotency](./patterns/idempotency.md) ⚔️
- [ ] [Exactly-once Semantics](./patterns/exactly-once.md) ⚔️
- [ ] [Backpressure & Flow Control](./patterns/backpressure.md) ⚔️
- [ ] [Dead Letter Queues & Retries](./patterns/dlq-retries.md) 🛰️
- [ ] [Priority Queuing](./patterns/priority-queues.md) 🛰️

### 5. Reliability & Shielding (How we stay alive)
- [ ] [Rate Limiting & Throttling](./patterns/rate-limiting.md) 🧱
- [x] [Timeouts & Deadlines](./patterns/timeouts.md) 🧱
- [x] [Redundancy](./patterns/redundancy.md) 🧱
- [ ] [Retries & Exponential Backoff](./patterns/backoff.md) 🧱
- [ ] [Circuit Breaker](./patterns/circuit-breaker.md) ⚔️
- [ ] [Bulkhead Isolation](./patterns/bulkhead.md) ⚔️
- [ ] [Load Shedding](./patterns/load-shedding.md) ⚔️
- [ ] [Adaptive Concurrency Limits](./patterns/adaptive-concurrency.md) 🛰️
- [ ] [Byzantine Fault Tolerance (BFT)](./patterns/bft.md) 🛰️

### 6. Performance & Evolution (How we get faster)
- [ ] [Caching Strategies](./patterns/caching.md) 🧱
- [ ] [Distributed ID Generation](./patterns/id-generation.md) 🧱
- [ ] [Cache Pitfalls](./patterns/cache-pitfalls.md) ⚔️
- [ ] [Bloom & Cuckoo Filters](./patterns/probabilistic-filters.md) ⚔️
- [ ] [Request Coalescing (Singleflight)](./patterns/singleflight.md) ⚔️
- [ ] [Double-Write Migration](./patterns/double-write.md) ⚔️
- [ ] [Shadow Reads](./patterns/shadow-reads.md) 🛰️
- [ ] [Probabilistic Structures (HLL)](./patterns/hll.md) 🛰️

### 7. Observability & Insight (How we see what's happening)
- [ ] [Metrics, Logs, and Traces (The Three Observability Pillars)](./patterns/observability-pillars.md) 🧱
- [ ] [Distributed Tracing & Context Propagation](./patterns/distributed-tracing.md) ⚔️
- [ ] [Structured Logging](./patterns/structured-logging.md) 🧱
- [ ] [Synthetic Monitoring vs. Real User Monitoring (RUM)](./patterns/monitoring-types.md) ⚔️
- [ ] [Sampling Strategies](./patterns/tracing-sampling.md) 🛰️

### 8. Deployment & Evolution (How we change the ship while sailing)
- [ ] [Blue-Green Deployment](./patterns/blue-green.md) 🧱
- [ ] [Canary Releases](./patterns/canary.md) ⚔️
- [ ] [Feature Flags / Toggles](./patterns/feature-flags.md) ⚔️
- [ ] [Strangler Fig Pattern (Legacy Migration)](./patterns/strangler-pattern.md) ⚔️
- [ ] [Database Schema Evolution (Expand/Contract)](./patterns/db-migration.md) 🛰️

### 9. Structural Styles (The Big Picture)
- [ ] [Monolith vs. Microservices](./patterns/monolith-microservices.md) 🧱
- [ ] [Serverless & FaaS](./patterns/serverless.md) ⚔️
- [ ] [Cell-based Architecture](./patterns/cell-based-architecture.md) 🛰️
- [ ] [Control Plane vs. Data Plane Separation](./patterns/cp-dp-separation.md) 🛰️

---

## 🔗 Bridge to the blogs
*For the high-level strategy and production stories, visit:*
👉 [**my Substack**](https://qianarthurwang.substack.com/)

---

## 📄 License
MIT License. Content curated by me, with framing assistance from AI.


