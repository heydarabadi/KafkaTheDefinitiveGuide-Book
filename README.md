# خلاصه و راهنمای جامع کتاب Kafka: The Definitive Guide  
(ویرایش دوم - Real-Time Data and Stream Processing at Scale)

<div dir="rtl">

این پروژه یک **خلاصه‌ی عمیق، فصل‌به‌فصل و کاملاً کاربردی** از کتاب مرجع **Kafka: The Definitive Guide** (ویرایش دوم) به زبان فارسی است.

**نویسندگان کتاب:**  
Gwen Shapira, Todd Palino, Rajini Sivaram, Krit Petty

</div>

## هدف پروژه

- ارائه خلاصه‌های **خوانا**، **دقیق** و **کاربردی** از هر فصل به زبان فارسی  
- توضیح مفاهیم کلیدی همراه با **مثال‌های واقعی** و **نکات عملیاتی** (Production-grade)  
- بررسی عمیق **معماری داخلی** (internals) آپاچی کافکا:  
  replication، log structure، controller، ISR، partition assignment، leader election و ...  
- جمع‌آوری منابع برتر (**Awesome Kafka**): ابزارها، کتاب‌ها، مقاله‌ها، ویدئوها، دوره‌ها و پروژه‌های متن‌باز مرتبط

## چرا این کتاب مهم است؟

این کتاب معتبرترین و جامع‌ترین منبع برای یادگیری **عمیق** آپاچی کافکا محسوب می‌شود.  
از مفاهیم پایه تا موضوعات پیشرفته شامل:

- معماری داخلی و پروتکل replication  
- تضمین‌های قابلیت اطمینان و Exactly-Once Semantics  
- امنیت، مانیتورینگ و عملیات در مقیاس بزرگ  
- Kafka Connect، Kafka Streams و ksqlDB  
- KRaft (جایگزین ZooKeeper)، Tiered Storage و تغییرات جدید نسخه‌های اخیر

## فهرست فصل‌های کتاب (ویرایش دوم)

| فصل | عنوان فصل (انگلیسی)                          | موضوع اصلی خلاصه                                                                 |
|-----|-----------------------------------------------|-----------------------------------------------------------------------------------|
| ۱   | Meet Kafka                                    | مفاهیم پایه: Pub/Sub، Topic، Partition، Broker، Producer/Consumer، Broker Cluster |
| ۲   | Installing Kafka                              | نصب، راه‌اندازی و پیکربندی اولیه                                                |
| ۳   | Kafka Producers: Writing Messages to Kafka    | Producer API، پیکربندی، acknowledgment، compression، batching، partitioning      |
| ۴   | Kafka Consumers: Reading Data from Kafka      | Consumer Group، Offset Management، Rebalance، Commit strategies                  |
| ۵   | Managing Apache Kafka Programmatically        | AdminClient API، مدیریت تاپیک، کانفیگ، Consumer Group و ...                     |
| ۶   | Reliability Guarantees                        | تضمین‌های دوام داده، Durability، Availability، In-Sync Replicas (ISR)          |
| ۷   | Exactly-Once Semantics & Transactions         | تراکنش‌ها، idempotent producer، transactional producer/consumer                 |
| ۸   | Kafka Internals                               | معماری داخلی: Log، Replication Protocol، Controller، Leader Election           |
| ۹   | Operations in Scale                           | Reassignment، MirrorMaker 2، Cluster Expansion، Backup & Restore                |
| ۱۰  | Monitoring Kafka                              | متریک‌ها، JMX، Prometheus + Grafana، ابزارهای مانیتورینگ                       |
| ۱۱  | Security                                      | SSL/TLS، SASL، ACL، Authorization، Authentication                               |
| ۱۲  | Kafka Connect                                 | معماری Connector، Source/Sink، Single Message Transforms (SMT)                 |
| ۱۳  | Kafka Streams & ksqlDB                        | Stream Processing، State Stores، Windowing، Joins، Aggregations، ksqlDB         |

> **فصل‌های پیشرفته‌تر** (بسته به نسخه و آپدیت‌ها): Tiered Storage، KRaft mode (بدون ZooKeeper)، تغییرات جدید API و ...

## ساختار ریپازیتوری

