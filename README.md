# Awesome-Industrial-IoT-Data-Collection-Modeling

# Top Industrial IoT Data Collection & Modeling Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Industrial Data Acquisition, Asset Modeling & Self-Hosted IIoT Platforms*  
**Last updated: October 2026**

This repository tracks notable **commercial industrial IoT data collection and modeling platforms** and **open-source projects** that acquire sensor data from PLCs, SCADA systems, and industrial equipment, then model assets hierarchically for analytics and digital twins.

**Examples** include AWS IoT SiteWise, PTC ThingWorx, AVEVA Insight, Litmus Edge, Cognite Data Fusion, Rockwell FactoryTalk, GE Digital Predix, Siemens MindSphere, Uptake, and Sight Machine (the category leaders).

**Open-source emphasis**: Industrial IoT data collection is a strong open-source domain. **OpenTwins** leads as a next-gen development framework for composing Digital Twins with 3D visualization, ML models, and real-time data acquisition . **Apache StreamPipes** provides a self-service industrial IoT toolbox enabling non-technical users to connect, analyze, and explore IoT data streams . **Apache PLC4X** delivers a universal protocol adapter for industrial PLCs — unifying Modbus, S7, OPC UA, EtherNet/IP, and more . **ThingSPIN** brings a Digital Twin-as-a-Service platform with semantic models and NGSI-LD compliance . **Eclipse Ditto** provides production-grade digital twin abstraction with 60+ device integration scenarios . **Eclipse Hono** handles large-scale device connectivity across MQTT, AMQP, and CoAP . **Eclipse Kura** delivers edge gateway services including Modbus and OPC-UA . **OpenIoE** supports Unified Namespace and Sparkplug B for MQTT-based industrial data . This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[AWS IoT SiteWise](https://aws.amazon.com/iot-sitewise/)**  
  **AWS's industrial IoT data platform** — collect, organize, and analyze data from industrial equipment at scale . **Asset modeling with hierarchical equipment relationships** — model factories, production lines, and individual machines . **Built-in metrics and transforms** for real-time calculations without coding . **SiteWise Edge** for on-premises data collection and processing . **Best for AWS-native industrial data collection** .

- **[PTC ThingWorx](https://www.ptc.com/en/products/thingworx)**  
  **Industrial IoT platform** — model industrial assets, collect data, and build applications . **ThingWorx Kepware** for industrial connectivity to PLCs and SCADA . **Best for industrial IoT application development** .

- **[AVEVA Insight](https://www.aveva.com/)**  
  **Cloud-based industrial data visualization and analytics** — dashboards for operational data . **Best for process industry monitoring** .

- **[Litmus Edge](https://litmus.io/)**  
  **Industrial edge platform** — collect data from any industrial device and normalize it for cloud analytics . **200+ industrial drivers** with edge computing and store-and-forward . **Best for industrial data collection at the edge** .

- **[Cognite Data Fusion](https://www.cognite.com/)**  
  **Industrial DataOps platform** — contextually enrich industrial data with asset models and relationships . **Best for industrial data contextualization** .

- **[Rockwell FactoryTalk](https://www.rockwellautomation.com/)**  
  **Industrial automation and information platform** — data collection from Rockwell control systems . **Best for Rockwell-centric facilities** .

- **[GE Digital Predix](https://www.ge.com/digital/)**  
  **Industrial IoT platform** — asset performance and predictive maintenance . **Note**: Predix has been largely retired and integrated into other GE Digital products . **Best for GE Digital ecosystem** .

- **[Siemens MindSphere](https://www.siemens.com/)**  
  **Industrial IoT operating system** — connect products, plants, systems, and machines . **Note**: MindSphere has been consolidated into Siemens Insights Hub . **Best for Siemens-centric industrial operations** .

- **[Sight Machine](https://sightmachine.com/)**  
  **Manufacturing analytics platform** — factory data collection and AI-powered insights . **Best for discrete and process manufacturing** .

- **[Uptake](https://www.uptake.com/)**  
  **Industrial AI platform** — asset reliability and predictive maintenance . **Best for heavy industry** .

## Open-Source GitHub Projects

### Digital Twin & Modeling Frameworks

- **[OpenTwins](https://github.com/ertis-research/opentwins)**  
  **Next-generation development framework for composing Digital Twins**, Apache-2.0 licensed . **Toolbox for orchestrating real-time 3D visualization, ML models, and data acquisition from IoT devices** . **Two deployment modes**: Swarm-based production deployment and Docker Compose single-server demo . **Core services**: PostgreSQL with TimescaleDB for time-series, Redis as message broker, K3s for orchestration, 3D visualization dashboard (Three.js), complex event processing (Flink), ML model serving, and DataHub for historical data . **Poseidon component** simplifies 3D digital twin generation with declarative YAML definitions and automatic MQTT/WS data binding to 3D nodes . **OpenTwins Async** decouples HTTP and MQTT for production use . **Best for composable digital twins with 3D visualization and ML** .

- **[ThingSPIN](https://github.com/opensource-spin/thingspin)**  
  **Digital Twin-as-a-Service platform for industrial environments**, open-source . **Semantic-based approach with NGSI-LD compliance** — full support for Smart Data Models and OPC-UA to NGSI-LD conversion . **Event-driven architecture** with RabbitMQ for inter-service communication . **Web dashboards** for managing Digital Twins, visualizing sensor data, and making predictions . **Modular microservices**: DB Manager, Semantic Broker, IoT Adapter, Machine Learning Engine, Server, Worker . **Kafka and RabbitMQ messaging support** for scalable event handling . **Best for semantic Digital Twins with NGSI-LD** .

- **[Eclipse Ditto](https://github.com/eclipse-ditto/ditto)**  
  **Production-grade Digital Twin framework**, EPL-2.0 licensed . **Abstracts physical devices into digital twins with a uniform API** — "digital twin as a service" . **60+ device integration scenarios** including HTTP, MQTT, AMQP, Kafka, and custom connections . **Thing model-based data validation** with JSON schema definitions . **Change notifications** for reactive applications . **Horizontal scaling with MongoDB persistence and cluster-safe search** . **Best for enterprise digital twin abstraction** .

### Industrial Data Collection & Protocol Adapters

- **[Apache PLC4X](https://github.com/apache/plc4x)**  
  **Universal protocol adapter for industrial PLCs**, Apache-2.0 licensed . **Unifies 20+ industrial protocols** — Modbus, S7, OPC UA, EtherNet/IP, BACnet, KNX, CAN, Profinet, and more . **Single API for all PLC types** — "one API to access them all" . **Java, Python, C++, .NET, and Go bindings** . **Reads and writes to PLCs with type-safe access** . **The de facto open-source industrial protocol adapter** . **Best for multi-protocol industrial data collection** .

- **[Apache StreamPipes](https://github.com/apache/streampipes)**  
  **Self-service industrial IoT toolbox**, Apache-2.0 licensed . **Enables non-technical users to connect, analyze, and explore IoT data streams** . **Drag-and-drop pipeline editor** with 100+ data processors and sinks . **Supports Kafka, MQTT, OPC-UA, PLC4X, and more** . **Online machine learning with anomaly detection** . **Best for citizen data scientists in industrial environments** .

- **[Eclipse Hono](https://github.com/eclipse-hono/hono)**  
  **Large-scale device connectivity platform**, EPL-2.0 licensed . **Connects millions of devices to backend systems** via MQTT, AMQP, CoAP, and HTTP . **Protocol adapters normalize device messages** for uniform downstream processing . **Integration with Eclipse Ditto for digital twins** . **Best for massive-scale device connectivity** .

- **[Eclipse Kura](https://github.com/eclipse-kura/kura)**  
  **Edge gateway framework for industrial IoT**, EPL-2.0 licensed . **Provides Modbus, OPC-UA, MQTT, and other industrial protocol support** . **Runs on edge gateways and single-board computers** . **Web UI for gateway configuration and monitoring** . **Best for edge-to-cloud industrial data collection** .

- **[OpenIoE](https://github.com/OpenIoE/openioe)**  
  **Industrial IoT framework supporting Unified Namespace and Sparkplug B**, open-source . **MQTT-based Unified Namespace** with Sparkplug B payload compliance . **Data modeling with asset hierarchies** . **Best for UNS-based industrial data architectures** .

### Time-Series & Data Storage

- **[Apache IoTDB](https://github.com/apache/iotdb)**  
  **IoT-native time-series database**, Apache-2.0 licensed with **5,000+ GitHub stars** . **Optimized for industrial IoT with high-throughput ingestion** . **Built-in caching, stream processing, and data subscription** . **Best for industrial time-series storage** .

- **[TDengine](https://github.com/taosdata/TDengine)**  
  **Purpose-built time-series database for IoT**, AGPL-3.0 licensed with **23,000+ GitHub stars** . **High-performance ingestion and compression** . **Best for IoT and industrial telemetry** .

- **[InfluxDB](https://github.com/influxdata/influxdb)**  
  **The leading open-source time-series database**, MIT licensed with **29,000+ GitHub stars** . **InfluxQL and Flux query languages** . **Built-in downsampling and retention policies** . **Best for industrial observability** .

- **[TimescaleDB](https://github.com/timescale/timescaledb)**  
  **PostgreSQL-based time-series database**, Apache-2.0/Timescale License . **Full SQL with time-series hyperfunctions** . **Best for PostgreSQL users needing industrial time-series** .

### Additional Strong Open-Source Options

- **OpenTwins** — Digital twin framework with 3D visualization and ML .
- **ThingSPIN** — NGSI-LD compliant digital twin platform .
- **Eclipse Ditto** — Production-grade digital twin abstraction .
- **Apache PLC4X** — Universal industrial protocol adapter .
- **Apache StreamPipes** — Self-service industrial IoT toolbox .
- **Eclipse Hono** — Large-scale device connectivity .
- **Eclipse Kura** — Edge gateway framework .
- **OpenIoE** — Unified Namespace and Sparkplug B .
- **Apache IoTDB** — IoT-native time-series database .
- **TDengine** — High-performance time-series database .
- **Node-RED** — Flow-based programming for industrial IoT .
- **OPC UA implementations** — open62541 (C), Milo (Java), asyncua (Python) .
- **Modbus libraries** — pymodbus, libmodbus, ModbusPal .
- **EdgeX Foundry** — Vendor-neutral IoT edge platform .

**Frameworks for building custom industrial IoT data collection and modeling solutions**: Combine **Apache PLC4X** for universal PLC protocol connectivity . Use **Apache StreamPipes** for self-service industrial data pipelines . Deploy **Eclipse Ditto** or **ThingSPIN** for digital twin modeling and asset abstraction . Integrate **OpenTwins** for composable digital twins with 3D visualization and ML . Choose **Eclipse Hono** for massive-scale device connectivity and **Eclipse Kura** for edge gateway services . Use **Apache IoTDB** or **TDengine** for industrial time-series storage . Implement **OpenIoE** for Unified Namespace and Sparkplug B architectures . Note that true enterprise industrial IoT with managed infrastructure, industrial-grade connectors, and vendor-supported SLAs (AWS IoT SiteWise, PTC ThingWorx, Litmus Edge) remains primarily commercial territory; open-source stacks provide strong protocol adapters, digital twin frameworks, and data pipelines that require integration for complete industrial IoT data collection and modeling.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Industrial IoT platforms handle sensitive operational data and may control physical equipment. Self-hosted solutions require proper security hardening, access controls, and compliance with industrial safety standards (IEC 62443).
- **OT networks are increasingly targeted** — industrial IoT deployments must implement network segmentation, zero-trust access, and continuous monitoring . Never expose industrial protocols directly to the internet .
- **OpenTwins deployment**: Swarm-based for production, Docker Compose for single-server demos . **ThingSPIN** requires RabbitMQ and Kafka for event-driven architecture . **Eclipse Ditto** scales with MongoDB and cluster-safe search .
- **Apache PLC4X** unifies 20+ protocols but industrial environments require careful network configuration and device-specific tuning .
- **License considerations**: OpenTwins uses Apache-2.0, ThingSPIN is open-source, Eclipse Ditto uses EPL-2.0, Apache PLC4X uses Apache-2.0, Apache StreamPipes uses Apache-2.0, and Eclipse Hono uses EPL-2.0 . Verify licensing against your use case before committing.
- The open-source ecosystem provides strong protocol adapters, digital twin frameworks, and data pipelines, but **managed infrastructure, industrial-grade connectors, and vendor-supported SLAs** remain primarily commercial offerings.

---

**Made for industrial engineers, IIoT architects, and organizations seeking industrial IoT data sovereignty.**
Let's make industrial IoT data collection and modeling more open, transparent, and interoperable.
