# Device Authentication & Identity

## Overview

Authentication answers a deceptively hard question: *is this device who it claims to
be?* In IoT, where devices are deployed in untrusted physical environments, lack
keyboards, and may live for a decade, establishing and maintaining trustworthy device
identity is foundational. **Weak or default credentials remain the #1 OWASP IoT
vulnerability** and the primary entry point for botnets like Mirai —
[OWASP IoT Top 10](https://owasp.org/www-project-internet-of-things/).

## Key Concepts

### Authentication vs. Authorization
- **Authentication** — Verifying identity ("who are you?")
- **Authorization** — Granting permissions ("what may you do?")

### Identity Mechanisms
| Mechanism | Strength | Notes |
|-----------|----------|-------|
| Username/password | Weak | Default credentials are the top IoT risk |
| Pre-shared keys (PSK) | Moderate | Simple; key distribution is the weak point |
| X.509 certificates | Strong | Scalable PKI; preferred for fleets |
| Token-based (JWT/OAuth) | Strong | Common for device-to-cloud APIs |
| Hardware root of trust | Strongest | TPM / secure element binds identity to silicon |

### Hardware Root of Trust
A **secure element** or **TPM** stores private keys in tamper-resistant hardware so
they can never be extracted. Combined with **secure boot**, this binds device
identity to the physical hardware and guarantees only signed firmware runs.

## The Device Identity Lifecycle

```
Manufacturing → Provisioning → Operation → Rotation → Decommission
   (inject       (onboard to     (mutual     (renew/    (revoke
    identity)     platform)       TLS auth)   re-key)    credentials)
```

- **Provisioning** — Securely onboarding a device and its credentials. Zero-touch
  provisioning injects identity at manufacture so no shared default secret exists.
- **Rotation** — Credentials and certificates must be renewable in the field; static
  lifetime keys are a liability over a 10-year device life.
- **Revocation** — Compromised or retired devices must be reliably de-authorized.

## Best Practices

1. **No default/shared credentials** — Unique per-device identity from the factory.
   (Regulations like the UK PSTI Act now ban universal default passwords.)
2. **Mutual TLS (mTLS)** — Both device and server authenticate each other.
3. **Hardware-backed keys** — Use a secure element/TPM where the threat model warrants.
4. **Secure boot + signed firmware** — Only authenticated code runs.
5. **Rotate and revoke** — Build credential renewal and revocation in from day one.
6. **Least privilege** — Scope each device's authorization to exactly what it needs.
7. **Zero-touch provisioning** — Eliminate human-handled shared secrets.

## Standards & Platform Support

- **X.509 / PKI** — The backbone of scalable device authentication
- **FIDO Device Onboard (FDO)** — Open standard for automated, secure onboarding
- **OPC UA** — Built-in certificate-based authentication for industrial systems
- **Cloud platforms** — AWS IoT, Azure IoT Hub, and Google Cloud all support
  certificate- and token-based device auth (see [Cloud Platforms](../architecture/cloud-platforms.md))

## Regulatory Drivers (2026)

- **UK PSTI Act** — Bans default passwords on consumer connectable products
- **EU Cyber Resilience Act** — Lifecycle security obligations, including
  authentication and secure updates (full enforcement expected 2027)
- **US Cyber Trust Mark** — Voluntary labeling signaling baseline security

## References & Citations

1. OWASP. "IoT Top 10 — I1: Weak, Guessable, or Hardcoded Passwords" — [owasp.org](https://owasp.org/www-project-internet-of-things/)
2. UK Government. "Product Security and Telecommunications Infrastructure (PSTI) Act" — [gov.uk](https://www.gov.uk/government/collections/the-product-security-and-telecommunications-infrastructure-psti-bill)
3. FIDO Alliance. "FIDO Device Onboard (FDO) Specification" — [fidoalliance.org](https://fidoalliance.org/device-onboarding-overview/)
4. NIST SP 800-213. "IoT Device Cybersecurity Guidance for the Federal Government" — [csrc.nist.gov](https://csrc.nist.gov/publications/detail/sp/800-213/final)

## Related Topics

- [IoT Security Overview](./overview.md)
- [Data Privacy](./privacy.md)
- [Cloud Platforms](../architecture/cloud-platforms.md)
- [Industrial IoT](../applications/industrial-iot.md)

---

**Document Version:** 1.0
**Last Updated:** 2026-06-20
**Contributed by:** IoT Index Project Team
