# Project-ATLAS
# Atlas — Infrastructure Incident Management Platform

**A monitoring and incident management dashboard for simulating infrastructure disruptions, prioritizing incidents, and tracking resolution performance.**

Atlas is an independent FinTech-inspired project that explores how operations teams can monitor interconnected services, assess incident severity, coordinate resolution, and evaluate system reliability through a centralized dashboard.

Built as a functional prototype using simulated infrastructure data, Atlas combines operational monitoring, incident lifecycle management, service dependency visualization, and reliability analytics.

> **Project Status:** Completed  
> **Project Type:** Product Management · Operations Analytics · FinTech  
> **Data:** Simulated infrastructure and incident data

---

## 1. Problem Statement

Modern financial technology platforms rely on interconnected services, APIs, databases, and data feeds. When a component experiences a disruption, teams need to identify the issue, understand its potential impact, prioritize the response, and coordinate resolution.

Fragmented monitoring information and unclear incident ownership can make these tasks more difficult.

**How might we help infrastructure operations teams understand system health, assess incident impact, and manage resolution through a unified, measurable workflow?**

## 2. Solution

Atlas provides a centralized dashboard for monitoring simulated infrastructure health and managing incidents from detection through resolution.

The platform enables users to:

- Monitor service availability, latency, and error rates.
- Identify and prioritize incidents using severity classifications.
- Explore dependencies between interconnected services.
- Assign ownership and track incident status.
- Review incident history and operational performance metrics.
- Evaluate reliability using simulated incident scenarios.

## 3. Key Features

### System Health Monitoring
- Centralized overview of service health and operational status.
- Monitoring of simulated latency, error rates, and availability.
- Visual identification of services experiencing performance degradation.

### Incident Detection and Prioritization
- Rule-based incident generation from configurable thresholds.
- Severity classification based on predefined conditions.
- Incident queue for reviewing affected services and prioritizing investigation.

### Service Dependency Mapping
- Visualization of relationships between infrastructure components.
- Identification of potentially affected downstream services.
- Support for understanding service dependencies during impact assessment.

### Incident Lifecycle Management
- Incident tracking from detection to resolution.
- Assignment of incident owners and recording of investigation notes.
- Status updates and escalation tracking.
- Historical records of incident activity.

### Operational Analytics
- **Mean Time to Detect (MTTD):** Average time taken to detect an incident.
- **Mean Time to Resolve (MTTR):** Average time taken to resolve an incident.
- **Incident Frequency:** Number of incidents during a selected period.
- **SLA Breach Rate:** Percentage of applicable incidents that exceed defined service targets.
- **Incident Severity Distribution:** Breakdown of incidents by severity.

## 4. Product Management Framework

Atlas was structured around a product-development workflow that translates operational challenges into defined requirements and measurable outcomes.

| Activity | Deliverable |
|---|---|
| Problem discovery | Problem statement and target-user definition |
| User workflow analysis | Incident lifecycle and user flows |
| Requirements definition | Product Requirements Document (PRD) |
| MVP planning | Prioritized features and product backlog |
| Product measurement | Operational KPIs and success criteria |
| Risk management | Risk register and mitigation strategies |
| Validation | Test scenarios and expected outcomes |
| Iteration planning | Product roadmap and future enhancements |

### Target Users
- Infrastructure operations teams
- Site reliability and support engineers
- Technical project and program managers
- Stakeholders responsible for service reliability

## 5. Technology Stack

| Technology | Purpose |
|---|---|
| Python | Application logic and data processing |
| Streamlit | Interactive dashboard interface |
| pandas | Data transformation and analysis |
| Plotly | Interactive charts and operational visualizations |
| CSV | Initial storage for simulated service and incident data |
| PostgreSQL *(optional extension)* | Relational storage for persistent incident records |

## 6. System Workflow

1. **Generate or load data:** Ingest simulated service-health metrics and incident records.
2. **Evaluate system health:** Compare metrics against predefined thresholds.
3. **Detect incidents:** Generate incidents when configured conditions are met.
4. **Prioritize response:** Classify incidents by severity and affected services.
5. **Coordinate resolution:** Track ownership, investigation notes, and status changes.
6. **Evaluate performance:** Calculate operational metrics and analyze incident patterns.

## 7. Success Metrics

Atlas evaluates its prototype using operational metrics derived from simulated incidents.

| Metric | Definition |
|---|---|
| MTTD | Average time between incident onset and detection |
| MTTR | Average time between incident detection and resolution |
| Incident Frequency | Number of incidents during a defined period |
| SLA Breach Rate | Percentage of applicable incidents that breach defined targets |
| Prioritization Accuracy | Percentage of test incidents assigned the expected severity |

These metrics provide a framework for assessing prototype behavior. They do not establish improvements in real-world infrastructure reliability.

## 8. Testing and Validation

The prototype can be evaluated using controlled scenarios covering:

- Normal service operation.
- Latency or error-rate threshold breaches.
- Multiple incidents occurring simultaneously.
- High-severity incidents affecting dependent services.
- Incident assignment and status transitions.
- Resolution-time calculations and SLA threshold checks.
- Missing, invalid, or incomplete input data.

Validation should confirm that the dashboard reflects the input data accurately, applies prioritization rules consistently, and calculates operational metrics correctly.

## 9. Project Roadmap

The completed project scope is organized into the following development stages:

- **Stage 1 — Product Definition:** Define the problem, target users, requirements, and MVP scope.
- **Stage 2 — Monitoring Dashboard:** Build service-health views and operational summaries.
- **Stage 3 — Incident Management:** Implement incident generation, prioritization, and lifecycle tracking.
- **Stage 4 — Dependency Visualization:** Map relationships between services and support impact assessment.
- **Stage 5 — Operational Analytics:** Calculate reliability metrics and visualize incident trends.
- **Stage 6 — Validation:** Evaluate functionality using simulated incident scenarios and document limitations.

## 10. Future Enhancements

Potential extensions include:

- Anomaly detection using historical service metrics.
- Dependency-aware incident impact scoring.
- AI-assisted incident summaries grounded in recorded incident data.
- Root-cause investigation support.
- Notifications and integrations with issue-tracking platforms.
- PostgreSQL-backed persistence and historical analysis.
- Role-based access controls and audit logs.

These enhancements are future opportunities and are not part of the completed scope unless explicitly implemented.

## 11. Limitations

Atlas is an educational prototype based on simulated infrastructure and incident data. It is not connected to live exchange systems, does not monitor Nasdaq infrastructure, and is not intended for production incident response.

Incident detection, severity classification, and operational metrics depend on the configured rules and the quality of the simulated data.

## 12. Running the Project

After cloning the repository, install the required dependencies and launch the Streamlit application.

```bash
git clone <your-repository-url>
cd atlas
python -m venv .venv
```

Activate the virtual environment:

**macOS / Linux**
```bash
source .venv/bin/activate
```

**Windows**
```bash
.venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch the application:

```bash
streamlit run app.py
```

The commands assume the repository contains `requirements.txt` and `app.py` at its root. Adjust the entry point and installation instructions to match the actual repository structure.


*Atlas is an independent educational project exploring infrastructure monitoring, incident coordination, operational analytics, and structured product delivery in a financial technology context.*
