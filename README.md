# Awesome Kafka

This project provides a deep, chapter-by-chapter, practical summary of the reference book **Kafka: The Definitive Guide (2nd Edition)** , along with internals deep-dives, code examples, diagrams, and a curated list of the best up-to-date Kafka resources (as of 2026).

**Authors of the book:**  
Gwen Shapira, Todd Palino, Rajini Sivaram, Krit Petty

## Project Goals

- Readable, accurate, and practical chapter summaries in Persian (Farsi)
- Clear explanations of key concepts with real-world examples and production-grade tips
- In-depth exploration of Apache Kafka internals: replication, log structure, controller, ISR, partition assignment, leader election, ...
- Collection of top-tier resources (**Awesome Kafka**): tools, blogs, videos, courses, open-source projects

## Why This Book Matters

**Kafka: The Definitive Guide** is widely regarded as the most authoritative and comprehensive resource for deep Apache Kafka knowledge.  
It covers everything from fundamentals to advanced production topics:

- Internal architecture and replication protocol
- Durability, availability, and Exactly-Once Semantics guarantees
- Security, monitoring, and large-scale operations
- Kafka Connect, Kafka Streams, and ksqlDB
- KRaft mode (ZooKeeper-free), Tiered Storage, and recent version changes

## Book Table of Contents (2nd Edition)

| Chapter | English Title                                      | Main Topics Covered                                                                 |
|--------|----------------------------------------------------|-------------------------------------------------------------------------------------|
| 1      | Meet Kafka                                         | Pub/Sub basics, Topic, Partition, Broker, Producer/Consumer, Broker Cluster        |
| 2      | Installing Kafka                                   | Installation, initial setup and configuration                                       |
| 3      | Kafka Producers: Writing Messages to Kafka         | Producer API, configuration, acks, compression, batching, partitioning             |
| 4      | Kafka Consumers: Reading Data from Kafka           | Consumer Groups, Offset Management, Rebalance, Commit strategies                   |
| 5      | Managing Apache Kafka Programmatically             | AdminClient API, topic & config management, consumer groups, cluster metadata      |
| 6      | Reliability Guarantees                             | Data durability, availability, In-Sync Replicas (ISR)                              |
| 7      | Exactly-Once Semantics & Transactions              | Transactions, idempotent & transactional producers/consumers                       |
| 8      | Kafka Internals                                    | Log structure, replication protocol, controller, leader election                   |
| 9      | Operations at Scale                                | Partition reassignment, MirrorMaker 2, cluster expansion, backup & restore         |
| 10     | Monitoring Kafka                                   | Metrics, JMX, Prometheus + Grafana, monitoring tools                               |
| 11     | Security                                           | SSL/TLS, SASL, ACLs, authentication & authorization                                |
| 12     | Kafka Connect                                      | Connector architecture, Source/Sink, Single Message Transforms (SMT)               |
| 13     | Kafka Streams & ksqlDB                             | Stream processing, state stores, windowing, joins, aggregations, ksqlDB            |

**Advanced / newer topics** (depending on updates): Tiered Storage, KRaft mode (ZooKeeper removal), recent API changes, ...

## Repository Structure
```text
├── docs/                  # Chapter-by-chapter summaries (separate markdown files)
│   ├── ch01-meet-kafka.md
│   ├── ch02-installing-kafka.md
│   ├── ch03-producers.md
│   ├── ch04-consumers.md
│   └── ...
├── internals/             # Deep dives into Kafka internals
│   ├── log-structure.md
│   ├── replication-protocol.md
│   ├── controller.md
│   ├── partition-assignment.md
│   └── ...
├── awesome-kafka/         # Curated list of excellent Kafka resources
│   └── README.md
├── examples/              # Sample code (Java, Spring Boot, Kafka Streams, ksqlDB, Python, Quarkus, ...)
├── images/                # Explanatory diagrams and images
├── CONTRIBUTING.md
└── README.md              # This file
```



## Awesome Kafka

**Best and most up-to-date Kafka resources (as of 2026)**  
Curated list of tools, monitoring solutions, Schema Registries, blogs, courses, videos, and interesting open-source projects.

### GUI Clients / Admin Tools

- **AKHQ** – Modern, lightweight, powerful UI
- **Kafka UI** – Beautiful, responsive, team-friendly
- **Offset Explorer** (formerly Kafka Tool) – Classic, very feature-complete
- **CMAK** (Yahoo Kafka Manager) – Still widely used in many organizations
- **Kafdrop** – Lightweight and simple
- **Lenses** – Commercial but very powerful
- **Redpanda Console** – Great for Redpanda, works with Kafka too
- **Kpow** – Advanced, suitable for large environments

### Monitoring & Observability

- **Prometheus + Grafana + JMX Exporter** – Most popular open-source stack
- **Confluent Control Center** – Most comprehensive commercial solution
- **Burrow** – Specialized consumer lag monitoring
- **Kafka Lag Exporter** – Prometheus-ready lag metrics
- **Cruise Control** – Automatic partition balancing & smart rebalancing
- **Confluent Telemetry** – Advanced metrics collection

### Schema Registry

- **Confluent Schema Registry** – Industry standard
- **Apicurio Registry** – Fully open-source, powerful alternative
- **Karapace** – Lightweight, Confluent-compatible
- **AWS Glue Schema Registry** – Good choice in AWS ecosystems

### Notable Blogs & Authors

- [Confluent Blog](https://www.confluent.io/blog/) – Official, up-to-date articles
- **Gwen Shapira** – Co-author of Kafka: The Definitive Guide
- **Kai Waehner** – Deep streaming & future-of-Kafka analysis
- **Jeqo** – Practical tips & real-world experience
- **Stéphane Maarek** – High-quality educational content
- **Robin Moffatt** – Deep & practical insights
- **Bill Bejeck** – Kafka Streams book author
- **Matthias Sax** – Kafka Streams team @ Confluent

### Courses & Videos

- **Confluent Developer** – Excellent free & paid courses
- **Kafka: The Definitive Guide** – Book + related O'Reilly courses
- **Kafka Summit** – Annual conference talks (YouTube)

**Recommended YouTube Channels:**

- [Confluent](https://www.youtube.com/c/Confluent)
- [Gwen Shapira](https://www.youtube.com/@gwenshap)
- [Kai Waehner – Streaming Database](https://www.youtube.com/@kaiwaehner)
- [Stéphane Maarek](https://www.youtube.com/c/StephaneMaarek)
- [Tim Berglund (Confluent)](https://www.youtube.com/@timburglund)

### Interesting Open-Source Projects Built Around / For Kafka

- **Strimzi** – Kafka Operator for Kubernetes
- **kPow** – Advanced management & observability
- **Kouncil** – Modern, lightweight UI
- **Spring Cloud Stream + Kafka** – Sample projects
- **Micronaut Kafka** – Reactive examples
- **Quarkus Kafka** – Fast, low-memory, native
- **ksqlDB + Kafka Streams** – Demos & boilerplates
- **WarpStream** – Kafka-compatible, ZooKeeper-free, object-storage backend
- **Redpanda** – High-performance Kafka-compatible alternative

## Contributing

We welcome contributions!  
See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

MIT License – feel free to use, modify, and share.

**Last updated:** February 2026