```text
.
├── docs/                  # خلاصه‌های فصل‌به‌فصل (فایل‌های markdown جداگانه)
│   ├── ch01-meet-kafka.md
│   ├── ch02-installing-kafka.md
│   ├── ch03-producers.md
│   ├── ch04-consumers.md
│   └── ...
├── internals/             # بررسی عمیق معماری داخلی کافکا
│   ├── log-structure.md
│   ├── replication-protocol.md
│   ├── controller.md
│   ├── partition-assignment.md
│   └── ...
├── awesome-kafka/         # لیست منابع عالی (Awesome List)
│   └── README.md
├── examples/              # کدهای نمونه (Java, Spring Boot, Kafka Streams, ksqlDB, ...)
├── images/                # دیاگرام‌ها و تصاویر توضیحی
├── CONTRIBUTING.md
└── README.md              # این فایل





# Awesome Kafka

بهترین و به‌روزترین منابع مرتبط با **آپاچی کافکا** (تا سال ۲۰۲۶)

لیست جامع ابزارها، مانیتورینگ، Schema Registry، بلاگ‌ها، دوره‌های آموزشی، ویدئوها و پروژه‌های متن‌باز مرتبط با Kafka

## ابزارهای گرافیکی و مدیریت (GUI Clients / Admin Tools)

- **AKHQ** – رابط کاربری مدرن، سبک و قدرتمند  
- **Kafka UI** – زیبا، واکنش‌گرا و مناسب تیم‌ها  
- **Offset Explorer** (قبلاً Kafka Tool) – ابزار کلاسیک و بسیار کامل  
- **CMAK** (Kafka Manager از Yahoo) – هنوز در بسیاری از سازمان‌ها استفاده می‌شود  
- **Kafdrop** – سبک و ساده  
- **Lenses** – تجاری اما بسیار قدرتمند  
- **Redpanda Console** – مخصوص Redpanda ولی با Kafka هم کار می‌کند  
- **Kpow** – پیشرفته و مناسب محیط‌های بزرگ  

## مانیتورینگ و Observability

- **Prometheus + Grafana + JMX Exporter** – ترکیب استاندارد open-source  
- **Confluent Control Center** – جامع‌ترین راه‌حل تجاری  
- **Burrow** – متخصص در مانیتورینگ Consumer Lag  
- **Kafka Lag Exporter** – برای Prometheus  
- **Cruise Control** – بالانس خودکار پارتیشن‌ها و rebalance هوشمند  
- **Confluent Telemetry** – metrics پیشرفته  

## Schema Registry

- **Confluent Schema Registry** – استاندارد صنعتی  
- **Apicurio Registry** – جایگزین کاملاً open-source و قدرتمند  
- **Karapace** – سبک و سازگار با Confluent Schema Registry  
- **AWS Glue Schema Registry** – اگر در اکوسیستم AWS هستید  

## بلاگ‌ها و نویسندگان برجسته

- [Confluent Blog](https://www.confluent.io/blog/) – مقالات رسمی و به‌روز  
- **Gwen Shapira** – یکی از نویسندگان کتاب Kafka: The Definitive Guide  
- **Kai Waehner** – تحلیل‌های بسیار عمیق در حوزه streaming و آینده کافکا  
- **Jeqo** – نکات عملی و تجربیات واقعی [](https://jeqo.github.io/)  
- **Stéphane Maarek** – آموزش‌های باکیفیت و بلاگ  
- **Robin Moffatt** – مطالب عمیق و کاربردی  
- **Bill Bejeck** – نویسنده کتاب Kafka Streams  
- **Matthias Sax** – از تیم Kafka Streams در Confluent  

## دوره‌های آموزشی و ویدئوها

- **Confluent Developer** – دوره‌های رایگان و پولی بسیار باکیفیت  
- **Kafka: The Definitive Guide** – کتاب + دوره‌های مرتبط (O'Reilly)  
- **Kafka Summit** – ویدئوهای کنفرانس سالانه (YouTube)  

**کانال‌های یوتیوب پیشنهادی:**

- [Confluent](https://www.youtube.com/c/Confluent)  
- [Gwen Shapira](https://www.youtube.com/@gwenshap)  
- [Kai Waehner – Streaming Database](https://www.youtube.com/@kaiwaehner)  
- [Stéphane Maarek](https://www.youtube.com/c/StephaneMaarek)  
- [Tim Berglund (Confluent)](https://www.youtube.com/@timburglund)  

## پروژه‌های متن‌باز جالب ساخته‌شده با/برای کافکا

- **Strimzi** – Kafka Operator برای Kubernetes  
- **kPow** – مدیریت و مشاهده پیشرفته  
- **Kouncil** – رابط کاربری مدرن و سبک  
- **Spring Cloud Stream + Kafka** – پروژه‌های نمونه  
- **Micronaut Kafka** – مثال‌های reactive  
- **Quarkus Kafka** – سریع، کم‌مصرف و native  
- **ksqlDB + Kafka Streams** – دموها و boilerplateهای آماده  
- **WarpStream** – Kafka-compatible بدون ZooKeeper و با object storage  
- **Redpanda** – جایگزین عملکرد بالا و Kafka-compatible
