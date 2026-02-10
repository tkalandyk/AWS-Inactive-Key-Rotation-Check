# AWS Inactive Access Key Risk Classification & Compliance Evidence Generator

## Overview

This project is an automated **GRC engineering security tool** that identifies, classifies, and reports on risky AWS IAM access keys across an AWS environment.

Instead of manually reviewing credentials in the AWS console or relying on expensive SaaS compliance platforms, this tool programmatically analyzes access key lifecycle data using Python and AWS APIs to generate **audit-ready evidence** and **actionable security intelligence**.

This demonstrates how compliance can move from manual checklists to **automated, risk-driven security engineering**.

---

## The Problem

Inactive or stale AWS access keys are one of the most common cloud security risks.  
Old credentials that remain active can become permanent backdoors if leaked or forgotten.

Most organizations currently rely on:

### Manual Reviews
- Time consuming  
- Not scalable  
- No historical evidence trail  
- High human error rate  

### Enterprise Compliance SaaS Tools
- Expensive recurring cost  
- Vendor lock-in  
- Limited customization of risk logic  
- Often function as black boxes  

---

## The Solution

This tool provides a **cost-effective automation layer** that:

- Scans all IAM users and access keys  
- Evaluates key age and last usage data  
- Applies configurable risk classification logic  
- Generates timestamped compliance evidence  
- Produces remediation recommendations  

---

## Key Capabilities

### Risk Classification Engine
Classifies keys into categories such as:

- Critical  
- High  
- Medium  
- Low  
- Compliant  
- Never Used  

Thresholds are configurable to align with internal security policy.

---

### Evidence Generation

Produces:

- JSON structured analysis output (automation / pipeline ready)  
- CSV audit summary reports (auditor friendly)  

Evidence includes:

- Account ID  
- Assessment timestamp  
- Username  
- Access Key ID  
- Risk classification  
- Key age  
- Last used data  
- Recommended action  

---

## Compliance Mapping

This project directly supports:

### SOC 2
- CC6.1 — Logical access security controls  

### NIST 800-53
- IA-4 — Identifier Management  

---

## Business Value

### Risk Reduction
- Identifies unused credentials before attackers can exploit them  
- Reduces attack surface automatically  
- Moves security from reactive to preventative  

### Cost Efficiency
- No SaaS licensing required  
- Runs using standard Python + boto3  

### Audit Confidence
- Generates timestamped, repeatable evidence  
- Eliminates spreadsheet-driven compliance  
- Provides proof of control operation, not just policy existence  

---

## How It Works (High Level)

1. Authenticates using AWS CLI profile credentials  
2. Enumerates IAM users and access keys  
3. Pulls lifecycle and last-used metadata  
4. Applies configurable risk logic  
5. Generates compliance evidence reports  

---

## Technology Stack

- Python  
- boto3  
- AWS IAM APIs  
- AWS CLI Profile Authentication  

---

## Deployment Flexibility

Currently runs locally for testing against a real AWS test environment.

Can be adapted for:

- AWS Lambda scheduled scans  
- CI/CD security gates  
- Security monitoring pipelines  
- ChatOps / alerting integrations  

---

## Example Output

Generated Evidence Files:

inactive_key_analysis_report.json

<img width="606" height="796" alt="image" src="https://github.com/user-attachments/assets/ed97c4f9-5e0e-4fca-b0d0-24a4a812060f" />


inactive_key_summary.csv

<img width="606" height="796" alt="image" src="https://github.com/user-attachments/assets/349e4340-9203-492a-916a-537775e0a636" />

Assessment Output Includes:

- Total Users Scanned  
- Total Keys Analyzed  
- Risk Distribution  
- Compliance Status  
- SOC 2 Status  
- NIST Status  

---

## Why This Matters (Beyond Passing Audits)

Audit readiness is a byproduct — not the goal.

The real goal is:

- Prevent credential abuse  
- Reduce persistent access risk  
- Enforce key lifecycle hygiene at scale  

This demonstrates the difference between:

**Compliance Theater → Security Engineering**

---

## Portfolio & Interview Value

This project demonstrates ability to:

- Translate compliance requirements into working automation  
- Build evidence-producing security controls  
- Reduce manual GRC workload using engineering  
- Align security automation with real business risk  

---

## Future Direction

This project is part of a broader evolution:

**GRC → Security Automation → AI-Assisted Risk Detection → Autonomous Security Operations**

Potential expansion:

- Org-wide multi-account scanning  
- Automated ticket generation  
- Predictive key risk scoring  
- AI-assisted anomaly detection  

---

## Summary

This tool proves the ability to:

- Engineer compliance controls  
- Automate risk detection  
- Produce audit-grade evidence  
- Improve real security posture — not just documentation  

Scales from small environments to enterprise cloud estates.
