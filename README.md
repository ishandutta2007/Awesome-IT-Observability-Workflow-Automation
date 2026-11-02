# Awesome IT Observability & Workflow Automation [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated directory of top-tier SaaS platforms and open-source software for **IT Observability, Full-Stack Telemetry, AIOps, and Workflow Automation**.

Turn reactive firefighting into proactive, self-healing operations across cloud, on-premises, and hybrid infrastructure.

---

## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS & Enterprise Hosted Platforms](#saas--enterprise-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [Architecture & Tooling Taxonomy](#architecture--tooling-taxonomy)
- [How to Contribute](#how-to-contribute)
- [Disclaimer & License Guidance](#disclaimer--license-guidance)

---

## Sector Overview & Market Dynamics

The global **IT Observability market** is estimated at **$3.08B to $3.5B in 2026** (expanding past **$5.8B to $8B+ by 2030** at ~13–15% CAGR), while the broader **Workflow Automation and Orchestration market** is valued at **$26.0B to $34.1B in 2026** (projected to exceed **$65B–$90B+ by the early 2030s** at ~10–16% CAGR). 

The sector is **moderately fragmented yet increasingly bifurcated**: foundational telemetry collection is rapidly commoditizing around open standards like OpenTelemetry (OTel), while multi-billion-dollar enterprise platforms (such as ServiceNow, CrowdStrike, and Datadog) aggressively drive market concentration at the correlation, AIOps root-cause analysis, and cross-enterprise automated remediation layers.

---

## SaaS & Enterprise Hosted Platforms

The following enterprise platforms provide end-to-end telemetry ingestion, machine learning event correlation (AIOps), infrastructure health monitoring, and automated incident remediation. 

*Sorted in descending order by company scale (market capitalization / valuation).*

| Platform | Company Valuation / Market Size | Starting Tier Pricing | Free Tier / Trial Limits | Key Capabilities & IT Automation Highlights |
| :--- | :--- | :--- | :--- | :--- |
| **[CrowdStrike Falcon for IT](https://www.crowdstrike.com/)** | **~$255B – $275B** (Market Cap) | **$7.99/device/month** (Falcon Go, billed annually ~$29.99–$59.99/device/yr) | **15-day free trial**; full platform access, no credit card required | Endpoint telemetry combined with IT hygiene checks, real-time asset query, and automated remediation workflows. |
| **[ServiceNow ITOM](https://www.servicenow.com/)** | **~$113B – $155B** (Market Cap) | **~$0.50 – $1.50+/monitored node/month** (Enterprise annual contract, packages starting at standard enterprise minimums) | **No self-service free tier**; vendor-guided Proof-of-Concept (PoC) / sales-assisted non-prod evaluation upon request | Service Observability, Health Log Analytics, Metric Intelligence, and Event Management across 12,000+ apps and 5,000+ servers with CMDB integration. |
| **[Datadog](https://www.datadoghq.com/)** | **~$88B – $100B** (Market Cap) | **$15/host/month** (Pro plan, annual billing) or **$0.10/GB** log ingestion | **Permanent Free Tier:** Up to 5 hosts, 1-day metric retention, core dashboards & alerts; **14-day free trial** for Pro/Enterprise features | Unified observability platform with AI log patterns, infrastructure telemetry, APM traces, and low-code workflow automation. |
| **[Splunk IT Service Intelligence](https://www.splunk.com/)** | **$28B** (Acquired by Cisco) | **$60/host/month** or **$0.05–$0.20+/GB/day** (Workload SVC & ingest pricing on top of Splunk Enterprise/Cloud) | **No standalone free tier for ITSI**; core Splunk Enterprise has a **60-day trial** (Splunk Cloud has a **14-day trial**, ITSI enabled via sales PoC) | ITSI 5.0 with AI-powered service and KPI discovery, Event iQ alert noise deduplication, and bi-directional CMDB sync. |
| **[Dynatrace](https://www.dynatrace.com/)** | **~$16.6B – $18.5B** (Market Cap) | **$0.04/hour** (~$28.80/month) for any host size (Infrastructure Monitoring) or **$0.01/hour/GiB memory** (Full-Stack APM) | **15-day free trial** (Full platform access to Davis AI, OneAgent, logs & tracing; no permanent free tier) | Deterministic and causal Davis AI engine for automated root-cause analysis, dynamic topological dependency mapping, and automated remediation. |
| **[ManageEngine OpManager](https://www.manageengine.com/)** | **~$12.5B** (Zoho Corp valuation; $1.4B+ rev) | **$95/year** for 10 devices (Standard Edition) or **$145/year** (Professional Edition) | **Permanent Free Tier:** Up to 3 devices forever; **30-day full-featured free trial** with no credit card required | Network infrastructure monitoring, server tracking, hardware health checks, and built-in workflow automation for mid-market IT teams. |
| **[Tanium](https://www.tanium.com/)** | **~$9B** (Peak valuation; ~$3.7B secondary market) | **~$20 – $24/endpoint/year** (Base platform, typically requires a 2,000-endpoint commercial minimum) | **30-day structured PoC evaluation** via sales or 14-to-30-day partner sandboxes; no self-service free tier | Real-time endpoint discovery and querying at enterprise fleet scale without pre-indexing; rapid scripted remediation execution. |
| **[New Relic](https://newrelic.com/)** | **$6.5B** (Acquired by Francisco Partners & TPG) | **$99/month** (Standard edition base) + **$0.40/GB** for data beyond free allowance + **$49/core user** | **Permanent Free Tier:** 100 GB/month data ingestion free, 1 full-platform user, unlimited basic users, 500 synthetic checks/month | Full-stack observability with NRQL Predictions, predictive anomaly detection, and core IT operations architecture tracking. |
| **[LogicMonitor](https://www.logicmonitor.com/)** | **$2.4B** (Majority owned by Vista Equity Partners) | **$16/hybrid unit/month** (Essentials, billed annually; 1 unit = 1 server/VM or 7 cloud PaaS items) | **15-day free trial** across infrastructure, cloud, and Edwin AI agent features; no permanent free tier | AI-first hybrid observability with Edwin AI agentic noise reduction (80%+ alert noise reduction, up to 67% incident suppression). |
| **[BigPanda](https://www.bigpanda.io/)** | **$1.2B** (Series E valuation) | **~$500/user/month** (Annual commitments starting around ~$6,000/yr, billed via Universal Credits pool) | **No self-service free tier**; vendor-guided Proof-of-Value (POV) with scoped event volumes and integrations | Specialized AIOps event correlation engine; ingests alerts from multi-vendor telemetry tools to deduplicate incidents and automate triage. |

---

## Open-Source GitHub Projects

Curated open-source tooling spanning metric storage, log aggregators, distributed tracing, AIOps correlation engines, and autonomous event-driven workflow automation systems.

*Sorted in descending order by GitHub Stars count.*

| Repository | GitHub Stars | License | Primary Focus | Description & Capabilities |
| :--- | :--- | :--- | :--- | :--- |
| **[n8n](https://github.com/n8n-io/n8n)** | [![GitHub stars](https://img.shields.io/github/stars/n8n-io/n8n?style=social&color=white)](https://github.com/n8n-io/n8n/stargazers) | Sustainable Use | Workflow Automation | Visual node-based workflow automation platform with native AI capabilities, 400+ node integrations, and self-hosting for secure IT remediation. |
| **[dify](https://github.com/langgenius/dify)** | [![GitHub stars](https://img.shields.io/github/stars/langgenius/dify?style=social&color=white)](https://github.com/langgenius/dify/stargazers) | Apache-2.0 | AI Workflow Platform | LLM application and agentic workflow builder featuring visual DAG canvas, RAG pipelines, and API integrations for intelligent IT operations. |
| **[netdata](https://github.com/netdata/netdata)** | [![GitHub stars](https://img.shields.io/github/stars/netdata/netdata?style=social&color=white)](https://github.com/netdata/netdata/stargazers) | GPL-3.0 | Real-Time Monitoring | High-resolution real-time infrastructure observability with per-second metrics, automated dashboard generation, and embedded ML anomaly detection. |
| **[elasticsearch](https://github.com/elastic/elasticsearch)** | [![GitHub stars](https://img.shields.io/github/stars/elastic/elasticsearch?style=social&color=white)](https://github.com/elastic/elasticsearch/stargazers) | AGPL-3.0 / Elastic | Search & Log Storage | Free and open distributed search and analytics engine for high-scale log aggregation, telemetry indexing, and observability pipelines. |
| **[grafana](https://github.com/grafana/grafana)** | [![GitHub stars](https://img.shields.io/github/stars/grafana/grafana?style=social&color=white)](https://github.com/grafana/grafana/stargazers) | AGPL-3.0 | Observability Visualization | The open and composable observability visualization platform for metrics, logs, and traces connecting Prometheus, Loki, OpenTelemetry, and SQL. |
| **[prometheus](https://github.com/prometheus/prometheus)** | [![GitHub stars](https://img.shields.io/github/stars/prometheus/prometheus?style=social&color=white)](https://github.com/prometheus/prometheus/stargazers) | Apache-2.0 | Time Series Metrics | Cloud-native computing foundation (CNCF) graduated time series database and metric scraper powering cloud infrastructure monitoring via PromQL. |
| **[huginn](https://github.com/huginn/huginn)** | [![GitHub stars](https://img.shields.io/github/stars/huginn/huginn?style=social&color=white)](https://github.com/huginn/huginn/stargazers) | MIT | Event-Driven Agents | Open-source agent system that monitors online events, polls APIs and web scrapers, and executes automated conditional tasks on your behalf. |
| **[airflow](https://github.com/apache/airflow)** | [![GitHub stars](https://img.shields.io/github/stars/apache/airflow?style=social&color=white)](https://github.com/apache/airflow/stargazers) | Apache-2.0 | Workflow Orchestration | Programmatic workflow authoring, scheduling, and monitoring framework using Python-defined Directed Acyclic Graphs (DAGs). |
| **[signoz](https://github.com/signoz/signoz)** | [![GitHub stars](https://img.shields.io/github/stars/signoz/signoz?style=social&color=white)](https://github.com/signoz/signoz/stargazers) | Apache-2.0 | All-in-One Observability | Open-source OpenTelemetry-native APM and observability platform combining metrics, traces, and logs with ClickHouse storage and AI agents. |
| **[loki](https://github.com/grafana/loki)** | [![GitHub stars](https://img.shields.io/github/stars/grafana/loki?style=social&color=white)](https://github.com/grafana/loki/stargazers) | AGPL-3.0 | Log Aggregation | Horizontally scalable, highly available log aggregation system inspired by Prometheus that indexes metadata labels instead of full text. |
| **[activepieces](https://github.com/activepieces/activepieces)** | [![GitHub stars](https://img.shields.io/github/stars/activepieces/activepieces?style=social&color=white)](https://github.com/activepieces/activepieces/stargazers) | MIT | Automation & MCPs | Open-source alternative to Zapier/Make featuring 500+ integrations, Model Context Protocol (MCP) servers, and human-in-the-loop workflows. |
| **[jaeger](https://github.com/jaegertracing/jaeger)** | [![GitHub stars](https://img.shields.io/github/stars/jaegertracing/jaeger?style=social&color=white)](https://github.com/jaegertracing/jaeger/stargazers) | Apache-2.0 | Distributed Tracing | CNCF-graduated distributed tracing platform for microservices root cause analysis, latency optimization, and distributed transaction monitoring. |
| **[victoriametrics](https://github.com/victoriametrics/victoriametrics)** | [![GitHub stars](https://img.shields.io/github/stars/victoriametrics/victoriametrics?style=social&color=white)](https://github.com/victoriametrics/victoriametrics/stargazers) | Apache-2.0 | Time Series Database | Ultra-fast, cost-efficient monitoring solution and long-term time series database with low RAM/CPU footprint and full PromQL compatibility. |
| **[argo-workflows](https://github.com/argoproj/argo-workflows)** | [![GitHub stars](https://img.shields.io/github/stars/argoproj/argo-workflows?style=social&color=white)](https://github.com/argoproj/argo-workflows/stargazers) | Apache-2.0 | Cloud-Native Workflows | Container-native workflow engine for orchestrating parallel batch compute and automated jobs on Kubernetes. |
| **[keep](https://github.com/keephq/keep)** | [![GitHub stars](https://img.shields.io/github/stars/keephq/keep?style=social&color=white)](https://github.com/keephq/keep/stargazers) | Apache-2.0 | AIOps & Alert Management | Open-source AIOps and alert correlation engine aggregating alerts across multi-vendor monitoring tools with automated alert deduplication. |
| **[fluent-bit](https://github.com/fluent/fluent-bit)** | [![GitHub stars](https://img.shields.io/github/stars/fluent/fluent-bit?style=social&color=white)](https://github.com/fluent/fluent-bit/stargazers) | Apache-2.0 | Telemetry Shipper | Fast, lightweight log and metrics processor and forwarder for Linux, Windows, BSD, and Kubernetes environments. |
| **[graylog2-server](https://github.com/Graylog2/graylog2-server)** | [![GitHub stars](https://img.shields.io/github/stars/Graylog2/graylog2-server?style=social&color=white)](https://github.com/Graylog2/graylog2-server/stargazers) | SSPL | Centralized Logging | Centralized log management platform with real-time pipeline processing, stream routing, and an Agentic AI framework for alert analysis. |
| **[oneuptime](https://github.com/oneuptime/oneuptime)** | [![GitHub stars](https://img.shields.io/github/stars/oneuptime/oneuptime?style=social&color=white)](https://github.com/oneuptime/oneuptime/stargazers) | Apache-2.0 | SRE & Status Platform | Open-source observability and SRE suite covering status pages, on-call alerts, telemetry monitoring, and incident retrospectives. |
| **[opentelemetry-collector](https://github.com/open-telemetry/opentelemetry-collector)** | [![GitHub stars](https://img.shields.io/github/stars/open-telemetry/opentelemetry-collector?style=social&color=white)](https://github.com/open-telemetry/opentelemetry-collector/stargazers) | Apache-2.0 | Telemetry Pipeline | Vendor-agnostic proxy agent to receive, process, transform, and export telemetry data (metrics, logs, traces) to multiple backends. |
| **[st2](https://github.com/stackstorm/st2)** | [![GitHub stars](https://img.shields.io/github/stars/stackstorm/st2?style=social&color=white)](https://github.com/stackstorm/st2/stargazers) | Apache-2.0 | Event-Driven Auto-Remediation | Event-driven DevOps automation engine ("IFTTT for Ops") with rules engines, ChatOps, and 160+ integration packs for self-healing IT infrastructure. |
| **[zabbix](https://github.com/zabbix/zabbix)** | [![GitHub stars](https://img.shields.io/github/stars/zabbix/zabbix?style=social&color=white)](https://github.com/zabbix/zabbix/stargazers) | AGPL-3.0 | Enterprise Monitoring | Mature open-source real-time monitoring platform for network devices, hypervisors, server hardware, applications, and cloud services. |
| **[alloy](https://github.com/grafana/alloy)** | [![GitHub stars](https://img.shields.io/github/stars/grafana/alloy?style=social&color=white)](https://github.com/grafana/alloy/stargazers) | AGPL-3.0 | OpenTelemetry Collector | Grafana's official OpenTelemetry Collector distribution with programmable pipelines unifying metrics, logs, and traces in a single binary. |

---

## Architecture & Tooling Taxonomy

When architecting a production observability and automated remediation pipeline:

```
[ Infrastructure & Microservices ] 
              │
              ▼ (Logs, Metrics, Traces)
[ Telemetry Ingestion / Collectors ]
  • Open-Source: OpenTelemetry Collector, Fluent Bit, Grafana Alloy
  • SaaS: Datadog Agent, Dynatrace OneAgent, CrowdStrike Falcon Agent
              │
              ▼
[ Storage, Indexing & Dashboards ]
  • Open-Source: Prometheus, Grafana, Loki, SigNoz, VictoriaMetrics, Elasticsearch
  • SaaS: Datadog, New Relic, Splunk Cloud
              │
              ▼ (Alerts & Anomalies)
[ AIOps Correlation & Incident Intelligence ]
  • Open-Source: Keep (deduplication & correlation)
  • SaaS: BigPanda, ServiceNow ITOM, Splunk ITSI, LogicMonitor (Edwin AI)
              │
              ▼ (Automated Actions & Remediation)
[ Workflow Automation & Orchestration Engines ]
  • Open-Source: StackStorm (event auto-remediation), n8n, Activepieces, Argo Workflows, Airflow
  • SaaS: ServiceNow ITOM Workflows, Datadog Workflow Automation
```

---

## How to Contribute

We welcome community contributions! To add a new platform or update an entry:

1. Fork the repository.
2. Edit `README.md` keeping the Markdown table formats consistent.
3. For SaaS platforms: include the official URL, company valuation/market cap, precise starting tier pricing, specific free tier/trial limits, and automation capabilities.
4. For Open-Source repositories: provide the GitHub repository URL, license, capability overview, and shields.io star badge (`?style=social&color=white`) linked to the stargazer page. Maintain descending sort order by GitHub stars.
5. Submit a descriptive Pull Request.

---

## Disclaimer & License Guidance

- **Community-Curated**: This list is independently maintained for educational and architectural evaluation.
- **Data Governance**: Ingesting production telemetry (logs, configuration snapshots, runtime metrics) requires strict compliance with enterprise security, data privacy (GDPR, HIPAA, SOC 2), and data residency standards.
- **Open-Source Trade-Offs**: While open-source telemetry ingestion (OpenTelemetry, Prometheus, Loki) is robust and battle-tested, alert correlation and automated IT change remediation often require glue code or specialized engines (e.g., Keep, StackStorm) compared to all-in-one commercial platforms (ServiceNow, BigPanda).
- **Licensing Verification**: Review software licenses prior to production deployment (e.g., Apache-2.0, MIT, AGPL-3.0, Elastic License, SSPL, or Sustainable Use Licenses).
