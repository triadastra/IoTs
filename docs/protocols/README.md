# IoT Communication Protocols

This section covers the communication protocols and standards that form the foundation of IoT systems. Choosing the right protocol is critical for balancing power consumption, latency, range, and cost.

## Protocols Covered

- **[Wireless Communication Overview](./wireless-communication.md)** — Comparative overview of all wireless protocols
- **[MQTT](./mqtt.md)** — Lightweight publish-subscribe protocol (most common)
- **[CoAP](./coap.md)** — Request-response protocol for constrained devices
- **[Bluetooth & BLE](./bluetooth.md)** — Short-range personal area networks

## Quick Comparison

| Protocol | Range | Power | Latency | Use Case |
|----------|-------|-------|---------|----------|
| MQTT | Wide | Variable | Low | Distributed systems |
| CoAP | Variable | Low | Low | Sensors, constrained |
| Bluetooth | 240m | Low | Medium | Personal devices |
| LoRaWAN | 15km | Very Low | High | Remote sensors |
| 5G | Wide | Medium | Very Low | Real-time apps |

## Selection Guide

**Choose MQTT if:**
- Cloud-connected systems
- Need reliable message delivery
- Publish-subscribe pattern fits
- Variable throughput acceptable

**Choose CoAP if:**
- Constrained devices (battery-powered)
- Local networks preferred
- REST-like architecture
- Every byte matters

**Choose Bluetooth if:**
- Personal area network (< 240m)
- Mobile devices (phones, watches)
- Low power wearables
- Consumer applications

**Choose Cellular (5G/LTE) if:**
- Wide geographic coverage needed
- Mobile devices
- High throughput required
- Cost not primary concern

## Learning Path

1. Start with [Wireless Communication Overview](./wireless-communication.md)
2. Choose your primary protocol and dive deep
3. Understand security implications in each
4. Review [architecture](../architecture/) for integration patterns

---

**Last Updated:** 2026-03-04
