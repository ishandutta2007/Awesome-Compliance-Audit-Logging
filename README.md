# Awesome-Compliance-Audit-Logging

# Top Compliance & Audit Logging Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Immutable Audit Trails, SIEM Correlation & Regulatory Compliance Reporting*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Compliance & Audit Logging**. These tools help organizations capture, retain, and analyze system and user activity logs to satisfy regulatory requirements (SOX, HIPAA, GDPR, PCI DSS), support forensic investigations, and detect anomalous behavior across cloud and on-premises environments.

**Examples** include Datadog Cloud SIEM, Splunk Cloud, Sumo Logic, Panther, Elastic Security, LogRhythm, Papertrail, Graylog, AuditBoard, and Zoho Audit Trail (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted log management, open-source SIEM, and community-driven audit logging—ideal for security teams, compliance officers, and organizations seeking transparent, vendor-neutral log retention without per-GB ingest pricing surprises.

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[Datadog Cloud SIEM](https://www.datadoghq.com/)** | Cloud-native SIEM layered on Datadog's log management. Bills per **million analyzed events** rather than per GB ingested—detection rules, signals, and threat intelligence included. Extends security signal retention to 15 months at no additional cost (Oct 2026) . | **$5 per million analyzed events/month** (annual billing); $6 month-to-month; $7.50 on-demand. Log ingestion/retention billed separately . | **No free tier** per PricingSaaS tracking . Paid plans only; trial via Datadog sales. |
| **[Splunk Cloud](https://www.splunk.com/)** | Enterprise SIEM and log analytics platform. Ingest-based pricing with tiered volume options. No free tier; free trial limited to **5 GB/day for 15 days** with no data export and no REST API access . | **$675/month** (5 GB/day, annual); **$8,100/month** (5 GB/day billed annually per CostBench); **$2,000/month** (20 GB/day) . | **No free tier**; **15-day trial**: 5 GB/day ingest, US East region only, no data export, no SSO, no premium apps, 10 concurrent searches max . |
| **[Sumo Logic](https://www.sumologic.com/)** | Cloud SIEM with two licensing models: Credits (ingest-based) and Flex (scan-based, $0 ingest for standard logs). Cloud SIEM ingest billed separately at **40 credits/GB**—the most expensive data type on the platform . | Credit model: $0.25/credit (Enterprise Suite); Flex model: ~$1.50/credit (Enterprise Suite Flex) . | **Free (Flex)**: 1.25 credits/day, 7-day log retention, 3 users . **Trial**: ~1 GB/day ingest (~500 GB search/day), 30-day retention, 20 users, 30 days . |
| **[Panther](https://panther.com/)** | Cloud-scale security analytics platform with detection-as-code. Consumption-based pricing per TB ingested; no per-seat charges for analysts. Typical annual contracts: **$50,000–$150,000** for 5–20 TB/month deployments . | **$3,000–$6,000 per TB/month** (before negotiation); contract minimums typically $50K–$100K/year . | **No free trial** available per SaaSworthy; free-forever and custom plans listed . |
| **[Elastic Security](https://www.elastic.co/)** | SIEM built on Elasticsearch with endpoint protection. Serverless pricing: **Security Analytics Essentials** at $0.09/GB ingest with 50 GB free, then $0.05/GB transfer; **Complete** at $0.11/GB . | Essentials: **$0.09/GB ingest** (50 GB free); Complete: **$0.11/GB** . | **50 GB free ingest** on Essentials tier; no time-limited trial mentioned for serverless . |
| **[LogRhythm](https://www.logrhythm.com/)** | Enterprise SIEM with per-message licensing. Positioned as expensive for smaller organizations but competitive for Windows-heavy environments compared to volume-based pricing . | Quote-only (per-message licensing) | No public free tier; trial via sales. Capterra placeholder shows $0.01 one-time (unverified) . |
| **[Papertrail (SolarWinds)](https://www.papertrail.com/)** | Cloud-hosted log management for troubleshooting. Simple pricing based on log volume and retention duration; all functionality available on all plans . | **$7.00/month** starting price | **Free plan available**: 50 MB log storage, 1-day searchable retention, 1-year downloadable archives . |
| **[Graylog](https://graylog.org/)** | Log management and SIEM platform. **Graylog Open** (free) includes 16 GB storage and single-node deployment; Security and Enterprise editions add clustering, long-term analysis, and advanced features . | Quote-only for Security/Enterprise; **Graylog Open free** . | **Free (Graylog Open)**: 16 GB storage, single node, full-fidelity log capture, threat detection, API discovery . |
| **[AuditBoard](https://www.auditboard.com/)** | Connected risk platform for SOX compliance, internal audit, and IT risk. Vendr benchmarks: small teams (5–15 users) at lower range; mid-sized (15–50 users, multiple solutions) bundled pricing; enterprise custom . | Quote-only; implementation typically **10–25% of annual subscription**; renewal escalations 3–7%/year . | **No free trial** per Software Advice listing; demo via sales. |
| **[Zoho Audit Trail](https://www.zoho.com/)** | Audit logging within Zoho applications. **Zoho Creator**: free plan retains change audit data for **3 months**; paid plans retain for **3 years**. **Zoho Commerce**: activity logs track create/update/delete with PII field filtering and export . | Included with Zoho application subscriptions | **Free (Creator)**: audit trail available with 3-month change audit retention; paid plans extend to 3 years . |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Graylog Open](https://github.com/Graylog2/graylog2-server)** | [![Stars](https://img.shields.io/github/stars/Graylog2/graylog2-server?style=social&color=white)](https://github.com/Graylog2/graylog2-server/stargazers) | Free and open log management platform (SSPL). Full-fidelity log capture, threat detection, API discovery, and guided remediation within 16 GB storage on a single node. The most mature self-hosted alternative to Splunk/Datadog for audit logging . |
| **[Tailpipe](https://github.com/turbot/tailpipe)** | [![Stars](https://img.shields.io/github/stars/turbot/tailpipe?style=social&color=white)](https://github.com/turbot/tailpipe/stargazers) | Open-source SIEM for instant log insights powered by DuckDB. Query millions of events in seconds from the terminal using SQL. No database required. Plugins for AWS CloudTrail, Azure Activity Logs, GCP Audit Logs, GitHub audit logs, nginx, Apache, and more . |
| **[pgMemento](https://github.com/pgMemento/pgMemento)** | [![Stars](https://img.shields.io/github/stars/pgMemento/pgMemento?style=social&color=white)](https://github.com/pgMemento/pgMemento/stargazers) | Audit trail with schema versioning for PostgreSQL using transaction-based logging. Tracks all data changes with full history and audit capabilities for compliance. |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[boxyhq/hermes](https://github.com/boxyhq/hermes)** | [![Stars](https://img.shields.io/github/stars/boxyhq/hermes?style=social&color=white)](https://github.com/boxyhq/hermes/stargazers) | Audit logs service from BoxyHQ. Designed for enterprise SaaS applications requiring compliance-grade audit trails. |
| **[auditdb](https://github.com/auditdb/auditdb)** | [![Stars](https://img.shields.io/github/stars/auditdb/auditdb?style=social&color=white)](https://github.com/auditdb/auditdb/stargazers) | Simple, efficient database record auditing. Lightweight library for tracking data changes in applications. |
| **[doctrine-audit-bundle](https://github.com/DamienHarper/doctrine-audit-bundle)** | [![Stars](https://img.shields.io/github/stars/DamienHarper/doctrine-audit-bundle?style=social&color=white)](https://github.com/DamienHarper/doctrine-audit-bundle/stargazers) | Symfony bundle for auditing Doctrine ORM entities. Tracks changes with configurable audit policies. |

**Frameworks for building custom systems**: Combine **Graylog Open** for centralized log ingestion and search, **Tailpipe** for SQL-based investigation of cloud audit logs, **pgMemento** for database-level change auditing, and **Hermes** for application audit trails—creating a fully self-hosted compliance logging stack without per-GB ingest fees.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Compliance audit logging platforms handle sensitive system activity and potentially PII; enforce encryption at rest and in transit, role-based access to audit data, and tamper-evident storage for regulatory defensibility.
- Pricing models vary dramatically: Datadog bills per analyzed event, Sumo Logic charges 40 credits/GB for Cloud SIEM ingest, and Splunk has no free tier. Enterprise platforms (Panther, AuditBoard, LogRhythm) are quote-only with implementation costs adding 10–25% to first-year totals . Open-source alternatives like Graylog Open require infrastructure and operational expertise but eliminate per-GB ingest costs.

---

**Made for compliance officers, security engineers, SOC analysts, and organizations building audit-ready infrastructure.**  
Let's make compliance audit logging more open, tamper-evident, and cost-predictable.
