# Architecture Field Notes

> **"Architecture is the art of deciding which trade-offs you can live with."**

Welcome! This repository is a curated collection of pragmatic architectural patterns and field notes. It focuses on the transition from "building functional systems" to "designing resilient, evolving infrastructures" that survive at scale.

Instead of chasing theoretical perfection, we focus on **physical limits**, **operational resilience**, and the **economic reality** of building massive systems in the wild.

---

## 🏗️ The 30-50-20 Philosophy

I categorize architectural knowledge into three distinct layers based on their role in a system's lifecycle:

- **⭐ The Foundations (30%):** Essential building blocks. Invariant patterns required for architectural closure and baseline reliability.
- **🔥 The Battlegrounds (50%):** Where the real complexity lies. Focuses on decoupling, high availability, and managing state at scale.
- **📘 The Expert's Edge (20%):** Specialized domains. Niche algorithms and advanced coordination models for extreme constraints.

---

## 🛠️ Pattern Wiki (The 49+ Patterns)

*A living catalog of architectural patterns. Detailed deep dives for each can be found in the `/patterns` directory.*

### 1. Traffic & Ingress Control
- [ ] Load Balancing (L4 vs L7) ⭐
- [ ] Service Discovery ⭐
- [ ] API Gateway Pattern ⭐
- [ ] BFF (Backend for Frontend) 🔥
- [ ] Sidecar Pattern 🔥
- [ ] Service Mesh 🔥
- [ ] Edge Computing / PoP Nodes 📘

### 2. Data & State Management
- [ ] Database Sharding ⭐
- [ ] Database Replication (Master-Slave / Multi-Master) ⭐
- [ ] Geo-Sharding & Replication 📘
- [ ] Directory-Based Partitioning 📘
- [ ] LSM-Tree (Write-heavy optimization) 🔥
- [ ] B+ Tree (Read-heavy optimization) 🔥
- [ ] CQRS (Command Query Responsibility Segregation) 🔥
- [ ] Event Sourcing 🔥

### 3. Coordination & Consistency
- [ ] CAP Theorem / PACELC ⭐
- [ ] Consistent Hashing ⭐
- [ ] Strong vs. Eventual Consistency ⭐
- [ ] Distributed Transactions (Saga Pattern) ⭐
- [ ] Distributed Locking (Redis / Zookeeper) 🔥
- [ ] Leader Election (Raft / Paxos) 🔥
- [ ] 2PC / 3PC 📘
- [ ] Quorums (N, R, W) 📘
- [ ] Logical Clocks (Vector Clocks / Lamport) 📘
- [ ] CRDTs (Conflict-free Replicated Data Types) 📘
- [ ] Merkle Trees 📘

### 4. Communication & Messaging
- [ ] Protocols: RPC vs. REST vs. GraphQL ⭐
- [ ] Message Queues (Kafka / RabbitMQ) ⭐
- [ ] Pub/Sub Pattern ⭐
- [ ] Backpressure 🔥
- [ ] Real-time: Polling, WebSockets, SSE 🔥
- [ ] Claim Check Pattern 📘
- [ ] Priority Queue Pattern 📘

### 5. Reliability & Resilience
- [ ] Rate Limiting ⭐
- [ ] Idempotency ⭐
- [ ] Timeouts ⭐
- [ ] Load Shedding / Throttling 🔥
- [ ] Circuit Breaker 🔥
- [ ] Bulkhead Pattern 🔥
- [ ] Retry with Backoff & Jitter 🔥
- [ ] Graceful Degradation 🔥

### 6. Performance & Evolution
- [ ] Caching Strategies (Cache-Aside, Write-Through) ⭐
- [ ] Distributed ID (Snowflake, etc.) ⭐
- [ ] Cache Pitfalls (Avalanche, Breakdown, Penetration) 🔥
- [ ] Bloom Filter 🔥
- [ ] Request Coalescing (Singleflight) 🔥
- [ ] Count-Min Sketch 📘
- [ ] Double-Write Migration & Observability 🔥

---

*This knowledge base is curated and edited by me, with architectural framing and drafting assistance from AI.*

---

## 📄 License
This project is licensed under the MIT License.
