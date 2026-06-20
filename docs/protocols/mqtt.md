# MQTT: Message Queuing Telemetry Transport

## Overview

MQTT is a lightweight, publish-subscribe message protocol designed for IoT and mobile applications. It is one of the most widely adopted protocols in IoT ecosystems due to its simplicity, low bandwidth requirements, and efficient use of network resources.

## Key Concepts

### Publish-Subscribe Model
- **Publishers** — Send messages to topics without knowing subscribers
- **Subscribers** — Receive messages from topics of interest
- **Broker** — Central message router that manages pub/sub relationships
- **Topics** — Hierarchical message channels (e.g., `home/livingroom/temperature`)

### Quality of Service (QoS) Levels
- **QoS 0** — At most once (fire and forget)
- **QoS 1** — At least once (guaranteed delivery)
- **QoS 2** — Exactly once (most reliable)

### Key Features
- Lightweight protocol (minimal overhead)
- Persistent connections with keep-alive
- Last Will and Testament (LWT) for detecting disconnections
- Wildcard subscriptions (+, #)

## Current Status (2026)

### Adoption
- Dominant protocol in IoT messaging (estimated 70%+ of IoT deployments)
- Supported by all major cloud platforms (AWS IoT, Azure IoT Hub, Google Cloud)
- Growing use in edge computing and 5G IoT

### Standards
- **MQTT 3.1.1** (2014) — Widely deployed
- **MQTT 5.0** (2019) — Enhanced features: properties, shared subscriptions, flow control
- **MQTT SN** — Sensor Networks variant for resource-constrained devices

## Common Use Cases

1. **Smart Home** — Temperature sensors, smart lights, security systems
2. **Industrial IoT** — Manufacturing automation, predictive maintenance
3. **Remote Monitoring** — Asset tracking, environmental sensors
4. **Real-time Applications** — Live dashboards, alert systems

## Architecture Example

```
[IoT Devices] ──→ [MQTT Broker] ←── [Applications]
   (Publish)          (Route)        (Subscribe)
```

## References & Citations

1. OASIS Standard (2019). "MQTT Version 5.0" — Official specification
2. Andrew Banks & Rahul Gupta (2019). "MQTT Essentials" — O'Reilly Media
3. Lightbend & Pivotal Cloud (2021). "IoT Platforms and MQTT: A Comprehensive Survey"
4. [Official MQTT.org](https://mqtt.org/) — Protocol documentation and resources
5. [HiveMQ Blog](https://www.hivemq.com/blog/) — Industry insights and tutorials

## Comparison with Alternatives

| Aspect | MQTT | CoAP | HTTP |
|--------|------|------|------|
| Model | Pub/Sub | Request/Response | Request/Response |
| Overhead | Very Low | Low | Medium |
| Latency | Very Low | Low | Medium-High |
| Scalability | Excellent | Good | Fair |
| Firewall Friendly | Less (port 1883) | No (UDP) | Yes (port 80/443) |

## Security Considerations

- Use TLS/SSL encryption (port 8883)
- Implement username/password or certificate authentication
- Control topic access with ACLs
- Monitor for unusual publish patterns

## Related Topics

- [Wireless Communication Protocols](./wireless-communication.md)
- [IoT Security Overview](../security/overview.md)
- [Cloud Platforms](../architecture/cloud-platforms.md)
- [Network Architecture](../architecture/network-architecture.md)

---

**Document Version:** 1.0
**Last Updated:** 2026-03-04
**Contributed by:** IoT Index Project Team
