# Kybalion Database 👁️
**The Ultimate Embedded, Encrypted, MVCC Database for Pure ALU**

Kybalion is an enterprise-grade database engine built completely from scratch in Pure ALU. Designed to solve the concurrency limitations of SQLite, Kybalion offers heavy multi-user workloads, blistering fast B-Tree indexing, and military-grade encryption at rest.

## Features
- **Multi-Version Concurrency Control (MVCC):** Readers never block writers. Designed for heavy multi-user workloads, scaling flawlessly where single-writer embedded databases fail.
- **B-Tree Indexing:** Ultra-fast `O(log n)` searching across millions of records.
- **Encryption at Rest:** Seamless integration with `std::crypto.alu` to encrypt all data pages with AES-256 before they touch the disk.
- **Strict Data Typing:** Mathematical schema enforcement powered by the ALU Z3 verifier.
- **Enterprise-Grade Security:** Used by the Aegis Antivirus Ring-0 Kernel Driver to safely store critical telemetry.
- **Log Compaction:** Built-in fragmentation management and log rotation.

## Installation
Currently tightly coupled with the ALU 1.0 ecosystem. Import via:
```alu
import kybalion::db
```
