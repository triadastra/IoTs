# IoT Architecture and Infrastructure

This section covers system design patterns, infrastructure choices, and platform selection for IoT systems.

## Topics Covered

- **[Cloud Platforms](./cloud-platforms.md)** — AWS IoT, Azure IoT, Google Cloud IoT
- **[Network Architecture](./network-architecture.md)** — Design patterns and topologies
- **[Data Management](./data-management.md)** — Storage and analytics

## Architecture Decision Framework

### Key Questions to Answer

1. **Scale** — How many devices? How much data?
   - Millions of lightweight sensors → Edge-first
   - Thousands of complex devices → Cloud-native
   - Hybrid scenarios → Edge + Cloud

2. **Latency Requirements** — How fast must decisions be?
   - Real-time (<10ms) → Edge processing
   - Near-real-time (100ms-1s) → Hybrid
   - Batch acceptable (minutes+) → Cloud analytics

3. **Connectivity** — How often is network available?
   - Always connected → Cloud-first
   - Intermittent → Edge caching + sync
   - Offline critical → Fully local

4. **Data Sensitivity** — Privacy/compliance concerns?
   - Personal data → Local processing
   - Regulated industry → Compliance framework
   - Telemetry data → Cloud acceptable

## Typical Architecture Patterns

### Cloud-Centric (Traditional)
```
[IoT Devices] --MQTT/HTTPS--> [Cloud Platform] <--> [Analytics/Storage]
```
**Best for:** Well-connected devices, high compute needs, scalability

### Edge-First (Modern)
```
[IoT Devices] <--> [Edge Gateway/Hub] <-SYNC-> [Cloud] (Backup/Analytics)
                          ↓
                    Local Processing
```
**Best for:** Latency-sensitive, offline operation, privacy-critical

### Hybrid (Flexible)
```
[Devices] ---> [Local Hub] ---> [Cloud]
                    ↓
             Smart filtering
             (Send only anomalies)
```
**Best for:** Cost optimization, balanced approach

## Platform Selection

### AWS IoT
- **Strengths** — Comprehensive ecosystem, industrial focus
- **Best for** — Enterprise, manufacturing, integration heavy
- **Cost** — Variable, scale-dependent

### Azure IoT
- **Strengths** — Microsoft integration, AI/ML capabilities
- **Best for** — Enterprise Windows shops, digital twins
- **Cost** — Predictable, cloud-inclusive

### Google Cloud IoT
- **Strengths** — Analytics, cost efficiency
- **Best for** — Data-heavy, analytics-first workloads
- **Cost** — Competitive, startup-friendly

### Edge-First Approach
- **Strengths** — No vendor lock-in, full control, offline capable
- **Best for** — Privacy, latency critical, custom needs
- **Cost** — Infrastructure, operational overhead

## Infrastructure Components

### Device Layer
- Sensors and actuators
- Edge gateways/hubs
- Microcontrollers and processors

### Network Layer
- Protocols (MQTT, CoAP, HTTP)
- Connectivity (WiFi, Cellular, LoRaWAN)
- Network management

### Data Layer
- Stream processing
- Storage (time-series, object)
- Caching and synchronization

### Application Layer
- Business logic
- Analytics and ML
- User interfaces

### Security Layer
- (Across all layers)
- Authentication
- Encryption
- Access control
- Monitoring

## Cost Considerations

**Typical breakdown (2026):**
- Device hardware: 30%
- Network connectivity: 20%
- Cloud services: 25%
- Operations/maintenance: 25%

**Cost optimization strategies:**
- Edge processing reduces cloud costs
- Efficient data compression
- Selective archival
- Reserved capacity for predictable workloads

## Scalability Planning

| Metric | Small | Medium | Large |
|--------|-------|--------|-------|
| Devices | 100s | 10,000s | Millions |
| Data volume | GB/day | TB/day | PB/day |
| Latency req | Relaxed | Strict | Critical |
| Architecture | Single cloud | Multi-cloud | Edge + Cloud |

---

**Last Updated:** 2026-03-04
**Starting point:** [Cloud Platforms](./cloud-platforms.md)
