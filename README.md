# Awesome-IT-Observability-Workflow-Automation

## Top IT Observability & Workflow Automation Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Unified Telemetry, AIOps & Self-Hosted Automation Engines*  

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **IT Observability & Workflow Automation**. These tools enable organizations to collect metrics, logs, and traces from infrastructure and applications, correlate signals to detect anomalies, and trigger automated remediation—turning reactive firefighting into proactive, self-healing operations.



**Examples** include CrowdStrike Falcon for IT, Tanium, Datadog, Dynatrace, New Relic, ServiceNow ITOM, Splunk IT Service Intelligence, BigPanda, LogicMonitor, and ManageEngine OpManager (the category leaders).



**Open-source emphasis**: IT Observability & Workflow Automation is a domain where open-source tooling is **genuinely mature at the telemetry and monitoring layers, but fragmented for AIOps correlation and remediation orchestration**. The **Prometheus + Grafana + Loki** stack remains the foundational open-source observability trio, while **Keep** provides an open-source alert management and AIOps platform that aggregates alerts, deduplicates events, and provides workflow automation . **n8n** and **Activepieces** handle workflow automation but are general-purpose tools rather than IT-ops-specific remediation engines . The critical caveat: **no open-source project matches the unified AIOps correlation** of BigPanda or the IT-specific workflow orchestration of ServiceNow ITOM—those platforms correlate alerts across domains and trigger remediation with enterprise-grade change control .



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[CrowdStrike Falcon for IT](https://www.crowdstrike.com/)**  

  IT observability and workflow automation within the Falcon platform; combines endpoint telemetry with IT hygiene checks and automated remediation workflows.



- **[Tanium](https://www.tanium.com/)**  

  Real-time endpoint visibility and interrogation without pre-ingestion; Tanium's advantage is finding what you're hunting for faster across any fleet size, with integrated remediation actions.



- **[Datadog](https://www.datadoghq.com/)**  

  Unified observability platform with AI-powered log management, infrastructure monitoring, APM, and workflow automation; Log Patterns auto-group similar messages and Pattern Inspector reveals underlying data .



- **[Dynatrace](https://www.dynatrace.com/)**  

  AI-powered observability with Davis AI for deterministic and agentic root cause analysis; automatic discovery, baselining, and remediation recommendations.



- **[New Relic](https://newrelic.com/)**  

  Observability platform with predictive alerting and NRQL Predictions for proactive anomaly detection; moved Service Architecture Intelligence and predictive features into Core Observability as of June 2026 .



- **[ServiceNow ITOM](https://www.servicenow.com/)**  

  IT Operations Management suite with Service Observability, Health Log Analytics, Metric Intelligence, and Event Management; streams real-time signals from 12,000+ apps and 5,000+ servers into a unified dashboard for predictive insight and root cause analysis .



- **[Splunk IT Service Intelligence](https://www.splunk.com/)**  

  ITSI 5.0 released June 2026 with AI-powered service and KPI discovery, Event iQ Detect and Diagnose for alert noise reduction, and CMDB enrichment from ServiceNow and Jira .



- **[BigPanda](https://www.bigpanda.io/)**  

  AIOps platform for event correlation and incident intelligence; aggregates alerts across monitoring tools and reduces noise through machine learning correlation.



- **[LogicMonitor](https://www.logicmonitor.com/)**  

  AI-first hybrid observability platform with Edwin AI agents; customers report 80%+ noise reduction and up to 67% fewer incidents; maps technology performance to business services across on-premises, cloud, and edge .



- **[ManageEngine OpManager](https://www.manageengine.com/)**  

  Network and infrastructure monitoring with workflow automation; positioned for mid-market IT teams.



## Open-Source GitHub Projects



### Observability Foundations (Prometheus, Grafana, Loki)



- **[Prometheus](https://github.com/prometheus/prometheus)**  

  The **de facto open-source metrics monitoring system and time series database** (Apache 2.0); pull-based collection with PromQL query language. The foundational layer for cloud-native observability .



- **[Grafana](https://github.com/grafana/grafana)**  

  Open-source **visualization and dashboarding platform** (AGPL-3.0); connects to Prometheus, Loki, Elasticsearch, and dozens of other data sources for unified observability dashboards .



- **[Loki](https://github.com/grafana/loki)**  

  Open-source **log aggregation system** designed for cost efficiency (AGPL-3.0); label-based indexing makes it cheaper to operate than full-text indexed alternatives, with native OpenTelemetry support .



- **[Grafana Alloy](https://github.com/grafana/alloy)**  

  Grafana's **OpenTelemetry Collector distribution** that unifies logs, metrics, and traces in a single agent; the supported successor to Promtail and Grafana Agent .



### AIOps & Alert Management (Keep)



- **[Keep](https://github.com/keephq/keep)**  

  The **leading open-source alert management and AIOps platform** (Apache 2.0) . Aggregates alerts from multiple monitoring tools, deduplicates and correlates events, and provides a unified interface for incident response with workflow automation and AI-powered enrichment . **Best for teams wanting to reduce alert noise** before paging—but it is an alert correlation layer, not a full workflow automation engine.



### Workflow Automation (n8n, Activepieces, Dify)



- **[n8n](https://github.com/n8n-io/n8n)**  

  Mature open-source **node-based workflow automation tool** (Sustainable Use License); 400+ integrations, visual canvas with drag-and-drop nodes, logic branching, and self-hosting for data privacy .



- **[Activepieces](https://github.com/activepieces/activepieces)**  

  MIT-licensed **workflow automation alternative to Zapier and Make**; 500+ integrations, AI Agents and Copilot, human-in-the-loop steps, and a full REST API .



- **[Dify](https://github.com/langgenius/dify)**  

  Open-source **LLM application development platform** with visual drag-and-drop workflow builder, RAG pipeline, and knowledge base; 58,000+ GitHub stars . **Best for AI-augmented automation**—but it is LLM-focused rather than IT-ops-specific.



### Additional Strong Open-Source Options



- **OneUptime** — Complete open-source **observability platform** including incident management, on-call rotations, log analysis, and performance tracking . **Best for teams wanting an all-in-one observability + incident stack**—but it is a substantial platform requiring deployment.

- **Graylog** — Open-source log management platform with stream routing and Graylog 7.2's Agentic Framework for AI-assisted operations . **Best for log-centric observability** with a built-in UI.

- **Netdata** — Real-time infrastructure monitoring with per-second resolution and ML-based anomaly detection; 800+ integrations with automatic dashboard generation .



**Frameworks for building custom systems**: For **metrics monitoring and dashboards**, Prometheus + Grafana is the foundational stack . For **log aggregation**, Loki or Graylog . For **alert correlation and AIOps**, Keep . For **workflow automation**, n8n or Activepieces . **No open-source project matches the unified AIOps correlation** of BigPanda or the IT-specific workflow orchestration of ServiceNow ITOM—those are enterprise platforms that correlate signals across domains and enforce change control at scale.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- IT observability and workflow automation platforms handling production telemetry must comply with organizational security policies and data governance requirements; **self-hosted solutions place full responsibility for storage sizing, alert tuning, and uptime on the operator**.

- **Open-source observability is mature at the telemetry layer but fragmented for AIOps and IT-specific automation**—Prometheus and Grafana provide production-grade monitoring , and Keep provides alert correlation . However, **no open-source project matches the unified AIOps correlation** of BigPanda or the IT workflow orchestration of ServiceNow ITOM. Choose based on whether you need foundational telemetry (Prometheus/Grafana), alert noise reduction (Keep), or general workflow automation (n8n/Activepieces).

- Verify license terms for commercial use; Prometheus uses Apache 2.0, Grafana and Loki use AGPL-3.0, and n8n uses the Sustainable Use License (not OSI-approved) .



---



**Made for SREs, IT operations teams, and organizations building observability and automation infrastructure.**  

Let's make IT observability and workflow automation more open, but with clear eyes about the AIOps correlation and enterprise IT orchestration gaps that commercial platforms still fill.
