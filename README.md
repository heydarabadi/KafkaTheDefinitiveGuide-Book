# Awesome Kafka

This project is a comprehensive **Awesome Kafka** resource — a deep, chapter-by-chapter, practical summary of the reference book **Kafka: The Definitive Guide** (2nd Edition and updates), combined with in-depth exploration of Kafka internals, code examples, diagrams, production tips, and a curated collection of the best online & offline resources (updated as of 2026).

We are building a complete learning path focused on **understanding Kafka internals** (replication protocol, log structure, controller, ISR, partition assignment, leader election, KRaft mode, Tiered Storage, exactly-once semantics, etc.) using both **online resources** (blogs, videos, GitHub repos, conference talks) and **offline resources** (books, documentation).

### Core Book (Current Focus)
- **Kafka: The Definitive Guide** (2nd Edition + updates)  
  Authors: Gwen Shapira, Todd Palino, Rajini Sivaram, Krit Petty  
  → Still the most authoritative, comprehensive, and production-oriented reference in 2026.

### Project Goals
- Readable, accurate, and practical chapter summaries with real-world context
- Clear explanations of Kafka concepts, internals, and production best practices
- Deep dives into Kafka architecture and internals with references to online/offline sources
- Curated **Awesome Kafka** list: top blogs, authors, courses, videos, open-source tools, books, and more
- Expandable structure: we plan to add summaries and deep-dives for **more Kafka-related books** in the future

---

### Why This Book Matters (Kafka: The Definitive Guide)
It remains the gold standard for deep Kafka knowledge, covering:
- Internal architecture & replication protocol
- Durability, availability, ISR, leader election
- Exactly-Once Semantics & Transactions
- Security, monitoring, large-scale operations
- Kafka Connect, Kafka Streams, ksqlDB
- KRaft mode (ZooKeeper-free), Tiered Storage, and recent Kafka version features
<img width="570" height="740" alt="image" src="https://github.com/user-attachments/assets/2f0423c7-3f88-425e-93f7-10c12720fdf4" />



## Kafka: The Definitive Guide Book Table of Contents (2nd Edition)

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


---


### Planned Book Expansions
We will gradually add summaries and internals deep-dives for other high-quality Kafka/streaming books, including (but not limited to):
- Kafka Streams in Action (Bill Bejeck)
- Kafka Connect in Action (or similar connector-focused books)
- Designing Data-Intensive Applications (relevant Kafka chapters – Martin Kleppmann)
- Streaming Systems (Tyler Akidau et al.)
- Building Event-Driven Microservices (Adam Bellemare)
- And more emerging titles on KRaft, Tiered Storage, and modern streaming patterns



