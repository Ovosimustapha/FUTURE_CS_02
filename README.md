# FUTURE_CS_02
# Phishing Detection & Awareness Report Analysis

## Overview

This project documents the analysis of a phishing email impersonating **Lowe's Companies, Inc.** The investigation focused on identifying technical and behavioral indicators of phishing through email header analysis, sender verification, authentication checks, and malicious link inspection.

The objective of this report is to demonstrate practical phishing detection techniques, threat classification, and user awareness recommendations commonly used by cybersecurity analysts and SOC teams.

---

## Case Summary

**Threat Type:** Phishing Email (Brand Impersonation)

**Impersonated Organization:** Lowe's Companies, Inc.

**Risk Level:** Critical

**Classification:** Confirmed Malicious

**Primary Threat Objective:**

* Credential Harvesting
* Identity Theft
* Malware Delivery
* User Tracking

---

## Tools Used

### MXToolbox

MXToolbox was used to perform email security and header analysis, including:

* Email Header Analysis
* SPF Validation Checks
* DKIM Verification
* DMARC Verification
* Mail Routing Investigation
* IP Reputation Review
* Sender Authentication Assessment

Tool Website:

https://mxtoolbox.com

---

## Analysis Approach

The phishing email was analyzed using a structured methodology commonly applied during email threat investigations.

### 1. Email Artifact Collection

The phishing email sample was collected and preserved for analysis.

Collected artifacts included:

* Email screenshot
* Raw email headers
* Embedded URLs
* HTML source code

---

### 2. Email Header Analysis

The raw email header was examined to identify:

* Sender infrastructure
* Message routing path
* Authentication failures
* Suspicious originating IP addresses

Key findings included:

* SPF Failure
* DKIM Missing
* DMARC Failure
* Suspicious Return-Path Domain
* High Spam Confidence Level (SCL)

---

### 3. Sender Domain Verification

The sender's display name and actual email address were compared.

Observed:

Display Name:
Lowes

Actual Sender Address:
[4uh0k@7rye9ue08e.com](mailto:4uh0k@7rye9ue08e.com)

Result:

The sending domain had no legitimate association with the official Lowe's domain, indicating domain impersonation and sender deception.

---

### 4. Link Inspection

Embedded hyperlinks were reviewed to determine whether they redirected users to trusted destinations.

Indicators identified:

* URL Shortening Services
* Obfuscated Redirect Chains
* Unrelated Destination Domains
* Potential Credential Harvesting Infrastructure

---

### 5. HTML Source Code Review

The email source code was inspected for hidden malicious components.

Findings:

* Redirect URLs
* Tracking Pixel
* Hidden External Resources
* User Activity Monitoring Mechanisms

---

### 6. Social Engineering Analysis

The email content was reviewed for psychological manipulation techniques.

Techniques observed:

* Artificial Urgency
* Fear of Missing Out (FOMO)
* High-Value Prize Incentives
* Brand Trust Exploitation
* Generic Recipient Targeting

---

### 7. Threat Classification

Based on the combined technical and behavioral indicators, the email was classified as:

**PHISHING / MALICIOUS**

Confidence Level:

**100% Confirmed Threat**

---

## Key Indicators of Compromise (IOCs)

### Suspicious Domains

* 7rye9ue08e.com
* hvshir.net
* fredseumneer.com
* dtherhproblem.us
* vertuoldmuneted.com

### Suspicious IP Address

* 166.1.22.115

### Authentication Failures

* SPF: Failed
* DKIM: Missing
* DMARC: Failed

---

## Attack Flow

1. Attacker sends spoofed phishing email.
2. User receives fake promotional offer.
3. User clicks embedded malicious link.
4. User is redirected to a fraudulent website.
5. Credentials or personal information are entered.
6. Information is transmitted to attacker-controlled infrastructure.

---

## Security Recommendations

### For End Users

* Verify sender email addresses.
* Hover over links before clicking.
* Avoid opening unexpected attachments.
* Report suspicious emails immediately.
* Never enter credentials through links received in emails.

### For Organizations

* Enforce SPF, DKIM, and DMARC policies.
* Deploy Secure Email Gateways (SEGs).
* Conduct regular phishing awareness training.
* Implement Multi-Factor Authentication (MFA).
* Monitor email authentication failures.

---

## Skills Demonstrated

* Phishing Email Analysis
* Email Header Investigation
* MXToolbox Usage
* Threat Intelligence
* Social Engineering Detection
* IOC Identification
* Security Awareness Reporting
* Technical Documentation
* Cybersecurity Risk Assessment

---

## Author

Cybersecurity Analyst Portfolio Project

This project was completed for phishing detection and cybersecurity awareness training purposes.
