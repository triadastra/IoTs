# Wireless Communication Protocols in IoT

## Overview

Wireless communication is the backbone of IoT ecosystems. This document provides an overview of the major wireless protocols, their characteristics, and suitability for different IoT applications.

## Key Concepts

### Protocol Layers
- **Physical Layer** — Radio frequency, modulation, power consumption
- **Data Link Layer** — MAC protocols, collision avoidance
- **Network Layer** — Routing, addressing schemes
- **Application Layer** — Data formats, message structures

### Key Trade-offs
- **Range vs. Power** — Longer range typically requires more power
- **Throughput vs. Latency** — High data rates may introduce delays
- **Cost vs. Performance** — Cheaper solutions may have limitations

## Current Status (2026)

The IoT wireless landscape includes:
- **Cellular** — 4G LTE, 5G (low-latency, wide coverage)
- **Wi-Fi** — Wi-Fi 6E, Wi-Fi 7 (high throughput)
- **Low-Power Protocols** — Bluetooth, Zigbee, LoRaWAN, NB-IoT
- **Emerging** — Satellite IoT, mesh networks

## Major Protocols

### Low-Power Wide-Area Networks (LPWAN)
| Protocol | Range | Power | Data Rate | Use Case |
|----------|-------|-------|-----------|----------|
| LoRaWAN | 2-15 km | Very Low | 50 kbps | Remote sensors |
| NB-IoT | 1-10 km | Low | 250 kbps | Cellular IoT |
| Sigfox | 10-40 km | Ultra-low | 100 bps | Asset tracking |

### Short-Range Protocols
| Protocol | Range | Power | Data Rate | Use Case |
|----------|-------|-------|-----------|----------|
| Bluetooth 5 | 240 m | Low | 2 Mbps | Wearables, personal devices |
| Zigbee | 10-100 m | Low | 250 kbps | Home automation |
| Z-Wave | 30 m | Low | 100 kbps | Smart home |

## References & Citations

1. Sridhar Rajagopal et al. (2022). "Wireless Communication Protocols for IoT: A Comparative Study" — IEEE Communications Magazine
2. ITU-T Recommendation Y.4401 (2024) — "Overview and market analysis of the Internet of Things (IoT) and smart city services"
3. [3GPP Technical Specification TS 23.720](https://www.3gpp.org/) — Cellular IoT specifications
4. [LoRa Alliance Technical Documentation](https://lora-alliance.org/about/)

## Related Topics

- [MQTT Protocol](./mqtt.md)
- [Network Architecture](../architecture/network-architecture.md)
- [IoT Security](../security/overview.md)
- [5G & Beyond](../trends/5g-connectivity.md)

---

**Document Version:** 1.0
**Last Updated:** 2026-03-04
**Contributed by:** IoT Index Project Team