## Repository Structure
```text
├── docs/                          # Chapter-by-chapter summaries (separate markdown files)
│   └── book-kafka-definitive-guide/  # Organized by book name
│       ├── ch01-meet-kafka.md
│       ├── ch02-installing-kafka.md
│       ├── ch03-producers.md
│       ├── ch04-consumers.md
│       └── ...                     # One file per chapter
├── internals/                     # Deep dives into Kafka internals (standalone or cross-book)
│   ├── log-structure.md
│   ├── replication-protocol.md
│   ├── controller.md
│   ├── partition-assignment.md
│   └── ...
├── awesome-kafka/                 # Curated list of excellent Kafka resources
│   └── README.md
├── examples/                      # Sample code (Java, Spring Boot, Kafka Streams, ksqlDB, Python, Quarkus, ...)
├── CONTRIBUTING.md
└── README.md                      # This file
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
## Notable Blogs & Authors

Here are some of the most respected voices and resources in the Kafka ecosystem — regularly publishing high-quality, up-to-date content about Apache Kafka, Kafka Streams, ksqlDB, stream processing architecture, best practices, and future trends.

- **[Confluent Blog](https://www.confluent.io/blog/)**  
  The official blog from Confluent — the company founded by Kafka’s creators. Contains the most authoritative and timely articles, release announcements, deep dives, and production stories.

- **[Gwen Shapira](https://www.gwenshapira.com/)**  
  Co-author of *Kafka: The Definitive Guide* and former Kafka PMC member. Writes about Kafka internals, architecture decisions, and real-world scaling lessons.

- **[Kai Waehner](https://www.kai-waehner.de/blog/)**  
  One of the deepest analysts in the streaming world. Covers Kafka ecosystem trends, comparisons (Kafka vs. Pulsar, Redpanda, etc.), future directions, and vendor-neutral architecture advice.

- **[Jeqo (João Boto)](https://jeqo.github.io/)**  
  Very practical, hands-on posts with real production experience — great for operators and SREs who want battle-tested configurations and troubleshooting guides.

- **[Stéphane Maarek](https://www.stephanemaarek.com/blog)**  
  Creator of the most popular Kafka courses on Udemy. Shares high-quality educational content, exam tips (Confluent Certified Developer for Apache Kafka), and clear explanations.

- **[Robin Moffatt](https://rmoff.net/)**  
  Deep, practical, and often humorous insights. Excellent posts about Kafka Connect, ksqlDB, monitoring, performance tuning, and real use cases.

- **[Bill Bejeck](https://billbejeck.com/)**  
  Author of *Kafka Streams in Action*. Writes detailed, code-heavy articles about stream processing patterns, state stores, exactly-once semantics, and Kafka Streams internals.

- **[Matthias J. Sax](https://www.mj-sax.de/)**  
  Kafka Streams tech lead at Confluent. Publishes very technical deep-dives into Kafka Streams, exactly-once guarantees, windowing, and upcoming features.

## Courses & Learning Resources

- **[Confluent Developer](https://developer.confluent.io/)**  
  Official free and paid learning platform — interactive courses, hands-on labs, certification paths (Developer, Operator), and Kafka 101 to advanced streaming topics.

- **[Kafka: The Definitive Guide – Related O'Reilly Courses & Videos](https://www.oreilly.com/library/view/kafka-the-definitive/9781492043072/)**  
  The book itself has companion video courses and live training on O'Reilly (Safari). Search for “Kafka: The Definitive Guide” on learning.oreilly.com.

- **[Kafka Summit Talks (YouTube)](https://www.youtube.com/c/KafkaSummit)**  
  Annual Kafka Summit conference videos — free on YouTube. Covers real customer stories, deep technical sessions, new features, and community talks from 2016–present.

**Recommended YouTube Channels:**

- [Confluent](https://www.youtube.com/c/Confluent)
- [Gwen Shapira](https://www.youtube.com/@gwenshap)
- [Kai Waehner – Streaming Database](https://www.youtube.com/@kaiwaehner)
- [Stéphane Maarek](https://www.youtube.com/c/StephaneMaarek)
- [Tim Berglund (Confluent)](https://www.youtube.com/@timburglund)

## Interesting Open-Source Projects Built Around / For Kafka

Here are some of the most notable and actively maintained open-source projects that extend, manage, observe, or provide alternatives/companions to **Apache Kafka**. These tools are widely used in production (as of 2026) for Kubernetes deployments, observability, UI management, developer frameworks, and high-performance alternatives.

- **[Strimzi](https://github.com/strimzi/strimzi-kafka-operator)**  
  The leading **Kafka Operator for Kubernetes** / OpenShift. It makes deploying, scaling, upgrading, and managing Kafka clusters declarative and GitOps-friendly. Supports KRaft mode, MirrorMaker 2, Kafka Connect, and advanced security features. Maintained by the Strimzi community (Red Hat involvement).

- **[kPow](https://github.com/factorhouse/kpow)** (by Factor House)  
  Enterprise-grade **management, observability, and control UI/API** for Kafka. Offers deep visibility into clusters, consumer groups, offsets, schema registry, Connect, Streams apps, and more — with OpenAPI support for automation. Vendor-agnostic and works with any Kafka distribution.

- **[Kouncil](https://github.com/Consdata/kouncil)**  
  Modern, lightweight, and feature-rich **web dashboard/UI** for Kafka. Allows browsing topics, managing consumer groups, producing/consuming messages, viewing metrics, and diagnosing issues. User-friendly and actively updated.

- **[Spring Cloud Stream + Kafka](https://github.com/spring-cloud/spring-cloud-stream-binder-kafka)** (Spring projects)  
  Official Spring integration for Kafka. Provides many sample projects, starters, and examples for building event-driven microservices with Kafka (e.g., processors, sinks, sources). Great for Java/Spring Boot developers.

- **[Micronaut Kafka](https://github.com/micronaut-projects/micronaut-kafka)**  
  Reactive Kafka client and integration for **Micronaut** (fast, lightweight JVM framework). Includes examples for producers/consumers, Streams, and low-latency reactive apps.

- **[Quarkus Kafka](https://github.com/quarkusio/quarkus/tree/main/extensions/smallrye-reactive-messaging-kafka)** (Quarkus extensions)  
  Super-fast, low-memory, native-compiled Kafka support in Quarkus. Includes reactive messaging, Kafka Streams, and native executables. Ideal for cloud-native and serverless Java apps.

- **[ksqlDB + Kafka Streams](https://github.com/confluentinc/ksql)** (Confluent open-source) + community demos  
  ksqlDB: SQL engine for stream processing on Kafka. Kafka Streams: powerful Java library for stateful/real-time processing. Look for official demos, boilerplates, and community repos (e.g., Confluent examples, Bill Bejeck’s samples) for patterns like joins, windowing, and exactly-once.

- **[WarpStream](https://github.com/warpstreamlabs/warpstream)** (core agent/protocol impl parts open, but primarily commercial)  
  Kafka-compatible streaming platform with **zero-disk, S3-native backend** (no ZooKeeper/KRaft needed). Focuses on infinite elasticity, low cost, and no inter-AZ traffic fees. Agent is open-source; full platform has proprietary elements.

- **[Redpanda](https://github.com/redpanda-data/redpanda)**  
  High-performance, Kafka-compatible alternative written in C++. No ZooKeeper/KRaft (uses internal Raft), single-binary simplicity, lower latency/footprint in many benchmarks. Includes **Redpanda Console** UI (open-source Kafka UI). Often used as a drop-in replacement.

### Bonus Mentions (Frequently Recommended in 2026)

- **Kafka UI / AKHQ / CMAK** — Popular free GUIs (e.g., [provectus/kafka-ui](https://github.com/provectus/kafka-ui), [tchiotludo/akhq](https://github.com/tchiotludo/akhq), Yahoo CMAK)
- **Burrow** — Consumer lag monitoring (LinkedIn original)
- **Cruise Control** — Automated rebalancing and optimization (LinkedIn)

These projects are excellent starting points for extending Kafka in Kubernetes, observability, developer productivity, or exploring high-performance alternatives. Most have active communities, Helm charts, Docker images, and documentation.
## Contributing

We welcome contributions!  

## License

MIT License – feel free to use, modify, and share.

**Last updated:** February 2026
