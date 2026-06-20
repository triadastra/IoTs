# CoAP: Constrained Application Protocol

## Overview

CoAP (Constrained Application Protocol) is a lightweight, RESTful protocol designed for resource-constrained IoT devices and networks with limited bandwidth. Unlike MQTT's publish-subscribe model, CoAP uses a request-response pattern and is particularly suited for devices with minimal memory and power budgets.

## Key Concepts

### Request-Response Model
- **Client** — Initiates requests to servers
- **Server** — Responds to client requests
- **Resources** — Identified by URIs (e.g., `/sensors/temperature`)
- **Methods** — GET, POST, PUT, DELETE (similar to HTTP)

### Message Types
- **Confirmable (CON)** — Requires acknowledgment
- **Non-confirmable (NON)** — Fire-and-forget
- **Acknowledgment (ACK)** — Response to CON messages
- **Reset (RST)** — Sender cannot process message

### Key Features
- **Lightweight** — Small message headers (4 bytes minimum)
- **Observe Pattern** — Server-push notifications for resource changes
- **Blockwise Transfers** — Split large messages into blocks
- **UDP-based** — Lower overhead than TCP
- **Built-in Security** — DTLS (Datagram TLS) support

## Current Status (2026)

### Adoption
- Widely used in constrained IoT environments
- Growing adoption in industrial IoT and sensor networks
- Competing with MQTT in certain domains

### Standards
- **RFC 7252** (2014) — Core CoAP specification
- **RFC 7748** — Update algorithms for secure communication
- **RFC 8613** — OSCORE (Object Security for Constrained RESTful Environments)

## Comparison with MQTT

| Aspect | CoAP | MQTT |
|--------|------|------|
| Pattern | Request-Response | Publish-Subscribe |
| Transport | UDP | TCP |
| Overhead | Very Low | Low |
| Messages Size | Small (4+ bytes) | Small |
| Latency | Low | Very Low |
| Server Push | Observe pattern | Native |
| Standardization | IETF RFC | ISO/IEC |
| Complexity | Simple | Medium |

## Use Cases

### Sensor Networks
- Environmental monitoring
- Building automation
- Agriculture IoT (soil moisture, weather)

### Energy-Constrained Devices
- Battery-powered sensors (years of operation)
- Wireless mesh networks
- Low-power wide-area networks (LPWAN)

### Embedded Systems
- Microcontroller-based IoT devices
- Wearables with minimal resources
- Industrial equipment monitoring

## Architecture Example

```
[CoAP Client (Sensor)]
        ↓ (UDP/DTLS)
[CoAP Server/Proxy]
        ↓
[Backend Application]
```

## Security Considerations

### DTLS (Datagram TLS)
- End-to-end encryption
- Message authentication
- Pre-shared keys or certificates
- Less overhead than TLS due to UDP

### OSCORE
- Object-level security
- Lightweight encryption with CBOR format
- Suitable for highly constrained devices

## Advantages & Limitations

### Advantages
- Extremely lightweight
- Low power consumption
- Natural fit for REST architecture
- Good for sensor/actuator networks

### Limitations
- No persistence like MQTT queues
- Less suitable for reliable message delivery
- Smaller ecosystem than MQTT
- Fewer commercial integrations

## References & Citations

1. Shelby, Z., Hartke, K., & Bormann, C. (2014). "The Constrained Application Protocol (CoAP)" — RFC 7252
2. Gutmann, P. (2018). "OSCORE: Object Security for Constrained RESTful Environments" — RFC 8613
3. Schilcher, U., & Braun, T. (2024). "CoAP in Industrial IoT Environments" — IEEE IoT Journal
4. [IETF Constrained RESTful Environments (CoRE)](https://datatracker.ietf.org/wg/core/) — Official specification
5. [Californium Project](https://www.eclipse.org/californium/) — Open-source CoAP implementation

## Related Topics

- [Wireless Communication Protocols](./wireless-communication.md)
- [MQTT Protocol](./mqtt.md)
- [Edge Computing](../applications/edge-computing.md)
- [IoT Security](../security/overview.md)

---

**Document Version:** 1.0
**Last Updated:** 2026-03-04
**Contributed by:** IoT Index Project Team
