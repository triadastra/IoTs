# Bluetooth & Bluetooth Low Energy (BLE)

## Overview

Bluetooth is a short-range wireless technology ubiquitous in consumer and IoT
devices. For IoT, the relevant variant is **Bluetooth Low Energy (BLE)** —
introduced in Bluetooth 4.0 and substantially extended in versions 5.0–5.4 — which
trades raw throughput for very low power consumption, enabling coin-cell-powered
sensors and wearables to run for months or years.

Bluetooth is also one of the three radio technologies underpinning the
[Matter](../applications/smart-home.md) smart-home standard (used for device
commissioning), alongside Thread and Wi-Fi.

## Key Concepts

### Classic Bluetooth vs. BLE
- **Classic (BR/EDR)** — Continuous streaming (audio, file transfer); higher power
- **BLE** — Short bursts, sleeps between; ultra-low power; the IoT-relevant variant

### BLE Roles
- **Peripheral** — Advertises and is connected to (e.g., a sensor)
- **Central** — Scans and initiates connections (e.g., a phone or gateway)
- **Broadcaster / Observer** — Connectionless advertising (e.g., beacons)

### GATT (Generic Attribute Profile)
BLE data is organized as a hierarchy of **services** containing **characteristics**
(values a client can read, write, or subscribe to via notifications). This is the
core model you implement when building a BLE device.

## Current Status (2026)

- **Bluetooth 5.x** is standard: up to 2 Mbps (2M PHY), long-range coded PHY
  (~hundreds of meters line-of-sight), and advertising extensions.
- **Bluetooth Mesh** enables many-to-many networks for building/industrial lighting
  and sensing — hundreds of nodes relaying messages.
- **LE Audio** (with the LC3 codec) and **Auracast** broadcast audio are now shipping
  in mainstream devices, reshaping the hearables/accessibility space.
- **Channel Sounding** (Bluetooth 6.0, ratified 2024) adds accurate distance
  measurement for secure proximity and finding applications.

Standards and certification are managed by the
[Bluetooth Special Interest Group (SIG)](https://www.bluetooth.com/).

## Comparison with Other Short-Range Protocols

| Aspect | BLE | Zigbee | Thread | Wi-Fi |
|--------|-----|--------|--------|-------|
| Band | 2.4 GHz | 2.4 GHz | 2.4 GHz (802.15.4) | 2.4/5/6 GHz |
| Topology | Star / Mesh | Mesh | Mesh (IP-based) | Star |
| Power | Very Low | Low | Low | High |
| IP-native | No | No | Yes (IPv6/6LoWPAN) | Yes |
| Typical range | 10–100+ m | 10–100 m | 10–30 m | 30–50 m |
| Common use | Wearables, beacons | Home automation | Matter devices | High-bandwidth |

## Common Use Cases

- **Wearables** — Fitness trackers, smartwatches, medical patches
- **Beacons** — Indoor positioning, retail proximity, asset tags
- **Smart home** — Locks, sensors, and Matter device commissioning
- **Healthcare** — Glucose monitors, pulse oximeters, hearing aids (LE Audio)
- **Industrial** — Bluetooth Mesh for connected lighting and condition monitoring

## Security Considerations

- Use **LE Secure Connections** (ECDH-based pairing, introduced in 4.2) rather than
  legacy pairing.
- Beware passive eavesdropping and MITM during pairing — use numeric comparison or
  passkey association models, not "Just Works," for sensitive devices.
- **Address randomization** (resolvable private addresses) mitigates device tracking;
  ensure it is enabled for privacy-sensitive products.
- Historic vulnerability classes (e.g., KNOB, BLESA, BIAS) targeted pairing/encryption
  negotiation — keep stacks patched.

## References & Citations

1. Bluetooth SIG (2024). "Bluetooth Core Specification 6.0" — [bluetooth.com](https://www.bluetooth.com/specifications/specs/core-specification-6-0/)
2. Bluetooth SIG (2023). "LE Audio and Auracast Broadcast Audio" — [bluetooth.com/auracast](https://www.bluetooth.com/auracast/)
3. Connectivity Standards Alliance — Matter uses BLE for commissioning, [csa-iot.org](https://csa-iot.org/)
4. NIST SP 800-121 Rev. 2, "Guide to Bluetooth Security" — [csrc.nist.gov](https://csrc.nist.gov/publications/detail/sp/800-121/rev-2/final)

## Related Topics

- [Wireless Communication Protocols](./wireless-communication.md)
- [Smart Home](../applications/smart-home.md)
- [Healthcare IoT](../applications/healthcare-iot.md)
- [IoT Security Overview](../security/overview.md)

---

**Document Version:** 1.0
**Last Updated:** 2026-06-20
**Contributed by:** IoT Index Project Team
