# Architecture Field Notes

> **"Architecture is the art of deciding which trade-offs you can live with."**

Welcome! This repository is a curated collection of pragmatic architectural patterns and field notes. It focuses on the transition from "building functional systems" to "designing resilient, evolving infrastructures" that survive at scale.

Instead of chasing theoretical perfection, we focus on **physical limits**, **operational resilience**, and the **economic reality** of building massive systems in the wild.

---

## 🏗️ The 30-50-20 Philosophy

I categorize architectural knowledge into three distinct layers based on their role in a system's lifecycle and the intuition required to master them:

* 🧱 **The Foundations (30%):** The invariants. Essential building blocks required for architectural closure and baseline reliability.
* ⚔️ **The Battlegrounds (50%):** Where real engineering happens. This layer focuses on scale, state management, and the messy trade-offs of high-availability systems.
* 🛰️ **The Expert's Edge (20%):** Specialized domains. Niche algorithms and advanced coordination models designed for extreme constraints and performance frontiers.

---

## 🛠️ Patterns Wiki

*A living catalog of architectural patterns and their quantitative trade-offs.*

### 0. The Architect's Ruler (Foundational Intuition)
- [ ] Hardware Latency Numbers Every Architect Should Know 🧱
- [ ] Availability Math (SLO/SLA Calculations) 🧱

### 1. Ingress & Traffic Orchestration
- [ ] Load Balancing (L4/L7 Strategies) 🧱
- [ ] Consistent Hashing 🧱
- [ ] Service Discovery Mechanisms 🧱
- [ ] Health Check & Readiness Probing 🧱
- [ ] API Gateway Pattern 🧱
- [ ] Backend for Frontend (BFF) ⚔️
- [ ] Sidecar Pattern ⚔️
- [ ] Service Mesh Control Planes ⚔️
- [ ] Global Traffic Management (GTM) 🛰️
- [ ] Edge Computing & PoP Nodes 🛰️

### 2. Data Strategy & State Management
- [ ] Database Sharding Strategies 🧱
- [ ] Horizontal vs. Vertical Partitioning 🧱
- [ ] Replication Models (Leader-based / Multi-leader) 🧱
- [ ] Write-Ahead Log (WAL) 🧱
- [ ] LSM-Tree Storage Engines ⚔️
- [ ] B-Tree Storage Engines ⚔️
- [ ] CQRS (Command Query Responsibility Segregation) ⚔️
- [ ] Event Sourcing ⚔️
- [ ] Change Data Capture (CDC) ⚔️
- [ ] Anti-Entropy Mechanisms ⚔️
- [ ] Geo-Replication & Data Sovereignty 🛰️
- [ ] Conflict Resolution (LWW, Custom Resolvers) 🛰️
- [ ] Directory-Based Partitioning 🛰️

### 3. Coordination & Distributed Consistency
- [ ] CAP Theorem 🧱
- [ ] PACELC Framework 🧱
- [ ] Strong vs. Eventual Consistency Models 🧱
- [ ] Distributed Transactions (Saga Pattern) 🧱
- [ ] TCC (Try-Confirm-Cancel) ⚔️
- [ ] Distributed Locking & Fencing Tokens ⚔️
- [ ] Lease Mechanisms ⚔️
- [ ] Leader Election Protocols ⚔️
- [ ] Consensus Algorithms (Raft / Paxos) ⚔️
- [ ] Quorum Systems (N, R, W) 🛰️
- [ ] Logical Clocks (Vector / Lamport) 🛰️
- [ ] CRDTs (Conflict-free Replicated Data Types) 🛰️
- [ ] Merkle Trees for State Sync 🛰️

### 4. Communication & Messaging Backbone
- [ ] Interface Protocols (gRPC vs. REST vs. GraphQL) 🧱
- [ ] Message Queues (Point-to-Point) 🧱
- [ ] Pub/Sub Patterns 🧱
- [ ] Idempotent Processing ⚔️
- [ ] Exactly-once Delivery Semantics ⚔️
- [ ] Backpressure & Flow Control ⚔️
- [ ] Real-time Streams (WebSockets / SSE) ⚔️
- [ ] Claim Check Pattern 🛰️
- [ ] Dead Letter Queues & Retry Policies 🛰️
- [ ] Priority Queuing & Weighted Fair Queuing 🛰️

### 5. Reliability & System Shielding
- [ ] Rate Limiting & Throttling 🧱
- [ ] Timeouts & Deadlines 🧱
- [ ] Retries & Exponential Backoff 🧱
- [ ] Circuit Breaker Pattern ⚔️
- [ ] Bulkhead Isolation ⚔️
- [ ] Load Shedding & Graceful Degradation ⚔️
- [ ] Chaos Engineering & Fault Injection ⚔️
- [ ] Adaptive Concurrency Limits 🛰️
- [ ] Byzantine Fault Tolerance (BFT) 🛰️

### 6. Performance Optimization & Evolution
- [ ] Caching Strategies (Cache-Aside / Write-Through) 🧱
- [ ] Distributed ID Generation (Snowflake, etc.) 🧱
- [ ] Cache Pitfalls (Avalanche / Breakdown / Penetration) ⚔️
- [ ] Bloom Filters ⚔️
- [ ] Cuckoo Filters ⚔️
- [ ] Request Coalescing (Singleflight) ⚔️
- [ ] Double-Write Migration ⚔️
- [ ] Shadow Reads & Dark Launches 🛰️
- [ ] Probabilistic Structures (HyperLogLog / Count-Min Sketch) 🛰️

---

*This knowledge base is curated and edited by me, with architectural framing and drafting assistance from AI.*

---

## 📄 License
This project is licensed under the MIT License.
