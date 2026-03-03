# IoTs
General Research Trends and Current Status on IoT Facets

---

## Table of Contents
1. [Development History](#development-history)
2. [Key Companies and Products](#key-companies-and-products)
3. [Important Research](#important-research)
4. [Current Trends](#current-trends)
5. [Flagship Products (2024–2025)](#flagship-products-20242025)
6. [References](#references)

---

## Development History

### Origins and Pre-IoT Foundations

The conceptual roots of the Internet of Things stretch back centuries. The **electromagnetic telegraph** (1832) was one of the earliest examples of machine-to-machine (M2M) communication over long distances. By the 1970s, telemetry and SCADA (Supervisory Control and Data Acquisition) systems were enabling remote monitoring in industrial settings.

A pivotal early prototype appeared in the **early 1980s at Carnegie Mellon University**, where researchers connected a Coca-Cola vending machine to the ARPANET (a precursor to the internet), allowing it to report inventory levels and whether drinks were cold — widely regarded as one of the first internet-connected "smart" devices. [¹](#ref1)

### Coining of the Term "Internet of Things" (1999)

The phrase **"Internet of Things"** was coined by **Kevin Ashton** in 1999 while working at **Procter & Gamble**. Ashton used the term to describe a system where physical objects were linked to the internet through sensors and RFID (Radio Frequency Identification) tags, enabling them to communicate without human interaction. He later co-founded the **Auto-ID Center at MIT**, which became a leading research institution for RFID and supply-chain IoT. [²](#ref2) [³](#ref3)

### 2000s – Early Commercial IoT

- **1995:** **Siemens** introduced an early commercial M2M GSM data module (the Siemens M1), one of the first cellular modules designed for machine-to-machine communication and remote equipment monitoring. [⁴](#ref4)
- **2000:** **LG Electronics** announced the first internet-connected refrigerator, featuring an LCD screen and the ability to order groceries online.
- **2003:** **BigBelly Solar** deployed internet-connected solar-powered trash compactors in Boston, capable of reporting fill levels and optimizing collection routes. [⁴](#ref4)
- **2005:** The **United Nations' International Telecommunication Union (ITU)** published a landmark report, *"The Internet of Things,"* formally recognizing it as a technological paradigm shift. [⁵](#ref5)
- **2008:** The **IPSO Alliance** (Internet Protocol for Smart Objects) was formed to promote IP-based networks for smart devices.
- **2008–2009:** The number of internet-connected devices worldwide **exceeded the global human population** for the first time — a milestone highlighted by **Cisco Systems** in their "Internet of Things" white papers. [⁶](#ref6)

### 2010s – Explosion of Connectivity

- **2011:** **Nest Labs** (founded by former Apple engineers Tony Fadell and Matt Rogers) released the **Nest Learning Thermostat**, one of the defining consumer IoT products. It used machine learning to adapt to household schedules. Google acquired Nest in 2014 for $3.2 billion. [⁴](#ref4)
- **2012:** **IPv6** was launched globally, providing a vastly larger address space (approximately 3.4 × 10³⁸ addresses) and becoming critical infrastructure for the IoT's long-term growth. [³](#ref3)
- **2013:** The **AllSeen Alliance** (including Qualcomm, Microsoft, and others) and the **Open Internet Consortium** (Intel, Samsung) were formed to create open IoT standards and interoperability frameworks.
- **2014:** **Amazon** launched the **Echo** smart speaker with the **Alexa** voice assistant, rapidly becoming one of the most successful consumer IoT products in history.
- **2015:** **Apple** launched **HomeKit**, a framework for smart home device control via iOS. **Samsung** acquired SmartThings for $200 million.
- **2016:** The **Mirai botnet** attack exploited insecure IoT devices (cameras, DVRs) to conduct one of the largest DDoS attacks in history, underscoring IoT security as a critical challenge. [³](#ref3)
- **2017–2019:** **NB-IoT** (Narrowband IoT) and **LTE-M** standards were deployed globally by telecom operators, enabling low-power, wide-area connectivity for billions of sensors and meters.

### 2020s – AI, 5G, and the Industrial IoT

- **2020–2022:** The **COVID-19 pandemic** accelerated IoT adoption in healthcare (remote patient monitoring, contact tracing wearables) and logistics (automated warehouses and supply chain tracking).
- **2022:** **Matter**, a unified smart home connectivity standard backed by Apple, Google, Amazon, and Samsung, was released — aiming to solve fragmentation in the consumer IoT space. [⁶](#ref6)
- **2023–2025:** The convergence of **AI and IoT (AIoT)**, rollout of **5G networks**, and proliferation of **edge computing** mark the current era. Industrial IoT (IIoT) is now projected to overtake consumer IoT in market value.

---

## Key Companies and Products

| Company | Key IoT Contribution | Notable Product(s) |
|---|---|---|
| **Amazon** | Consumer IoT & cloud platform | Echo/Alexa, AWS IoT Core |
| **Google / Nest** | Smart home & AI integration | Nest Learning Thermostat, Google Home |
| **Apple** | Consumer ecosystem & standards | Apple Watch, HomeKit |
| **Microsoft** | Enterprise IoT platform | Azure IoT Hub, Azure Digital Twins |
| **Cisco** | IoT networking & security | Cisco IoT Control Center, Catalyst IR routers |
| **Intel** | IoT edge hardware | Intel Atom x6000E series (Elkhart Lake), OpenVINO AI toolkit |
| **Siemens** | Industrial IoT (IIoT) | MindSphere IIoT platform, SIMATIC controllers |
| **GE (General Electric)** | Industrial analytics | Predix IIoT platform |
| **Qualcomm** | IoT chipsets | Snapdragon IoT platforms, QCS6490 |
| **Nordic Semiconductor** | Ultra-low-power wireless chips | nRF52840, nRF9160 (LTE-M/NB-IoT) |
| **Texas Instruments** | Embedded IoT processors | CC2652, SimpleLink MCU family |
| **Bosch** | Sensors & connected mobility | Bosch IoT Suite, MEMS sensors |
| **Samsung** | Smart home & connectivity | SmartThings, Galaxy Watch |
| **Particle Industries** | IoT development platform | Particle Boron (LTE), Tracker One |
| **Raspberry Pi Foundation** | Open-source IoT hardware | Raspberry Pi 5, Raspberry Pi Pico W |

---

## Important Research

### Foundational Academic Works

- **Ashton, K. (2009).** "That 'Internet of Things' Thing." *RFID Journal.* The original essay formalizing the concept of IoT by the person who coined the term. [²](#ref2)

- **Atzori, L., Iera, A., & Morabito, G. (2010).** "The Internet of Things: A survey." *Computer Networks, 54*(15), 2787–2805. One of the most highly cited IoT papers, covering key enabling technologies (RFID, sensors, middleware, applications) and future directions. [⁷](#ref7)

- **Gubbi, J., Buyya, R., Marusic, S., & Palaniswami, M. (2013).** "Internet of Things (IoT): A vision, architectural elements, and future directions." *Future Generation Computer Systems, 29*(7), 1645–1660. Introduces a cloud-centric architectural vision for IoT and defines a reference model still widely cited today. [⁸](#ref8)

- **Zanella, A., Bui, N., Castellani, A., Vangelista, L., & Zorzi, M. (2014).** "Internet of Things for Smart Cities." *IEEE Internet of Things Journal, 1*(1), 22–32. A landmark paper on applying IoT infrastructure to urban environments. [⁹](#ref9)

- **Al-Fuqaha, A., Guizani, M., Mohammadi, M., Aledhari, M., & Ayyash, M. (2015).** "Internet of Things: A Survey on Enabling Technologies, Protocols, and Applications." *IEEE Communications Surveys & Tutorials, 17*(4), 2347–2376. A comprehensive survey covering IoT protocols (MQTT, CoAP, AMQP), enabling technologies, and application domains. [¹⁰](#ref10)

- **Choudhary, G., et al. (2024).** "Internet of Things: a comprehensive overview, architectures, applications, and research challenges." *Cluster Computing (Springer Nature).* A recent meta-review summarizing the state of IoT research across architectures, security, and emerging applications. [¹¹](#ref11)

### Key Industry Reports and Standards Bodies

- **ITU-T Y.2060 (2012):** International Telecommunication Union standard defining the overview and requirements of IoT. [⁵](#ref5)
- **IEEE P2413:** Standard for an Architectural Framework for the Internet of Things.
- **3GPP Release 13 (2016):** Standardized NB-IoT and LTE-M, foundational LPWAN protocols for IoT.
- **Connectivity Standards Alliance (formerly Zigbee Alliance):** Maintains the **Matter** and **Zigbee** standards for smart home interoperability.

---

## Current Trends

### 1. AI and IoT Convergence (AIoT)

Artificial intelligence is being deeply embedded into IoT pipelines — not just in the cloud, but directly on devices (TinyML / edge AI). This enables real-time inference without internet dependency, dramatically reducing latency. By 2025, an estimated **70% of enterprise IoT deployments** are expected to incorporate real-time machine learning. [¹²](#ref12)

**Examples:** AI-powered predictive maintenance sensors in BMW and Siemens factories; edge AI cameras in Barcelona's smart city traffic system for dynamic rerouting.

### 2. Edge Computing Proliferation

Rather than sending all sensor data to the cloud, edge gateways process data near its source. By 2025, **75% of enterprise-generated data** is projected to be processed outside centralized data centers. [¹³](#ref13)

This reduces bandwidth costs, improves response times, and is critical for safety-critical applications (autonomous vehicles, smart grids).

### 3. 5G and 5G RedCap

5G networks (with sub-millisecond latency and up to 10 Gbps throughput) are enabling a new class of industrial and real-time IoT applications. The **5G RedCap (Reduced Capability, 3GPP Release 17)** standard simplifies 5G module design, cutting costs and power consumption by ~65% vs. full 5G — ideal for wearables, smart meters, and industrial sensors. [¹⁴](#ref14)

### 4. Low Power Wide Area Networks (LPWAN)

Protocols designed for battery-operated, low-data-rate sensors covering kilometers:

| Protocol | Range | Power Use | Data Rate | Battery Life |
|---|---|---|---|---|
| **NB-IoT** | 10–35 km (rural) | Ultra-low | 20–250 kbps | 10+ years |
| **LoRaWAN** | 5–15 km (urban) | Ultra-low | 0.3–50 kbps | 10+ years |
| **LTE-M** | Cellular coverage | Low | 1 Mbps | 5–10 years |
| **Bluetooth 5.4 LE** | ~100 m | Very low | Up to 2 Mbps | 1–5 years |
| **Zigbee** | ~100 m (mesh) | Very low | 250 kbps | 2–5 years |

By 2025, LoRaWAN-connected nodes are projected to exceed **2 billion**; Bluetooth Low Energy (LE) devices may reach **26 billion cumulatively**. [¹⁵](#ref15)

### 5. Matter Standard and Smart Home Interoperability

Released in 2022 and backed by Apple, Google, Amazon, and the Connectivity Standards Alliance, the **Matter** standard (built on Thread and Wi-Fi) allows devices from different manufacturers to work seamlessly together. Thread uses IPv6 mesh networking and is designed for ultra-low power operation. This resolves years of fragmentation across competing smart home ecosystems. [⁶](#ref6)

### 6. Non-Terrestrial Networks (NTN) and Satellite IoT

Satellite constellations (SpaceX Starlink, Iridium, Orbcomm) are bringing IoT connectivity to remote areas without terrestrial infrastructure — oceans, deserts, polar regions. eSIM and iSIM technologies allow seamless switching between networks with over-the-air provisioning. [¹⁶](#ref16)

### 7. Security and Zero Trust Architecture

Post-Mirai, IoT security has become a major research and regulatory focus. Current best practices include:
- **AES-256** encryption at rest and in transit
- **Mutual TLS (mTLS)** authentication
- **Secure boot** and firmware attestation
- **Zero Trust Architecture** — no device is inherently trusted on the network
- AI-powered anomaly detection to identify compromised devices

The EU's **Cyber Resilience Act (CRA, 2024)** and the US **IoT Cybersecurity Improvement Act (2020)** are establishing mandatory security baselines for IoT products. [¹³](#ref13)

### 8. Sustainability and Green IoT

IoT device proliferation is a significant and growing contributor to global energy demand — with billions of always-on sensors, gateways, and cloud servers collectively consuming substantial electricity. Designing for efficiency has become both a regulatory and consumer-driven priority. Industry responses include:
- **Energy harvesting** (solar, kinetic, thermal) to power sensors indefinitely
- **Ultra-low-power chipsets** (e.g., Nordic nRF9161, Ambiq Apollo4)
- Duty-cycling and deep sleep modes extending battery life to 10+ years
- Software-defined power management in cloud IoT platforms [¹³](#ref13) [¹⁵](#ref15)

---

## Flagship Products (2024–2025)

### Consumer IoT

| Product | Manufacturer | Key Capability | Power |
|---|---|---|---|
| **Echo Show 15** | Amazon | 15.6" smart display, Alexa AI, visual ID | 30 W |
| **Apple Watch Series 10** | Apple | Health monitoring (ECG, blood oxygen, sleep apnea detection), Siri, LTE | ~1.4 Wh battery, ~18 hr life |
| **Google Nest Learning Thermostat (4th Gen)** | Google/Nest | AI scheduling, Farsight display, Matter/Thread support | ~1.5 W average |
| **Samsung SmartThings Station** | Samsung | Matter/Thread hub, Qi2 wireless charging, connects 200+ device types | 15 W |
| **Arlo Pro 5S 2K** | Arlo | 2K color night vision, AI motion zones, wire-free | Solar or 14,450 mAh battery |
| **Tile Ultra** | Life360 | UWB + Bluetooth precise finding, 400 ft range, 1-year battery | CR2032 coin cell |

### Industrial and Enterprise IoT

| Product | Manufacturer | Key Capability | Power |
|---|---|---|---|
| **Siemens SIMATIC IOT2050** | Siemens | Industrial edge gateway, dual-core ARM, Python/Node-RED | 12–24 V DC, ~15 W |
| **Cisco Catalyst IR1101** | Cisco | Industrial router with LTE/5G, DIN-rail, IOS-XE | -40°C to +60°C, 18 W |
| **Honeywell Experion PKS IoT** | Honeywell | Process control & IIoT integration, AI analytics | Varies (enterprise system) |
| **Bosch Rexroth ctrlX CORE** | Bosch | Real-time Linux industrial controller, OPC-UA, 5G-ready | 24 V DC, 35 W max |
| **PTC ThingWorx 9.x** | PTC | Industrial IoT platform, AR integration, digital twin | Cloud/on-premise |

### Medical and Healthcare IoT

| Product | Manufacturer | Key Capability | Power |
|---|---|---|---|
| **Abbott FreeStyle Libre 3** | Abbott | Continuous glucose monitoring, 14-day wear, phone alerts | Disposable sensor, ~0.24 mW |
| **Philips Biosensor BX100** | Philips | Wearable biometric patch (HR, RR, posture, fall detection) | 7-day disposable patch |
| **Dexcom G7** | Dexcom | Real-time CGM, 10-day wear, direct Apple Watch/Android integration | ~0.15 mW average |

### Development Platforms and Modules

| Product | Manufacturer | Key Capability | Power |
|---|---|---|---|
| **Raspberry Pi 5** | Raspberry Pi Foundation | Quad-core Cortex-A76 @ 2.4 GHz, PCIe 2.0, 8 GB RAM | 5 V / 5 A (25 W max) |
| **Nordic nRF9161 DK** | Nordic Semiconductor | LTE-M/NB-IoT/GNSS SiP, Arm Cortex-M33 | PSM sleep: ~2.5 µA |
| **ESP32-S3** | Espressif | Dual-core Xtensa LX7, Wi-Fi 4, BLE 5.0, AI accelerator | Deep sleep: 7 µA |
| **Particle Boron** | Particle Industries | LTE-M/NB-IoT cellular, cloud OTA, Arduino compatible | Deep sleep: ~0.16 mA |
| **STM32U5** | STMicroelectronics | Ultra-low-power Cortex-M33, TrustZone, AES hardware | Run mode: 19 µA/MHz |

---

## References

<a name="ref1"></a>**[1]** Cogniteq. (2023). *The History of Internet of Things (IoT)*. https://www.cogniteq.com/blog/history-iot-how-technology-evolving

<a name="ref2"></a>**[2]** Ashton, K. (2009). "That 'Internet of Things' Thing." *RFID Journal.* https://www.rfidjournal.com/that-internet-of-things-thing

<a name="ref3"></a>**[3]** Wikipedia. (2024). *Internet of Things.* https://en.wikipedia.org/wiki/Internet_of_things

<a name="ref4"></a>**[4]** NRI Digital / Mine Magazine. (2024). *Timeline: Internet of Things.* https://mine.nridigital.com/mine_feb24/timeline-internet-of-things

<a name="ref5"></a>**[5]** International Telecommunication Union (ITU). (2005). *The Internet of Things: ITU Internet Reports 2005.* Geneva: ITU. https://www.itu.int/osg/spu/publications/internetofthings/

<a name="ref6"></a>**[6]** Britannica. (2024). *Internet of Things.* https://www.britannica.com/science/Internet-of-Things

<a name="ref7"></a>**[7]** Atzori, L., Iera, A., & Morabito, G. (2010). "The Internet of Things: A survey." *Computer Networks, 54*(15), 2787–2805. https://doi.org/10.1016/j.comnet.2010.05.010

<a name="ref8"></a>**[8]** Gubbi, J., Buyya, R., Marusic, S., & Palaniswami, M. (2013). "Internet of Things (IoT): A vision, architectural elements, and future directions." *Future Generation Computer Systems, 29*(7), 1645–1660. https://doi.org/10.1016/j.future.2013.01.010

<a name="ref9"></a>**[9]** Zanella, A., Bui, N., Castellani, A., Vangelista, L., & Zorzi, M. (2014). "Internet of Things for Smart Cities." *IEEE Internet of Things Journal, 1*(1), 22–32. https://doi.org/10.1109/JIOT.2014.2306328

<a name="ref10"></a>**[10]** Al-Fuqaha, A., Guizani, M., Mohammadi, M., Aledhari, M., & Ayyash, M. (2015). "Internet of Things: A Survey on Enabling Technologies, Protocols, and Applications." *IEEE Communications Surveys & Tutorials, 17*(4), 2347–2376. https://doi.org/10.1109/COMST.2015.2444095

<a name="ref11"></a>**[11]** Choudhary, G., et al. (2024). "Internet of Things: a comprehensive overview, architectures, applications, and research challenges." *Cluster Computing (Springer Nature).* https://link.springer.com/article/10.1007/s43926-024-00084-3

<a name="ref12"></a>**[12]** Minew. (2025). *Top 7 IoT Trends in 2025: In-Depth Analysis & Predictions.* https://www.minew.com/iot-trends/

<a name="ref13"></a>**[13]** MoldStud. (2024). *Discover the Latest Trends in IoT Development for 2024 and Beyond.* https://moldstud.com/articles/p-discover-the-latest-trends-in-iot-development-for-2024-and-beyond

<a name="ref14"></a>**[14]** Frost & Sullivan. (2024). *IoT Solutions World Congress 2024: Five Key Takeaways.* https://www.frost.com/growth-opportunity-news/information-communications-technology/iot-edge/iot-solutions-world-congress-2024-five-key-takeaways/

<a name="ref15"></a>**[15]** ZedIoT. (2025). *IoT Trends and Prospects in 2025: Comprehensive AI Integration and More.* https://zediot.com/blog/2025-iot-trends/

<a name="ref16"></a>**[16]** G+D (Giesecke+Devrient). (2024). *The future of IoT: 2024 trend overview.* https://www.gi-de.com/en/spotlight/transformation-trends/five-trends-shaping-the-future-of-iot

<a name="ref17"></a>**[17]** IoT Analytics. (2024). *State of IoT: 10 emerging IoT trends driving market growth.* https://iot-analytics.com/state-of-iot-10-emerging-iot-trends-driving-market-growth/

<a name="ref18"></a>**[18]** Simetric. (2024). *The IoT Trends Shaping 2024—and What's Coming in 2025.* https://simetric.com/the-iot-trends-shaping-2024and-whats-coming-in-2025/

<a name="ref19"></a>**[19]** minnovation. (2024). *History of IoT: When IoT Started – A Historical Overview.* https://minnovation.com.au/iot-platform/history-of-iot-when-iot-started/

<a name="ref20"></a>**[20]** Perez, M., et al. (2021). "The evolution of the Internet of Things (IoT) over the past 20 years." *Computers & Industrial Engineering.* https://www.sciencedirect.com/science/article/pii/S0360835221000784

---

> **Disclaimer:** We are not affiliated with any company mentioned in this document. This is a general trend research publication compiled from publicly available academic papers, industry reports, and news sources for educational and informational purposes only. All trademarks, product names, and company names are the property of their respective owners.
