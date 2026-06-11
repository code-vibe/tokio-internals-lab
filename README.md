# Tokio Internals Lab

A deep dive into Rust asynchronous programming and Tokio internals.

This repository documents my journey from using Tokio to understanding how asynchronous systems actually work underneath.

The goal is to build increasingly complex systems while gaining a strong understanding of:

- Futures
- Wakers
- Executors
- Cooperative Scheduling
- Pinning
- Async Traits
- Cancellation
- Backpressure
- Channels
- Synchronization
- Resource Management

---

## Learning Objectives

By the end of this repository I should be able to explain:

- How async/await works internally
- How Tokio schedules tasks
- What a Future actually is
- What a Waker does
- Why Pin exists
- How executors poll tasks
- How async cancellation works
- How channels enable communication
- How production async systems are designed

without relying on external references.

---

## Projects

### 01 - TCP Echo Server

Concepts:

- TcpListener
- TcpStream
- tokio::spawn
- Async I/O
- Concurrent connections

---

### 02 - HTTP Server

Concepts:

- TCP protocol
- HTTP parsing
- Request/Response lifecycle
- Connection management

---

### 03 - Concurrent Job Queue

Concepts:

- mpsc channels
- Work distribution
- Backpressure
- Task orchestration

---

### 04 - Background Worker System

Concepts:

- Long running workers
- Graceful shutdown
- Retry patterns
- Message processing

---

### 05 - Rate Limiter

Concepts:

- Time-based coordination
- Shared state
- RwLock
- Token bucket algorithms

---

### 06 - Connection Pool

Concepts:

- Resource management
- Pooling
- Synchronization
- High-throughput design

---


## Documentation

Detailed notes are available in:

/docs

These notes focus on understanding the internals rather than merely using APIs.

---

## Philosophy

Most developers learn:

"How to use Tokio."

This repository focuses on:

"How Tokio works."

The goal is to become capable of reasoning about performance, concurrency, scheduling, and distributed systems at a systems-engineering level.