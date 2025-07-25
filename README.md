# AURA – Cloud-Native Logging Platform

AURA is a cloud-native logging platform designed for distributed microservices running on Oracle Cloud Infrastructure (OCI). The project focuses on scalable log ingestion, event-driven ETL processing, and real-time analytics to give developers and operators actionable insights.

> **Status:** Currently in the design and prototyping phase.

## Features

### Planned Capabilities

- **Asynchronous Log Ingestion**  
  Receive high-throughput JSON logs from microservices via OCI API Gateway and OCI Functions.

- **Event-Driven ETL**  
  Automatically parse and transform raw logs stored in OCI Object Storage into structured data in Oracle Autonomous Database.

- **Real-Time Analytics Dashboard**  
  Interactive dashboard in Oracle APEX for log visualization, faceted search, and system performance monitoring.

- **Cloud-Native Scalability**  
  Designed to scale horizontally across services with minimal operational overhead.

## Architecture (Planned)

```
Microservices → OCI API Gateway → OCI Functions → Object Storage → Autonomous DB → Oracle APEX
```

- **Log Ingestion:** API Gateway + Functions handle incoming logs asynchronously.
- **Storage & ETL:** Object Storage triggers ETL pipelines for transformation.
- **Visualization:** APEX dashboard consumes structured data for insights.

## Tech Stack

- **Languages:** Python, PL/SQL
- **Cloud Services:** OCI API Gateway, OCI Functions, Object Storage, Autonomous DB
- **Frontend/Visualization:** Oracle APEX
- **Workflow:** Event-driven architecture leveraging OCI native integrations

## Status & Roadmap

- **Phase 1 (Current):** Architecture design and PoC for log ingestion pipeline
- **Phase 2 (Planned):** Implement ETL and initial dashboard for basic metrics
- **Phase 3 (Future):** Full faceted search, alerting, and advanced visualizations

## Contribution

Contributions are welcome as the architecture evolves. Please fork the repository, open an issue, or submit a pull request for proposals and enhancements.

## License

This project is licensed under the MIT License.
