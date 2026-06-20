# Sustainability & Green IoT

## Overview

Sustainability has moved from a marketing talking point to an engineering constraint
in IoT. With tens of billions of devices deployed, the aggregate energy, battery
waste, and e-waste footprint is significant. "Green IoT" covers two complementary
goals: **making IoT itself sustainable** (low-power, battery-free, recyclable
devices) and **using IoT to make other systems sustainable** (smart grids, precision
agriculture, energy monitoring).

A defining 2026 development is the maturation of **Ambient IoT** — battery-free
devices powered by harvested ambient energy (light, RF, vibration, heat).

## Key Concepts

### Energy Harvesting Sources
- **Photovoltaic** — Indoor/outdoor light (most mature for sensors)
- **RF / backscatter** — Reflecting ambient radio signals (very low power, no battery)
- **Thermoelectric** — Temperature gradients
- **Piezoelectric / kinetic** — Vibration and motion

### Ambient IoT
Devices that operate **without a battery**, harvesting energy from the environment and
often communicating via **backscatter**. The 3GPP is standardizing Ambient IoT in
**Release 19 and 20**, extending cellular IoT (NB-IoT, LTE-M, RedCap) toward
zero-energy devices — [arXiv 2511.09372](https://arxiv.org/pdf/2511.09372).

### Sustainable Design Principles
- Duty cycling and aggressive sleep states
- Edge processing to cut transmission energy (see [AI/ML in IoT](./ai-ml-iot.md))
- Recyclable / repairable hardware and longer support lifecycles
- Firmware longevity to keep devices useful (and secure) for years

## Current Status (2026)

- **Energy-harvesting IoT is reaching commercial scale.** Indoor-photovoltaic-powered
  LTE-M/NB-IoT sensors (e.g., Sequans + e-peas designs) and battery-free asset tags
  are shipping — [IoT Business News](https://iotbusinessnews.com/2025/11/26/energy-harvesting-iot-practical-applications-finally-reaching-scale-in-2026/).
- **Backscatter range improvements** (meta-backscatter up to ~10 m) make chipless and
  battery-free tags viable beyond near-field — [arXiv 2511.09372](https://arxiv.org/pdf/2511.09372).
- **Regulatory tailwinds**: lifecycle requirements in the EU Cyber Resilience Act and
  right-to-repair / e-waste rules push longer device support windows.

## IoT *for* Sustainability

| Application | Sustainability impact |
|-------------|----------------------|
| Smart grids & metering | Demand-side management, reduced peak load |
| Precision agriculture | Less water, fertilizer, and pesticide use |
| Building automation | HVAC/lighting optimization; 10–30% energy savings |
| Asset & fleet tracking | Route optimization, reduced fuel/emissions |
| Environmental sensing | Air/water quality, emissions monitoring |

## Challenges

- **Battery waste** — Billions of coin cells; battery-free designs are the long-term fix
- **E-waste** — Short product lifecycles and non-repairable designs
- **Embodied carbon** — Manufacturing footprint of devices and semiconductors
- **Energy vs. capability** — Harvested energy budgets constrain compute and radio duty
  cycle; careful co-design is required

## References & Citations

1. "Generation-Agnostic Zero-Energy Devices for Sustainable Connectivity, Sensing, and Localization" (2025) — [arXiv 2511.09372](https://arxiv.org/pdf/2511.09372)
2. IoT Business News (2025). "Energy-Harvesting IoT: Practical Applications Finally Reaching Scale in 2026" — [iotbusinessnews.com](https://iotbusinessnews.com/2025/11/26/energy-harvesting-iot-practical-applications-finally-reaching-scale-in-2026/)
3. 3GPP — Ambient IoT in Release 19/20, [3gpp.org](https://www.3gpp.org/)
4. Wiliot — Ambient IoT / battery-free tags, [wiliot.com/ambient-iot](https://www.wiliot.com/ambient-iot)

## Related Topics

- [5G & Beyond](./5g-connectivity.md)
- [AI/ML in IoT](./ai-ml-iot.md)
- [Wireless Communication Protocols](../protocols/wireless-communication.md)
- [Edge Computing](../applications/edge-computing.md)

---

**Document Version:** 1.0
**Last Updated:** 2026-06-20
**Contributed by:** IoT Index Project Team
