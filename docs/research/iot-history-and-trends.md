# Internet of Things: Development History, Current Trends, and Flagship Technologies

**A General Trend Research Overview**

---

## Abstract

The Internet of Things (IoT) describes a global infrastructure of networked physical devices equipped with sensors, actuators, and communication capabilities that collect, exchange, and act upon data with minimal human intervention. This document surveys the development history of IoT from its conceptual origins in the early nineteenth century through to present-day deployments, examines key contributing companies and research institutions, reviews foundational academic literature, and characterizes the dominant technological trends and representative commercial products of 2024 to 2025. Particular attention is given to device capabilities, communication protocols, and power consumption characteristics, as these factors increasingly determine deployment feasibility at scale.

**Keywords:** Internet of Things, IoT, IIoT, AIoT, edge computing, LPWAN, 5G, Matter, smart home, industrial IoT, embedded systems, wireless sensor networks

---

## Table of Contents

1. [Introduction](#1-introduction)
2. [Development History](#2-development-history)
3. [Key Contributing Companies and Products](#3-key-contributing-companies-and-products)
4. [Foundational Research and Standards](#4-foundational-research-and-standards)
5. [Current Trends](#5-current-trends)
6. [Flagship Products (2024-2025)](#6-flagship-products-2024-2025)
7. [Key Facts](#7-key-facts)
8. [Conclusion](#8-conclusion)
9. [References](#9-references)

---

## 1. Introduction

The term "Internet of Things" was formally introduced in 1999, but the underlying paradigm of machine-to-machine (M2M) communication and remote sensing has evolved over more than a century. What distinguishes contemporary IoT from earlier telemetry and SCADA systems is the convergence of low-cost microcontrollers, ubiquitous wireless connectivity, cloud computing infrastructure, and artificial intelligence — all of which have reached commercial maturity simultaneously over the past decade.

IoT systems now span consumer electronics, industrial process control, healthcare monitoring, smart city infrastructure, agricultural automation, and supply chain logistics. The heterogeneity of these application domains, combined with differing requirements for latency, bandwidth, power consumption, and security, has produced a correspondingly diverse ecosystem of hardware, protocols, and platforms.

This document provides a structured overview of IoT's developmental arc, the organizations that shaped it, the academic literature that has defined its theoretical foundations, and the technological trends that are driving its continued expansion.

---

## 2. Development History

### 2.1 Origins and Pre-IoT Foundations

The conceptual roots of the Internet of Things extend to the invention of the **electromagnetic telegraph** (1832), one of the earliest demonstrations of electrical M2M signal transmission over distance. By the 1970s, industrial telemetry and SCADA (Supervisory Control and Data Acquisition) systems enabled centralized monitoring of distributed physical infrastructure in sectors such as energy, water, and manufacturing.

A widely cited early prototype of internet-connected sensing appeared in the **early 1980s at Carnegie Mellon University**, where researchers connected a Coca-Cola vending machine to the ARPANET, enabling it to report inventory levels and beverage temperature — regarded as one of the first internet-connected embedded devices. [1]

### 2.2 Coining of the Term (1999)

The phrase **"Internet of Things"** was coined by **Kevin Ashton** in 1999 while employed at **Procter & Gamble**, where he proposed attaching RFID (Radio Frequency Identification) tags to consumer goods to enable automated inventory tracking. Ashton described IoT as a system in which physical objects communicate autonomously over networks without human mediation. He subsequently co-founded the **Auto-ID Center at MIT**, which became a primary research institution for RFID standards and supply-chain IoT. [2] [3]

### 2.3 Early Commercial Development (1995-2009)

The period from the mid-1990s to the end of the 2000s saw the first commercial M2M products and the initial recognition of IoT as a distinct technology category:

- **1995:** Siemens introduced an early commercial M2M GSM data module (the Siemens M1), one of the first cellular modules designed for remote equipment monitoring. [4]
- **2000:** LG Electronics announced the first internet-connected refrigerator, featuring an LCD display and online grocery ordering capability.
- **2003:** BigBelly Solar deployed internet-connected solar-powered trash compactors in Boston, capable of reporting fill levels and optimizing collection routes. [4]
- **2005:** The International Telecommunication Union (ITU) published the landmark report *"The Internet of Things"*, formally recognizing IoT as a global technological paradigm shift. [5]
- **2008:** The IPSO Alliance (Internet Protocol for Smart Objects) was established to promote IP-based networking for constrained devices.
- **2008-2009:** The number of internet-connected devices worldwide exceeded the global human population for the first time, a milestone documented by Cisco Systems in their IoT white paper series. [6]

### 2.4 Mainstream Adoption (2010-2019)

The 2010s saw rapid consumer and industrial adoption, the emergence of major platform players, and the first large-scale IoT security incidents:

- **2011:** Nest Labs (founded by former Apple engineers Tony Fadell and Matt Rogers) released the Nest Learning Thermostat, one of the defining consumer IoT products, employing machine learning to adapt to household schedules. Google acquired Nest in 2014 for $3.2 billion. [4]
- **2012:** Global launch of IPv6 provided an address space of approximately 3.4 x 10^38 addresses, removing a fundamental constraint on IoT device addressing. [3]
- **2013:** The AllSeen Alliance (Qualcomm, Microsoft, and others) and the Open Internet Consortium (Intel, Samsung) were established to develop open interoperability frameworks for IoT devices.
- **2014:** Amazon launched the Echo smart speaker with the Alexa voice assistant, becoming one of the highest-volume consumer IoT products in history.
- **2015:** Apple launched HomeKit, a framework for smart home device control via iOS. Samsung acquired SmartThings for $200 million.
- **2016:** The Mirai botnet attack exploited insecure IoT devices (IP cameras and DVRs) to execute one of the largest distributed denial-of-service (DDoS) attacks recorded at that time, demonstrating the systemic security risks of poorly secured connected devices. [3]
- **2017-2019:** NB-IoT (Narrowband IoT) and LTE-M were deployed globally by mobile network operators, providing low-power wide-area connectivity infrastructure for large-scale IoT deployments.

### 2.5 The AI and Connectivity Era (2020-Present)

- **2020-2022:** The COVID-19 pandemic accelerated IoT adoption in healthcare (remote patient monitoring, contact tracing wearables) and logistics (automated warehouses and supply chain visibility).
- **2022:** The Matter standard, backed by Apple, Google, Amazon, and Samsung, was released, providing a unified application-layer protocol for smart home devices aimed at resolving ecosystem fragmentation. [6]
- **2023-2025:** The convergence of artificial intelligence with IoT (AIoT), the rollout of 5G networks, and the proliferation of edge computing define the current phase. Industrial IoT (IIoT) is projected to overtake consumer IoT in total market value within this period.

---

## 3. Key Contributing Companies and Products

The following organizations have made material contributions to the development of IoT infrastructure, standards, hardware, or platforms:

| Company | Primary IoT Contribution | Notable Product(s) |
|---|---|---|
| Amazon | Consumer IoT and cloud platform | Echo/Alexa, AWS IoT Core |
| Google / Nest | Smart home and AI integration | Nest Learning Thermostat, Google Home |
| Apple | Consumer ecosystem and standards | Apple Watch, HomeKit |
| Microsoft | Enterprise IoT platform | Azure IoT Hub, Azure Digital Twins |
| Cisco | IoT networking and security | Cisco IoT Control Center, Catalyst IR routers |
| Intel | IoT edge hardware | Atom x6000E series (Elkhart Lake), OpenVINO AI toolkit |
| Siemens | Industrial IoT (IIoT) | MindSphere IIoT platform, SIMATIC controllers |
| GE (General Electric) | Industrial analytics | Predix IIoT platform |
| Qualcomm | IoT chipsets | Snapdragon IoT platforms, QCS6490 |
| Nordic Semiconductor | Ultra-low-power wireless chipsets | nRF52840, nRF9160 (LTE-M/NB-IoT) |
| Texas Instruments | Embedded IoT processors | CC2652, SimpleLink MCU family |
| Bosch | Sensors and connected mobility | Bosch IoT Suite, MEMS sensor portfolio |
| Samsung | Smart home and connectivity | SmartThings, Galaxy Watch |
| Particle Industries | IoT development platform | Particle Boron (LTE), Tracker One |
| Raspberry Pi Foundation | Open-source IoT hardware | Raspberry Pi 5, Raspberry Pi Pico W |

---

## 4. Foundational Research and Standards

### 4.1 Foundational Academic Works

The following peer-reviewed publications represent landmarks in the academic literature on IoT:

**Ashton, K. (2009).** "That 'Internet of Things' Thing." *RFID Journal.* The original essay formalizing the IoT concept by the person who coined the term. [2]

**Atzori, L., Iera, A., & Morabito, G. (2010).** "The Internet of Things: A survey." *Computer Networks, 54*(15), 2787-2805. One of the most highly cited IoT papers, covering key enabling technologies including RFID, sensors, middleware, and application domains. [7]

**Gubbi, J., Buyya, R., Marusic, S., & Palaniswami, M. (2013).** "Internet of Things (IoT): A vision, architectural elements, and future directions." *Future Generation Computer Systems, 29*(7), 1645-1660. Introduces a cloud-centric architectural reference model widely adopted in subsequent research. [8]

**Zanella, A., Bui, N., Castellani, A., Vangelista, L., & Zorzi, M. (2014).** "Internet of Things for Smart Cities." *IEEE Internet of Things Journal, 1*(1), 22-32. A foundational paper on applying IoT infrastructure at urban scale. [9]

**Al-Fuqaha, A., Guizani, M., Mohammadi, M., Aledhari, M., & Ayyash, M. (2015).** "Internet of Things: A Survey on Enabling Technologies, Protocols, and Applications." *IEEE Communications Surveys & Tutorials, 17*(4), 2347-2376. A comprehensive survey of IoT protocols (MQTT, CoAP, AMQP), enabling technologies, and application categories. [10]

**Choudhary, G., et al. (2024).** "Internet of Things: a comprehensive overview, architectures, applications, and research challenges." *Cluster Computing (Springer Nature).* A recent meta-review of IoT research across architectures, security, and emerging applications. [11]

### 4.2 Key Standards and Regulatory Bodies

- **ITU-T Y.2060 (2012):** International Telecommunication Union standard establishing the overview, definitions, and requirements for IoT. [5]
- **IEEE P2413:** Standard for an Architectural Framework for the Internet of Things, providing cross-domain interoperability guidance.
- **3GPP Release 13 (2016):** Standardized NB-IoT and LTE-M, the foundational LPWAN cellular protocols for IoT.
- **Connectivity Standards Alliance (formerly Zigbee Alliance):** Maintains the Matter and Zigbee standards for smart home device interoperability.

---

## 5. Current Trends

### 5.1 AI and IoT Convergence (AIoT)

Artificial intelligence is being embedded directly into IoT pipelines at the device level (TinyML and edge AI), enabling real-time inference without cloud dependency and substantially reducing end-to-end latency. By 2025, an estimated 70% of enterprise IoT deployments are expected to incorporate real-time machine learning. [12] Representative deployments include AI-powered predictive maintenance sensors in automotive and industrial manufacturing, and edge AI camera systems used for dynamic traffic management in smart city installations.

### 5.2 Edge Computing

Rather than transmitting all sensor data to centralized cloud infrastructure, edge gateways and edge servers process data proximate to its source. By 2025, 75% of enterprise-generated data is projected to be processed outside centralized data centers. [13] Edge computing reduces latency, lowers bandwidth costs, and enables deterministic responses in safety-critical applications such as autonomous vehicles and smart grid management.

### 5.3 5G and 5G RedCap

Fifth-generation cellular networks, characterized by sub-millisecond latency and throughput up to 10 Gbps, are enabling industrial and real-time IoT applications not previously feasible on 4G infrastructure. The 5G RedCap (Reduced Capability) specification, standardized in 3GPP Release 17, simplifies 5G module design and reduces power consumption by approximately 65% relative to full 5G, making cellular connectivity practical for wearables, smart meters, and distributed sensors. [14]

### 5.4 Low Power Wide Area Networks (LPWAN)

LPWAN protocols are purpose-built for battery-operated, low-data-rate sensors requiring multi-kilometer range. The following table summarizes the principal protocols:

| Protocol | Range | Power Profile | Data Rate | Typical Battery Life |
|---|---|---|---|---|
| NB-IoT | 10-35 km (rural) | Ultra-low | 20-250 kbps | 10+ years |
| LoRaWAN | 5-15 km (urban) | Ultra-low | 0.3-50 kbps | 10+ years |
| LTE-M | Cellular coverage | Low | 1 Mbps | 5-10 years |
| Bluetooth 5.4 LE | ~100 m | Very low | Up to 2 Mbps | 1-5 years |
| Zigbee | ~100 m (mesh) | Very low | 250 kbps | 2-5 years |

By 2025, LoRaWAN-connected nodes are projected to exceed 2 billion; Bluetooth Low Energy devices may reach 26 billion cumulatively. [15]

### 5.5 Matter Standard and Smart Home Interoperability

Released in 2022 and maintained by the Connectivity Standards Alliance with backing from Apple, Google, Amazon, and Samsung, the Matter standard provides a unified application layer for smart home devices operating over Wi-Fi and Thread (an IPv6-based mesh protocol). Matter resolves years of protocol fragmentation across competing smart home ecosystems and enables devices from different manufacturers to interoperate without proprietary bridges. [6]

### 5.6 Non-Terrestrial Networks and Satellite IoT

Satellite constellations — including SpaceX Starlink, Iridium, and Orbcomm — are extending IoT connectivity to remote locations without terrestrial network infrastructure, including maritime, agricultural, and polar deployments. eSIM and iSIM technologies enable over-the-air network provisioning and operator switching, simplifying global device deployments. [16]

### 5.7 Security and Zero Trust Architecture

Following the Mirai botnet incident and subsequent large-scale IoT compromises, security has become a primary engineering and regulatory concern. Current best practices include AES-256 encryption at rest and in transit, mutual TLS (mTLS) for device authentication, secure boot with firmware attestation, and Zero Trust Architecture principles under which no network-connected device is inherently trusted. The EU Cyber Resilience Act (2024) and the US IoT Cybersecurity Improvement Act (2020) are establishing mandatory security baselines for commercial IoT products. [13]

### 5.8 Sustainability and Power Efficiency

The proliferation of billions of always-on sensors, gateways, and associated cloud infrastructure represents a growing contributor to global electricity demand. Industry responses include energy harvesting (solar, kinetic, and thermoelectric), ultra-low-power microcontrollers, aggressive duty-cycling and deep-sleep modes capable of extending battery life to ten or more years, and software-defined power management in cloud IoT platforms. [13] [15]

---

## 6. Flagship Products (2024-2025)

### 6.1 Consumer IoT

| Product | Manufacturer | Key Capability | Power Specification |
|---|---|---|---|
| Echo Show 15 | Amazon | 15.6" smart display, Alexa AI, visual recognition | 30 W |
| Apple Watch Series 10 | Apple | ECG, blood oxygen, sleep apnea detection, LTE | ~1.4 Wh battery, ~18 hr life |
| Nest Learning Thermostat (4th Gen) | Google/Nest | AI scheduling, Farsight display, Matter/Thread | ~1.5 W average |
| SmartThings Station | Samsung | Matter/Thread hub, Qi2 wireless charging, 200+ device types | 15 W |
| Arlo Pro 5S 2K | Arlo | 2K color night vision, AI motion zones, wire-free | Solar or 14,450 mAh battery |
| Tile Ultra | Life360 | UWB + Bluetooth precise finding, 400 ft range | CR2032 coin cell, ~1 year |

### 6.2 Industrial and Enterprise IoT

| Product | Manufacturer | Key Capability | Power Specification |
|---|---|---|---|
| SIMATIC IOT2050 | Siemens | Industrial edge gateway, dual-core ARM, Python/Node-RED | 12-24 V DC, ~15 W |
| Catalyst IR1101 | Cisco | Industrial router, LTE/5G, DIN-rail mount, IOS-XE | -40°C to +60°C, 18 W |
| Experion PKS IoT | Honeywell | Process control and IIoT integration, AI analytics | Varies (enterprise system) |
| ctrlX CORE | Bosch Rexroth | Real-time Linux controller, OPC-UA, 5G-ready | 24 V DC, 35 W max |
| ThingWorx 9.x | PTC | Industrial IoT platform, AR integration, digital twin | Cloud/on-premise |

### 6.3 Medical and Healthcare IoT

| Product | Manufacturer | Key Capability | Power Specification |
|---|---|---|---|
| FreeStyle Libre 3 | Abbott | Continuous glucose monitoring, 14-day wear, phone alerts | Disposable sensor, ~0.24 mW |
| Biosensor BX100 | Philips | Wearable biometric patch (HR, RR, posture, fall detection) | 7-day disposable patch |
| Dexcom G7 | Dexcom | Real-time CGM, 10-day wear, Apple Watch/Android integration | ~0.15 mW average |

### 6.4 Development Platforms and Modules

| Product | Manufacturer | Key Capability | Power Specification |
|---|---|---|---|
| Raspberry Pi 5 | Raspberry Pi Foundation | Quad-core Cortex-A76 @ 2.4 GHz, PCIe 2.0, 8 GB RAM | 5 V / 5 A (25 W max) |
| nRF9161 DK | Nordic Semiconductor | LTE-M/NB-IoT/GNSS SiP, Arm Cortex-M33 | PSM sleep: ~2.5 µA |
| ESP32-S3 | Espressif | Dual-core Xtensa LX7, Wi-Fi 4, BLE 5.0, AI accelerator | Deep sleep: 7 µA |
| Particle Boron | Particle Industries | LTE-M/NB-IoT cellular, cloud OTA, Arduino-compatible | Deep sleep: ~0.16 mA |
| STM32U5 | STMicroelectronics | Ultra-low-power Cortex-M33, TrustZone, AES hardware | Run mode: 19 µA/MHz |

---

## 7. Key Facts

The following points summarize the most important findings from this survey:

1. The term "Internet of Things" was coined by Kevin Ashton at Procter & Gamble in 1999 and formalized through research at the MIT Auto-ID Center. [2]
2. One of the first internet-connected devices was a Coca-Cola vending machine connected to the ARPANET at Carnegie Mellon University in the early 1980s. [1]
3. By 2008-2009, the number of internet-connected devices surpassed the global human population, a threshold cited by Cisco as marking the birth of modern IoT. [6]
4. The global IPv6 launch in 2012 provided approximately 3.4 x 10^38 unique addresses, resolving the IP address exhaustion that would otherwise have constrained IoT growth. [3]
5. Google acquired Nest Labs in 2014 for $3.2 billion, signaling the high strategic value major technology companies placed on IoT data and infrastructure. [4]
6. The 2016 Mirai botnet attack demonstrated that insecure IoT devices could be weaponized at scale, prompting significant regulatory and industry responses on IoT security. [3]
7. By 2025, an estimated 70% of enterprise IoT deployments are projected to incorporate real-time machine learning at the edge. [12]
8. By 2025, 75% of enterprise-generated data is projected to be processed outside centralized cloud data centers, at or near the IoT device. [13]
9. NB-IoT and LoRaWAN sensors can operate on a single battery charge for 10 or more years, enabling deployments in locations where power infrastructure is unavailable or impractical. [15]
10. The 5G RedCap (Reduced Capability) standard reduces 5G module power consumption by approximately 65% compared to full 5G, making cellular IoT practical for wearables and low-power sensors. [14]
11. The Matter standard (2022), supported by Apple, Google, Amazon, and Samsung, addresses longstanding smart home device fragmentation by defining a common application-layer protocol over Thread and Wi-Fi. [6]
12. Satellite IoT networks (Starlink, Iridium, Orbcomm) and eSIM/iSIM provisioning are extending IoT connectivity to maritime, agricultural, and remote industrial environments previously beyond terrestrial network reach. [16]
13. The EU Cyber Resilience Act (2024) and the US IoT Cybersecurity Improvement Act (2020) represent the first generation of mandatory security legislation specifically targeting IoT products. [13]
14. Medical IoT devices such as the Abbott FreeStyle Libre 3 and Dexcom G7 consume below 0.25 mW average power while providing continuous physiological monitoring, demonstrating the degree to which power efficiency has advanced in clinical-grade wearables. [Section 6.3]
15. Ultra-low-power microcontrollers such as the Nordic nRF9161 and STM32U5 achieve sleep-mode currents below 3 µA, enabling multi-year battery-powered operation in cellular-connected sensor nodes. [Section 6.4]

---

## 8. Conclusion

The Internet of Things has evolved from early RFID and M2M experiments into a foundational layer of global technological infrastructure. Its trajectory has been shaped by advances in wireless communication standards, reductions in embedded hardware costs, the maturation of cloud computing platforms, and more recently by the integration of edge artificial intelligence. The diversity of IoT application domains — spanning consumer electronics, industrial automation, healthcare, smart cities, and environmental monitoring — reflects the generality of its core paradigm: connecting the physical world to digital systems at scale.

Current development is characterized by the convergence of AI at the edge, the proliferation of low-power wide-area connectivity, the emergence of unified interoperability standards such as Matter, and increasing regulatory attention to security and power efficiency. The products and protocols surveyed in this document represent the state of the art as of 2024-2025, but the pace of innovation in chipset design, communication standards, and software platforms suggests that the next generation of IoT devices will achieve substantially greater capability, efficiency, and security than those currently available.

---

## 9. References

<a name="ref1"></a>**[1]** Cogniteq. (2023). *The History of Internet of Things (IoT)*. https://www.cogniteq.com/blog/history-iot-how-technology-evolving

<a name="ref2"></a>**[2]** Ashton, K. (2009). "That 'Internet of Things' Thing." *RFID Journal.* https://www.rfidjournal.com/that-internet-of-things-thing

<a name="ref3"></a>**[3]** Wikipedia. (2024). *Internet of Things.* https://en.wikipedia.org/wiki/Internet_of_things

<a name="ref4"></a>**[4]** NRI Digital / Mine Magazine. (2024). *Timeline: Internet of Things.* https://mine.nridigital.com/mine_feb24/timeline-internet-of-things

<a name="ref5"></a>**[5]** International Telecommunication Union (ITU). (2005). *The Internet of Things: ITU Internet Reports 2005.* Geneva: ITU. https://www.itu.int/osg/spu/publications/internetofthings/

<a name="ref6"></a>**[6]** Britannica. (2024). *Internet of Things.* https://www.britannica.com/science/Internet-of-Things

<a name="ref7"></a>**[7]** Atzori, L., Iera, A., & Morabito, G. (2010). "The Internet of Things: A survey." *Computer Networks, 54*(15), 2787-2805. https://doi.org/10.1016/j.comnet.2010.05.010

<a name="ref8"></a>**[8]** Gubbi, J., Buyya, R., Marusic, S., & Palaniswami, M. (2013). "Internet of Things (IoT): A vision, architectural elements, and future directions." *Future Generation Computer Systems, 29*(7), 1645-1660. https://doi.org/10.1016/j.future.2013.01.010

<a name="ref9"></a>**[9]** Zanella, A., Bui, N., Castellani, A., Vangelista, L., & Zorzi, M. (2014). "Internet of Things for Smart Cities." *IEEE Internet of Things Journal, 1*(1), 22-32. https://doi.org/10.1109/JIOT.2014.2306328

<a name="ref10"></a>**[10]** Al-Fuqaha, A., Guizani, M., Mohammadi, M., Aledhari, M., & Ayyash, M. (2015). "Internet of Things: A Survey on Enabling Technologies, Protocols, and Applications." *IEEE Communications Surveys & Tutorials, 17*(4), 2347-2376. https://doi.org/10.1109/COMST.2015.2444095

<a name="ref11"></a>**[11]** Choudhary, G., et al. (2024). "Internet of Things: a comprehensive overview, architectures, applications, and research challenges." *Cluster Computing (Springer Nature).* https://link.springer.com/article/10.1007/s43926-024-00084-3

<a name="ref12"></a>**[12]** Minew. (2025). *Top 7 IoT Trends in 2025: In-Depth Analysis & Predictions.* https://www.minew.com/iot-trends/

<a name="ref13"></a>**[13]** MoldStud. (2024). *Discover the Latest Trends in IoT Development for 2024 and Beyond.* https://moldstud.com/articles/p-discover-the-latest-trends-in-iot-development-for-2024-and-beyond

<a name="ref14"></a>**[14]** Frost & Sullivan. (2024). *IoT Solutions World Congress 2024: Five Key Takeaways.* https://www.frost.com/growth-opportunity-news/information-communications-technology/iot-edge/iot-solutions-world-congress-2024-five-key-takeaways/

<a name="ref15"></a>**[15]** ZedIoT. (2025). *IoT Trends and Prospects in 2025: Comprehensive AI Integration and More.* https://zediot.com/blog/2025-iot-trends/

<a name="ref16"></a>**[16]** G+D (Giesecke+Devrient). (2024). *The future of IoT: 2024 trend overview.* https://www.gi-de.com/en/spotlight/transformation-trends/five-trends-shaping-the-future-of-iot

<a name="ref17"></a>**[17]** IoT Analytics. (2024). *State of IoT: 10 emerging IoT trends driving market growth.* https://iot-analytics.com/state-of-iot-10-emerging-iot-trends-driving-market-growth/

<a name="ref18"></a>**[18]** Simetric. (2024). *The IoT Trends Shaping 2024 and What's Coming in 2025.* https://simetric.com/the-iot-trends-shaping-2024and-whats-coming-in-2025/

<a name="ref19"></a>**[19]** minnovation. (2024). *History of IoT: When IoT Started -- A Historical Overview.* https://minnovation.com.au/iot-platform/history-of-iot-when-iot-started/

<a name="ref20"></a>**[20]** Perez, M., et al. (2021). "The evolution of the Internet of Things (IoT) over the past 20 years." *Computers & Industrial Engineering.* https://www.sciencedirect.com/science/article/pii/S0360835221000784

---

*Disclaimer: We are not affiliated with any company mentioned in this document. This is a general trend research publication compiled from publicly available academic papers, industry reports, and news sources for educational and informational purposes only. All trademarks, product names, and company names are the property of their respective owners.*
