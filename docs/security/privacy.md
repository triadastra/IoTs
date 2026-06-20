# Data Privacy in IoT

## Overview

IoT devices are prolific data collectors — capturing location, audio, video,
biometrics, energy usage, and behavioral patterns, often continuously and in
intimate spaces (homes, bodies, vehicles). This makes privacy a first-class design
concern, not an afterthought. Privacy and [security](./overview.md) are related but
distinct: security protects data from unauthorized access; privacy governs what is
collected, why, and who may use it.

## Key Concepts

### Privacy-by-Design (7 Principles)
Ann Cavoukian's framework, now embedded in regulation:
1. Proactive, not reactive
2. Privacy as the default setting
3. Privacy embedded into design
4. Full functionality (positive-sum, not zero-sum)
5. End-to-end security across the lifecycle
6. Visibility and transparency
7. Respect for user privacy (user-centric)

### Data Minimization
Collect only what is needed, retain it only as long as needed, and process it as
close to the source as possible. On-device inference (see
[AI/ML in IoT](../trends/ai-ml-iot.md)) is a powerful privacy lever: raw audio/video
never leaves the device; only derived events do.

### Key Definitions
- **PII** — Personally identifiable information
- **Data controller / processor** — Roles under GDPR with distinct obligations
- **Consent** — Freely given, specific, informed, unambiguous
- **Re-identification** — Combining "anonymous" datasets to identify individuals

## Regulatory Landscape (2026)

| Regulation | Region | IoT-relevant requirement |
|------------|--------|--------------------------|
| **GDPR** | EU | Lawful basis, consent, data minimization, breach notification, DPIA |
| **EU Data Act** | EU | User access to and portability of IoT-generated data |
| **CCPA/CPRA** | California | Disclosure, opt-out of sale, sensitive-data limits |
| **HIPAA** | US (health) | Protection of health data in IoMT |
| **EU Cyber Resilience Act** | EU | Security across product lifecycle (enables privacy) |

The **EU Data Act** is especially consequential for IoT: it gives users rights over
the data their connected products generate, reshaping who controls device telemetry.

## Privacy Threats Specific to IoT

- **Inference attacks** — Deriving sensitive facts (occupancy, health, habits) from
  innocuous data like power draw or motion
- **Always-on sensing** — Microphones/cameras capturing bystanders who never consented
- **Device fingerprinting & tracking** — Persistent identifiers (e.g., MAC, BLE
  addresses) enabling cross-context tracking
- **Data aggregation** — Combining streams across devices to build detailed profiles
- **Opaque data flows** — Cloud back-ends and third-party SDKs sharing data invisibly

## Best Practices

1. **Minimize** — Collect and retain the least data necessary
2. **Process at the edge** — Keep raw sensitive data on-device
3. **Encrypt** — In transit (TLS) and at rest
4. **Randomize identifiers** — Use rotating/resolvable addresses
5. **Be transparent** — Clear privacy notices, in-product indicators (e.g., camera LEDs)
6. **Honor user control** — Easy access, export, and deletion
7. **Run DPIAs** — Assess privacy impact before deployment
8. **Default to private** — Privacy-protective settings out of the box

## References & Citations

1. EU (2016). "General Data Protection Regulation (GDPR)" — [gdpr.eu](https://gdpr.eu/)
2. EU (2023/2854). "Data Act" — [digital-strategy.ec.europa.eu](https://digital-strategy.ec.europa.eu/en/policies/data-act)
3. Cavoukian, A. "Privacy by Design: The 7 Foundational Principles" — [iapp.org](https://iapp.org/)
4. NIST (2020). "Privacy Framework 1.0" — [nist.gov/privacy-framework](https://www.nist.gov/privacy-framework)
5. State of California. "California Privacy Rights Act (CPRA)" — [cppa.ca.gov](https://cppa.ca.gov/)

## Related Topics

- [IoT Security Overview](./overview.md)
- [Device Authentication](./authentication.md)
- [AI/ML in IoT](../trends/ai-ml-iot.md)
- [Healthcare IoT](../applications/healthcare-iot.md)

---

**Document Version:** 1.0
**Last Updated:** 2026-06-20
**Contributed by:** IoT Index Project Team
