# IoT Network Architecture

## Overview

IoT network architecture describes how data flows from physical sensors to
applications and back to actuators. A useful mental model is a layered stack — from
the constrained device edge, through gateways and connectivity, to cloud platforms.
Good architecture balances latency, bandwidth, power, cost, reliability, and security
for a specific workload.

## The Layered Model

A common reference decomposition:

```
┌─────────────────────────────────────────┐
│ Application Layer   (apps, dashboards,   │
│                      analytics, ML)      │
├─────────────────────────────────────────┤
│ Platform / Cloud    (ingestion, rules,   │
│                      storage, device mgmt)│
├─────────────────────────────────────────┤
│ Network / Transport (MQTT, CoAP, HTTP;   │
│                      Wi-Fi, cellular,    │
│                      LPWAN)               │
├─────────────────────────────────────────┤
│ Edge / Gateway      (aggregation, local  │
│                      processing, buffering)│
├─────────────────────────────────────────┤
│ Perception / Device (sensors, actuators, │
│                      MCUs)                │
└─────────────────────────────────────────┘
```

## Topologies

| Topology | Description | Best for |
|----------|-------------|----------|
| **Star** | Devices connect to a central hub/gateway | Simple home/office deployments |
| **Mesh** | Devices relay for each other | Coverage extension (Zigbee, Thread, BLE Mesh) |
| **Tree/hierarchical** | Layered aggregation | Large industrial sites |
| **Point-to-point** | Direct links | Dedicated sensor↔controller |

## Architectural Patterns

### Cloud-centric
All processing in the cloud. Simple, scalable; higher latency and bandwidth cost.

### Edge-first
Local processing on gateways/devices; cloud for backup and heavy analytics. Low
latency, offline-capable, privacy-friendly. See [Edge Computing](../applications/edge-computing.md).

### Fog computing
Intermediate layer of distributed nodes between edge and cloud, coined by the
OpenFog/IIC community — useful for regional aggregation in industrial deployments.

### Hybrid (most common in 2026)
Tiered: device → local hub (filter/aggregate) → regional edge → cloud. Send only
events and anomalies upstream to minimize bandwidth and cost.

## Key Design Considerations

- **Latency budget** — Real-time control demands edge processing (<10 ms)
- **Bandwidth & cost** — Filter/aggregate near the source; egress is expensive
- **Power** — Battery/harvested-energy devices dictate duty cycling and protocol choice
- **Connectivity reliability** — Plan for intermittent links; buffer and sync
- **Scale** — Provisioning, addressing, and device management at fleet scale
- **Security** — Segment IoT from IT networks; zero-trust between layers
- **Interoperability** — Standardize protocols (MQTT, OPC UA) to avoid silos

## Network Segmentation (Security)

Isolating IoT devices onto dedicated VLANs/segments limits **lateral movement** —
a primary attack technique where a compromised IoT device becomes a foothold into IT
networks. This is a baseline control in every serious IoT security framework. See
[IoT Security Overview](../security/overview.md).

## Connectivity Selection

| Need | Choose |
|------|--------|
| High bandwidth, mains power | Wi-Fi / Ethernet |
| Wide area, low data, low power | NB-IoT / LTE-M / LoRaWAN |
| Mid-tier 5G IoT | 5G RedCap (see [5G & Beyond](../trends/5g-connectivity.md)) |
| Short-range mesh | Thread / Zigbee / BLE Mesh |
| Personal devices | Bluetooth LE |

## References & Citations

1. ITU-T Y.4000/Y.2060. "Overview of the Internet of Things" — [itu.int](https://www.itu.int/rec/T-REC-Y.2060)
2. Industrial Internet Consortium. "Industrial Internet Reference Architecture (IIRA)" — [iiconsortium.org](https://www.iiconsortium.org/)
3. OpenFog Consortium. "OpenFog Reference Architecture" — [iiconsortium.org](https://www.iiconsortium.org/)
4. NIST SP 1800-? series on IoT — [nccoe.nist.gov](https://www.nccoe.nist.gov/)

## Related Topics

- [Cloud Platforms](./cloud-platforms.md)
- [Data Management](./data-management.md)
- [Edge Computing](../applications/edge-computing.md)
- [Wireless Communication Protocols](../protocols/wireless-communication.md)
- [IoT Security Overview](../security/overview.md)

---

**Document Version:** 1.0
**Last Updated:** 2026-06-20
**Contributed by:** IoT Index Project Team
