## Avanade Move Client Data Data Collector

The **Avanade Move Client Data Collector** is Avanade’s standard approach for performing structured data discovery in support of cloud migration planning, readiness assessment, and execution. It provides a consistent, repeatable way to collect server and workload metadata from Windows environments so migration teams can make informed decisions based on evidence rather than assumptions.

This repository hosts the downloadable Data Collector ZIP package used during discovery activities.

## Purpose

The Avanade Move Data Collector is designed to capture a point-in-time view of servers and key workloads before, during, or after migration activities. The collected data helps migration teams understand the current environment, identify readiness concerns, validate workload configuration, and uncover dependencies that may affect migration planning or execution.

The tool supports Avanade’s migration methodology by creating a standardized discovery baseline across servers, applications, and infrastructure components.

## What the Tool Collects

The Data Collector gathers metadata and configuration details across several important discovery areas:

- Windows server inventory and operating system details
- CPU, memory, storage, disk, and volume configuration
- Network adapters, routes, listening ports, firewall status, and proxy settings
- Installed software, Windows roles, features, services, processes, and scheduled tasks
- Patch, reboot, uptime, and event-log indicators
- Hosts file entries and potential hardcoded private IP references
- Windows Server Failover Cluster details where applicable
- SQL Server discovery data when SQL workloads are detected
- IIS discovery data when web workloads are detected

The collector is workload-aware and can perform deeper discovery for SQL Server and IIS when those technologies are present.

## Why It Matters

Discovery is one of the most important steps in a successful migration. Incomplete or inconsistent discovery can lead to missed dependencies, incorrect sizing, migration delays, application issues, or rework.

The Avanade Move Data Collector helps reduce that risk by providing:

- A repeatable discovery process
- Consistent data collection across servers
- Structured outputs for analysis and reporting
- Evidence to support migration readiness decisions
- Visibility into workload configuration and dependencies
- A reusable baseline for pre-migration, test migration, and post-migration comparisons

## Key Benefits

### Standardized Discovery

The tool provides a consistent way to gather server and workload information across an environment, helping teams avoid manual, inconsistent, or incomplete discovery methods.

### Migration Readiness Insight

Collected data can help identify common migration concerns such as pending reboots, low disk space, persistent routes, firewall configuration, proxy settings, patch status, event-log issues, and other readiness indicators.

### Workload Awareness

The collector detects SQL Server and IIS workloads and captures additional metadata relevant to migration planning, validation, and troubleshooting.

### Dependency Visibility

Network, route, port, host file, SQL, IIS, and cluster information can help surface dependencies that may need to be considered during migration design and execution.

### Repeatable Evidence

Because the outputs are structured and generated consistently, they can be used as evidence during assessment, planning, validation, and post-migration review.

## Output

The Data Collector produces structured discovery outputs that can be reviewed by Avanade migration teams and used as input for analysis, reporting, and planning activities.

Typical outputs include:

- Per-server discovery files
- Workload-specific discovery data where applicable
- Collection transcripts
- Success and failure summaries
- Optional scan results depending on selected collection scope

These outputs remain local until shared through the appropriate project-approved process.

## Data Handling

The Data Collector focuses on metadata, configuration, and migration-readiness information. It is not intended to collect application database table contents or business transaction data.

However, discovery outputs may still contain sensitive operational details such as hostnames, IP addresses, file paths, service names, event messages, certificate metadata, SQL metadata, IIS bindings, and other infrastructure context. Outputs should be handled as confidential project data and reviewed before sharing.

## Intended Use

The Avanade Move Data Collector is intended for use by Avanade migration teams, client infrastructure teams, and authorized project stakeholders as part of migration discovery and assessment activities.

It supports:

- Pre-migration assessment
- Migration planning
- Workload validation
- Dependency discovery
- Technical readiness review
- Test migration comparison
- Post-migration validation

## Summary

The **Avanade Move Data Collector** is Avanade’s standardized data discovery package for migration engagements. It provides a repeatable, evidence-based way to collect server and workload information, helping teams understand the current environment, identify risks, validate readiness, and plan migrations with greater confidence.
