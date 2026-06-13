# Cyber Threat Exposure Analyzer

## Introduction

The Cyber Threat Exposure Analyzer is a vulnerability intelligence and risk prioritization tool developed in Python. The project integrates vulnerability data from the National Vulnerability Database (NVD) and the Cybersecurity and Infrastructure Security Agency (CISA) Known Exploited Vulnerabilities (KEV) Catalog to support vulnerability assessment and remediation prioritization.

The objective of the project is to identify high-risk vulnerabilities, analyze current threat trends, and generate actionable security insights using publicly available threat intelligence sources.

## Features

* Automated collection of recent CVE records from NVD
* Integration with the CISA KEV Catalog
* CVSS-based vulnerability assessment
* Risk prioritization using severity, exploitability, and recency
* Vendor and product trend analysis
* Threat exposure reporting
* Data export for further analysis

## Data Sources

### NIST National Vulnerability Database (NVD)

The NVD API is used to collect:

* CVE identifiers
* Publication dates
* CVSS scores
* Vulnerability descriptions
* Vendor and product information

### CISA Known Exploited Vulnerabilities Catalog

The KEV Catalog is used to identify vulnerabilities that are known to be actively exploited in real-world environments.

## Methodology

Vulnerabilities are collected from the NVD API and enriched using data from the CISA KEV Catalog.

A risk prioritization model is applied using:

* CVSS severity
* Known exploitation status
* Vulnerability age

The resulting score is used to classify vulnerabilities into remediation priority tiers.

## Analysis Performed

The notebook provides:

* Severity distribution analysis
* Risk score distribution
* Publication trend analysis
* Vendor exposure analysis
* Identification of actively exploited vulnerabilities
* Prioritized remediation recommendations


## Limitations

Vendor attribution depends on metadata available within NVD records. Some vulnerabilities may not contain complete vendor or product information and may therefore be classified as unknown.

Risk scores are intended to support prioritization decisions and should not replace formal organizational risk assessment processes.

## Future Work

* Asset inventory integration
* CVE-to-asset mapping
* Historical trend comparison
* Automated report generation
* Interactive dashboard development

This is a Cybersecurity project focusing on vulnerability intelligence, threat exposure analysis, and risk-based remediation prioritization.
